Categories: categoryPath with split logic
Frontend form field:

Single text input: categoryPath
User types: "Components/Resistors" or just "Resistors"
Placeholder: "e.g. Components/Resistors or just Resistors"
Backend logic (server-side):

When user submits the form with categoryPath: "Components/Resistors":

Split by / → ["Components", "Resistors"]
Extract: mainCategoryName = "Components", subCategoryName = "Resistors"
Look up MainCategory by name:
If exists → use it
If not exists → create new MainCategory("Components") and save
Look up SubCategory by name + mainCategoryId:
If exists → use it
If not exists → create new SubCategory("Resistors", mainCategory) and save
Attach the SubCategory to the Product
Scenarios:

User input	Result
"Components/Resistors"	Creates MainCategory "Components" (if missing) + SubCategory "Resistors" under it
"Components/LEDs"	Creates MainCategory "Components" (if missing) + SubCategory "LEDs" under it
"Power/Connect"	Creates MainCategory "Power" (if missing) + SubCategory "Connect" under it
"Resistors"	Error or default behavior: either reject with "use format Main/Sub" OR treat as SubCategory under default MainCategory "General"
Edge cases & validation:

Empty string → reject with "Categoria is required"
"Components/" or "/Resistors" → reject with "Invalid format"
"Components/Resistors/Extra" → take first two parts, ignore rest (or reject)
Trimming: " Components / Resistors " → trim spaces, split works fine
