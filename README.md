# 📊 BOQ Exporter — Revit Add-in

<div align="center">

[![Revit API](https://img.shields.io/badge/Revit%20API-2022–2026-blue?style=for-the-badge&logo=autodesk)](https://www.autodesk.com/developer-network/platform-technologies/revit)
[![Language](https://img.shields.io/badge/C%23-.NET-purple?style=for-the-badge&logo=csharp)](https://dotnet.microsoft.com/)
[![Version](https://img.shields.io/badge/Version-1.0-green?style=for-the-badge)]()
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)]()

**A Revit API plugin that extracts quantities directly from your model and exports a fully formatted Bill of Quantities to Excel — automating one of the most tedious workflows in AEC.**

[▶️ Watch Demo Video](https://drive.google.com/file/d/1gkmRYRMwWQUn2vaoKT5IaMMfwbMvNPhM/view?usp=sharing) • [📥 Download Installer](https://github.com/MahmoudAllamAEC/BOQExporter/releases/tag/BimDev) • [📄 View Presentation](./BOQ_Exporter_Presentation.pdf)

</div>

---

## 🎬 Demo

> Click the thumbnail below to watch the full walkthrough

[![BOQ Exporter Demo](https://img.shields.io/badge/▶_Watch_Full_Demo-Google_Drive-red?style=for-the-badge&logo=google-drive)](https://drive.google.com/file/d/1gkmRYRMwWQUn2vaoKT5IaMMfwbMvNPhM/view?usp=sharing)

<!-- 💡 TO DO: Replace the line below with an actual screenshot of your plugin UI -->
<!-- ![BOQ Exporter UI](docs/screenshots/ui-preview.png) -->

---

## 🧩 What Problem Does It Solve?

In traditional AEC workflows, generating a Bill of Quantities requires:
- Manually counting elements category by category in Revit
- Copy-pasting data into Excel
- Formatting tables, adding charts, and calculating totals by hand

**BOQ Exporter eliminates all of that in one click.** Select your categories, enter project info, and get a professionally formatted Excel report — complete with summary tables, pie charts, and cost calculations — in seconds.

---

## ✨ Features

| Feature | Description |
|---|---|
| 📂 **Category Selection** | Choose which Revit categories to include in the BOQ |
| 📋 **Project Metadata** | Input Project Name, Client, Location, and Issue Date |
| 🏢 **Logo Embedding** | Add your company logo directly into the Excel output |
| 📊 **Detailed BOQ Report** | Quantities, unit rates, total cost, and remarks per item |
| 📑 **Summary Report** | Item usage counts across the entire model |
| 🥧 **Pie Chart Analysis** | Auto-generated category breakdown visualization |
| 🎨 **Formatted Output** | Alternating row shading, subtotals, professional layout |
| ⚙️ **Auto Installer** | One-click setup for all supported Revit versions |

---

## 🖥️ Screenshots

<div align="center">

<!-- 💡 TO DO: Add your actual screenshots below -->
<!-- Drag your screenshots into the repo under docs/screenshots/ then update these paths -->

| Plugin UI | Excel Output | Pie Chart |
|---|---|---|
| ![UI](https://github.com/MahmoudAllamAEC/BOQExporter/blob/master/Snipaste_2026-01-15_02-35-00.png) | ![Excel](https://github.com/MahmoudAllamAEC/BOQExporter/blob/master/Snipaste_2026-01-15_02-35-44.png) | ![Chart](https://github.com/MahmoudAllamAEC/BOQExporter/blob/master/Snipaste_2026-01-15_02-38-40.png) |

</div>

---

## 🔧 Tech Stack

- **Language:** C# / .NET Framework
- **API:** Autodesk Revit API
- **UI:** Windows Forms
- **Export:** EPPlus / Excel Interop
- **Packaging:** Custom installer (multi-version support)

---

## 📦 Installation

### Option 1 — Installer (Recommended)

1. Download the latest release from the [Releases page](https://github.com/MahmoudAllamAEC/BOQExporter/releases/tag/BimDev)
2. Run the setup file — it automatically installs for all detected Revit versions
3. Launch Revit and go to the **KAITECH-BD-R09** tab → **General** panel
4. Click **BOQ Exporter** to launch

### Option 2 — Manual

1. Clone this repository
2. Build the solution in Visual Studio
3. Copy the `.addin` manifest and `.dll` to:
   ```
   %APPDATA%\Autodesk\Revit\Addins\{RevitVersion}\
   ```

---

## ✅ Compatibility

| Revit Version | Status |
|---|---|
| Revit 2022 | ✅ Supported |
| Revit 2023 | ✅ Supported |
| Revit 2024 | ✅ Supported |
| Revit 2025 | ✅ Supported |
| Revit 2026 | ✅ Supported |

---

## 🚀 How to Use

1. Open any Revit project
2. Go to **KAITECH-BD-R09 tab → General → BOQ Exporter**
3. Select the element categories you want to include
4. Enter your project metadata (name, client, date, etc.)
5. Click **Extract** to preview grouped BOQ items
6. Click **Export** to generate the Excel report

---

## 📁 Project Structure

```
BOQExporter/
├── BOQExporter/          # Main plugin source code
│   ├── Commands/         # Revit external commands
│   ├── Forms/            # Windows Forms UI
│   ├── Models/           # Data models (BOQ items, categories)
│   └── Helpers/          # Excel export, formatting utilities
├── BOQ_Exporter_Presentation.pdf
├── BOQExporter.sln
└── README.md
```

---

## 🗺️ Roadmap

- [ ] WPF UI redesign (MVVM pattern)
- [ ] Filter by Revit phases and worksets
- [ ] PDF export option
- [ ] Multi-language support (Arabic / English)
- [ ] Cloud sync / BIM 360 integration

---

## 👤 Author

**Mahmoud Amr Allam**
Architect & BIM Software Developer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/mahmoud-allam-4a25b4172/)
[![Email](https://img.shields.io/badge/Email-mahmoud.amr55@gmail.com-red?style=flat-square&logo=gmail)](mailto:mahmoud.amr55@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-MahmoudAllamAEC-black?style=flat-square&logo=github)](https://github.com/MahmoudAllamAEC)

---

<div align="center">

⭐ **If this project helped you, please give it a star!** ⭐

</div>
