# StandtoCherax

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen)](#)
[![License](https://img.shields.io/badge/license-MIT-blue)](#)
[![Platform](https://img.shields.io/badge/platform-Windows-lightgrey)](#)
[![Cherax Compatible](https://img.shields.io/badge/cherax-supported-purple)](#)

**StandtoCherax** is a custom-made GTA V vehicle converter tool that converts **Stand Mod Menu .txt vehicle files** into **Cherax .json vehicle files**.

## 📦 Files Required

To use the `StandtoCherax.exe`, make sure the following files are in the **same folder** as the executable:

- `StandtoCherax.exe` ✅ *(The converter tool)*
- `Base.json` ✅ *(Base vehicle structure used to build output JSON)*
- `VehicleList.ini` ✅ *(Model name → hash mappings used for correct Cherax values)*

---

## 🚀 How to Use

1. **Run `StandtoCherax.exe`**
2. Click **"Open Stand Vehicle 📂"**
   - Select a **root folder** that contains subfolders (or itself) with `.txt` files exported from Stand Mod Menu.
3. Click **"🚀 Convert to Cherax .json(s)"**
   - The script will recursively search for `.txt` files in the root and all subfolders.
4. **Output Location:**
   - A new folder will be created named:  
     ```
     Cherax_<SelectedRootFolder>/
     ├── Cherax_<SubfolderName>/
     │   └── file1.json
     └── Cherax_<AnotherSubfolder>/
         └── file2.json
     ```

---

## ✅ Key Features

- Batch converts **all `.txt` files** from the selected folder **and all subfolders**
- Each subfolder becomes its own Cherax output folder (named `Cherax_<Subfolder>`)
- Outputs are neatly organized inside `Cherax_<RootFolder>`
- Includes GTA-styled UI with purple/pink gradient
- Automatically parses:
  - Vehicle mods, colors, neons, wheels, plate text, tints
  - Model hashes matched via `VehicleList.ini`

---

## 🛠 Troubleshooting

- 🟥 **Missing Base.json** → Place `Base.json` in the EXE folder
- 🟥 **Missing VehicleList.ini** → Required to resolve model names to hashes
- 🟨 **No `.txt` files found** → Ensure the folder or its subfolders contain `.txt` vehicle files

---

## 💬 Credits

- Created by **Bunny**  
- Discord `.itsBunny`

---

