# Krita-DDS-Addon
This is a fork of the following projects. It replaces the Texconv.exe/ImageMagick Dependency and replaces it with cbindings for a cross-platform lib of Texconv.
As of this post it's still a fork of the blender add-on solely, and I may deside to not use either of these dds add-ons as the base, and just use them as inspiration.

DDS File Exporter for Krita (GNU-V3):
https://krita-artists.org/t/python-plugin-dds-support-windows-only/73488
https://github.com/esuriddick/Programming/tree/main/Python/Krita/DDS_File_Exporter
https://github.com/esuriddick/Programming/tree/main/Python/Krita/DDS_File_Importer

-OR-
DDS-Evrika-Plugin (MIT):
https://github.com/Sepera-okeq/DDS-Evrika-Plugin

Blender-DDS-Addon (MIT):
https://github.com/matyalatte/Blender-DDS-Addon
https://github.com/matyalatte/Texconv-Custom-DLL

#### First Method
1. Open [Krita](https://krita.org) and go to _Tools_ > _Scripts_ > _Import Python Plugins..._, and select the **x.zip** archive.
2. Restart [Krita](https://krita.org).
3. Go to _Settings_ > _Configure Krita..._ > _Python Plugin Manager_, and click the checkbox to the left of the field that says **x**.
4. Restart [Krita](https://krita.org).

#### Second Method
1. Extract the content within the folder **x** to the folder **pykrita** (typically located here: C:\Users\USERNAME\AppData\Roaming\krita, where **USERNAME** should be replaced with your Windows username).
2. Restart [Krita](https://krita.org).
3. Go to _Settings_ > _Configure Krita..._ > _Python Plugin Manager_, and click the checkbox to the left of the field that says **DDS File Importer**.
4. Restart [Krita](https://krita.org).

### Execute
Go to the menu item _Tools_ > _Scripts_, and press the option named _Export DDS_. Choose the desired format to convert the DDS file into, and then it will appear in Krita.

## Download

## Getting Started

## Supported Formats

The addon supports most of the DXGI formats.  
  
Here is a list of supported formats.  

<details>
<summary>Supported DXGI Formats</summary>

* BC1_UNORM
* BC1_UNORM_SRGB
* BC2_UNORM
* BC2_UNORM_SRGB
* BC3_UNORM
* BC3_UNORM_SRGB
* BC4_UNORM
* BC4_SNORM
* BC5_UNORM
* BC5_SNORM
* BC6H_UF16
* BC6H_SF16
* BC7_UNORM
* BC7_UNORM_SRGB
* R32G32B32A32_FLOAT
* R32G32B32A32_UINT
* R32G32B32A32_SINT
* R32G32B32_FLOAT
* R32G32B32_UINT
* R32G32B32_SINT
* R16G16B16A16_FLOAT
* R16G16B16A16_UNORM
* R16G16B16A16_UINT
* R16G16B16A16_SNORM
* R16G16B16A16_SINT
* R32G32_FLOAT
* R32G32_UINT
* R32G32_SINT
* D32_FLOAT_S8X24_UINT
* R10G10B10A2_UNORM
* R10G10B10A2_UINT
* R11G11B10_FLOAT
* R8G8B8A8_UNORM
* R8G8B8A8_UNORM_SRGB
* R8G8B8A8_UINT
* R8G8B8A8_SNORM
* R8G8B8A8_SINT
* R16G16_FLOAT
* R16G16_UNORM
* R16G16_UINT
* R16G16_SNORM
* R16G16_SINT
* D32_FLOAT
* R32_FLOAT
* R32_UINT
* R32_SINT
* D24_UNORM_S8_UINT
* R8G8_UNORM
* R8G8_UINT
* R8G8_SNORM
* R8G8_SINT
* R16_FLOAT
* D16_UNORM
* R16_UNORM
* R16_UINT
* R16_SNORM
* R16_SINT
* R8_UNORM
* R8_UINT
* R8_SNORM
* R8_SINT
* A8_UNORM
* R1_UNORM
* R9G9B9E5_SHAREDEXP
* R8G8_B8G8_UNORM
* G8R8_G8B8_UNORM
* B5G6R5_UNORM
* B5G5R5A1_UNORM
* B8G8R8A8_UNORM
* B8G8R8X8_UNORM
* R10G10B10_XR_BIAS_A2_UNORM
* B8G8R8A8_UNORM_SRGB
* B8G8R8X8_UNORM_SRGB
* B4G4R4A4_UNORM
* A4B4G4R4_UNORM
* ASTC_4X4_UNORM
* ASTC_4X4_UNORM_SRGB
* ASTC_5X4_UNORM
* ASTC_5X4_UNORM_SRGB
* ASTC_5X5_UNORM
* ASTC_5X5_UNORM_SRGB
* ASTC_6X5_UNORM
* ASTC_6X5_UNORM_SRGB
* ASTC_6X6_UNORM
* ASTC_6X6_UNORM_SRGB
* ASTC_8X5_UNORM
* ASTC_8X5_UNORM_SRGB
* ASTC_8X6_UNORM
* ASTC_8X6_UNORM_SRGB
* ASTC_8X8_UNORM
* ASTC_8X8_UNORM_SRGB
* ASTC_10X5_UNORM
* ASTC_10X5_UNORM_SRGB
* ASTC_10X6_UNORM
* ASTC_10X6_UNORM_SRGB
* ASTC_10X8_UNORM
* ASTC_10X8_UNORM_SRGB
* ASTC_10X10_UNORM
* ASTC_10X10_UNORM_SRGB
* ASTC_12X10_UNORM
* ASTC_12X10_UNORM_SRGB
* ASTC_12X12_UNORM
* ASTC_12X12_UNORM_SRGB

</details>

## External Projects

### Texconv-Custom-DLL

[Texconv](https://github.com/microsoft/DirectXTex/wiki/Texconv)
is a texture converter developed by Microsoft, and [Texconv-Custom-DLL](https://github.com/matyalatte/Texconv-Custom-DLL) is a cross-platform implementation.  
The official Texconv only supports Windows but you can use it on Unix/Linux systems.  
It is released under the [MIT license](../LICENSE).

### astc-encoder

[astc-encoder](https://github.com/ARM-software/astc-encoder) is a texture converter for ASTC formats.  
It is released under the [Apache-2.0 license](https://github.com/ARM-software/astc-encoder?tab=Apache-2.0-1-ov-file#readme).

## License

Files in this repository are available under the [MIT license](../LICENSE).

## For Developers

There are some documents for developers.

- [How to Build](./How-To-Build.md): How to create a zip from the repository.
- [Tools for development](./For-Dev.md): How to test the addon.
