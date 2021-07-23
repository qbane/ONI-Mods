# About this fork

tl;dr. The author did some extreme trial-and-error to finally successfully port the mod to Linux. The hard work deserves a fork. \
See the [original discussion thread](https://steamcommunity.com/workshop/filedetails/discussion/2070840646/3044978964803635873) for details. 

# Instructions on building your own font asset bundles

**Section 1**: Generating a font asset

1. Install Unity 2018.x (should be on Windows).
2. Create a new project with TextMesh Pro (its version **must** be v1.2.x) package. \
   The package manager can be found in **Windows** > **Package Manager**.
3. Add your font file as an asset.
4. Navigate to **Windows** > **TextMesh Pro**. Import the **TMP Essentials** and create a font asset there.
5. (Optional) Click the little triangle on your newly-created asset. Change the shader of its material to "TextMesh Pro/Mobile/Distance Field".

**Section 2**: Generating an asset bundle (OS-dependent)

1. Depending on the operating system you are going to support:

   * **Windows**: Continue to use the project in Section 1.
   * **Linux/macOS**: Prepare a separate Unity 2018.x environment with the specified TextMesh Pro version on either Linux or macOS. The generated file seems to be interchangable at least for now, thus the `generic` named font file in this repository.

2. Install Asset bundle browser (v1.7.0). Navigate to **Windows** > **Asset bundle browser**.
3. Drag/Import the generated font asset to the **Configure** panel.
4. In the **Build** panel, select the platform of the form "[YOUR_CURRENT_OS] Standalone 64" and build.
5. The result will be at `/Asset Bundles/[PLATFORM]/[ASSET_NAME]` under your project directory.

Tested fonts:

1. Noto Sans CJK TC (`NotoSansCJKtc-Regular`): https://github.com/miZyind/ONI-Mods (*Upstream*)
2. jf open 粉圓 (`open-jfhuninn`): https://github.com/dershiuan/ONI-Mods

The original README goes below.

---

# miZyind's ONI Mods
[![ONI](https://img.shields.io/badge/oxygen_not_included-000?style=for-the-badge&logo=steam)](https://store.steampowered.com/app/457140/Oxygen_Not_Included)
[![Unity](https://img.shields.io/badge/unity-000?style=for-the-badge&logo=unity)](https://unity.com)
[![Visual Studio](https://img.shields.io/badge/2019-5c2d91?style=for-the-badge&logo=visual-studio)](https://visualstudio.microsoft.com)
[![.NET](https://img.shields.io/badge/4.7.1-5c2d91?style=for-the-badge&logo=.net)](https://dotnet.microsoft.com)
[![C#](https://img.shields.io/badge/4.0-239120?style=for-the-badge&logo=c-sharp)](https://docs.microsoft.com/dotnet/csharp)

## 🔮 Tested Game Version
- **FA-471883-B & EX1-S14-471883-S**
- **CS-469300 & MD-469473 & EX1-S13-469473**
- **CS-460672 & EX1-S10-461546**
- **CS-455509 & EX1-S8-455425**
- **CS-449460 & EX1-S6-449549**
- **CS-444111**
- **AP-410209**
- **AP-399948**

## 🙏 Thanks To
- @Cairath for [Oxygen-Not-Included-Modding](https://github.com/Cairath/Oxygen-Not-Included-Modding)
- @peterhaneve for [PLib](https://github.com/peterhaneve/ONIMods/tree/main/PLib)
- @古靈精怪 for [繁體中文語言包](https://steamcommunity.com/sharedfiles/filedetails/?id=929305589)
- @Kud for [繁體中文語言包](https://steamcommunity.com/sharedfiles/filedetails/?id=1562134514)
- @LaFa for [拉法繁中](https://steamcommunity.com/sharedfiles/filedetails/?id=1123693010)
- @Jiun for [非官方繁中](https://steamcommunity.com/sharedfiles/filedetails/?id=1821957996)
- @qbane for [類 Unix 作業系統相容性](https://steamcommunity.com/workshop/filedetails/discussion/2070840646/3044978964803635873)

## 💠 Development Environment & Tools
- ILRepack >= 2.0.x
- PLib >= 4.2
- Harmony >= 2.0.x
- .NET Framework = 4.7.1
- Unity = 2018.4.14f1
- TextMesh Pro = 1.2.3
- Visual Studio 2019
- Asset Studio GUI
- Asset Bundle Extractor
- dnSpy

## 🗂 Mod List
|                                           Name                                           	|                   Description                   	|
|:----------------------------------------------------------------------------------------:	|:-----------------------------------------------:	|
| [Traditional Chinese](https://steamcommunity.com/sharedfiles/filedetails/?id=2070840646) 	| Adds Traditional Chinese translation and font.  	|

## 🖋 Author
miZyind <mizyind@gmail.com>

## 📇 License
Licensed under the [MIT](LICENSE) license.
