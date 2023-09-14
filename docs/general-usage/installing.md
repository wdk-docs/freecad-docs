# 安装附加组件

## 介绍

在为您的操作系统([Windows](https://wiki.freecad.org/Installing_on_Windows)， [Linux](https://wiki.freecad.org/Installing_on_Linux)或[Mac](https://wiki.freecad.org/Installing_on_Mac))安装 FreeCAD 后，您可能需要考虑安装以下一个或多个附加组件。

## 帮助文件

参见[安装帮助文件](https://wiki.freecad.org/Installing_Helpfile).

## 外部的工作台

除了与 FreeCAD 捆绑的默认工作台之外，还有大量有用的[外部工作台](https://wiki.freecad.org/External_workbenches)由社区成员制作。

## 第三方软件

FreeCAD 支持几个现成的第三方软件包。在许多情况下，你所需要做的就是安装软件，当 FreeCAD 重新启动时，它会自动找到并能够使用它。本节旨在提供这些软件包的列表，以及在 FreeCAD 中使用它们的位置和可以下载它们的位置的一些信息。

### 支持

#### GitPython

[GitPython](https://github.com/gitpython-developers/GitPython)是一个与 Git 存储库交互的库。[插件管理器](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/blob/main/src/pages/std-addonMgr.md)可以使用这个库。GitPython 包含在 Windows 和 Mac 的 FreeCAD 安装程序中。

#### GraphViz

[GraphViz](https://www.graphviz.org/)是一个开源的图形可视化软件。它被[Std DependencyGraph](https://wiki.freecad.org/Std_DependencyGraph)工具使用。

#### OpenCAMLib

[OpenCAMLib](http://www.anderswallin.net/CAM)是一个开源的计算机辅助制造(CAM)算法库。它在[Path Workbench](docs\ Workbench \ Path .md)中使用。请参阅[OpenCamLib](https://wiki.freecad.org/OpenCamLib)页面获取安装说明。

#### OpenSCAD

[OpenSCAD](https://www.openscad.org/)是一个实体 3D 建模器。[OpenSCAD Workbench](docs\workbenches\OpenSCAD.md)依赖于此软件，[Mesh Workbench](<docs\ Workbench\Mesh.md>)使用它作为其布尔工具。使用[Std import](https://wiki.freecad.org/Std_Import)工具导入 SCAD 文件时，也需要使用此命令。

### 文件格式

本节中的所有软件将由[Std Import](https://wiki.freecad.org/Std_Import)或[Std Export](https://wiki.freecad.org/Std_Export)工具使用。

#### CADExchanger

[CADExchanger](https://cadexchanger.com/)是一个用于交换各种 CAD 文件格式的商业应用程序。在 FreeCAD 中有一个[外部工作台](https://github.com/yorikvanhavre/CADExchanger)来使用这个应用程序。

#### DXF 导入器

FreeCAD 有 DXF 文件的本地导入和导出，用 c++编程。目前它们没有实现 DXF 格式的所有功能。对于这些特性，遗留的 Python 导入器和导出器仍然可用。这些需要[Draft-dxf-importer](https://github.com/yorikvanhavre/Draft-dxf-importer) Python 库。请参阅[FreeCAD 和 DXF 导入](https://wiki.freecad.org/FreeCAD_and_DXF_Import)页面了解更多信息。

#### DWG 转换器

FreeCAD 不能直接读写 DWG 文件。为了将 DXF 文件转换为 DWG 文件，反之亦然，FreeCAD 依赖于外部转换器。对以下 DWG 转换器的内置支持:

- [LibreDWG](https://www.gnu.org/software/libredwg) (open-source, lacks support for some DWG entities).
- [ODA File Converter](https://www.opendesign.com/guestfiles/oda_file_converter) (free, but not open-source).
- [QCAD pro](https://qcad.org/en/qcad-command-line-tools#dwg2dwg) (commercial). introduced in version 0.20

See [Import Export Preferences](https://wiki.freecad.org/Import_Export_Preferences#DWG) and [FreeCAD and DWG Import](https://wiki.freecad.org/FreeCAD_and_DWG_Import) for more information.

#### IfcOpenShell

[IfcOpenShell](http://ifcopenshell.org/) is a library for working with the Industry Foundation Classes (IFC) file format used in architectural design. The library is also used by the [Arch IfcExplorer](https://wiki.freecad.org/Arch_IfcExplorer) (version 0.18 and below) and BIM IfcExplorer tools. IfcOpenShell is included in the FreeCAD installers for Windows and Mac.

#### IfcJson

[IfcJson](https://github.com/buildingSMART/ifcJSON) is a library required for exporting to the IFCJSON file format. IFCJSON is a new IFC format that is not yet supported by many applications.

#### Pycollada

[Pycollada](https://github.com/pycollada/pycollada/releases), also known as python-collada, is a Python library to read and write Collada (DAE) files. Pycollada is included in the FreeCAD installers for Windows and Mac.

### 渲染

#### LuxCoreRender

[LuxCoreRender](https://www.luxcorerender.org/) is a render engine, reboot of the [LuxRender](https://wiki.freecad.org/LuxRender) project. Officially it is not supported by the [Raytracing Workbench](https://wiki.freecad.org/Raytracing_Workbench), but it might be worth to give it a try. It is officially supported by the new [Render Workbench](https://github.com/FreeCAD/FreeCAD-render), intended as a future replacement of the Raytracing Workbench. See the [LuxCoreRender](https://wiki.freecad.org/LuxCoreRender) page for more information and installation instructions.

#### LuxRender

[LuxRender](https://luxcorerender.org/history/) is one of the two render engines supported by the [Raytracing Workbench](https://wiki.freecad.org/Raytracing_Workbench). In 2013 the project has been rebooted becoming [LuxCoreRender](https://wiki.freecad.org/LuxCoreRender), with a major code rewriting and compatibility breaking changes. Officially the Raytracing Workbench only supports the abandoned [LuxRender](https://wiki.freecad.org/LuxRender) (latest version is 1.6, 2017-12-28), while the new [Render Workbench](https://github.com/FreeCAD/FreeCAD-render) (intended as a future replacement of the Raytracing Workbench) supports instead LuxCoreRender and has dropped the support for LuxRender. Anyway, even if officially not supported, [LuxCoreRender](https://wiki.freecad.org/LuxCoreRender) may work with the Raytracing Workbench, it might be worth to give it a try. See the [LuxRender](https://wiki.freecad.org/LuxRender) page for more information and installation instructions, and the [LuxCoreRender](https://wiki.freecad.org/LuxRender) if you want to try a more modern software.

#### POV-Ray

[POV-Ray](https://www.povray.org/) is a well-known ray-tracer which can render photo-realistic images. It is one of two render engines currently supported by the [Raytracing Workbench](https://wiki.freecad.org/Raytracing_Workbench). See the [POV-Ray](https://wiki.freecad.org/POV-Ray) page for more information and installation instructions.

### 有限元

#### CalculiX

[CalculiX](http://calculix.de/) is a suite of two finite element packages: CalculiX CrunchiX, a FEM solver, and CalculiX GraphiX, a GUI frontend. Only the solver is supported by FreeCAD. It is used by the [Solver CalculiX](https://wiki.freecad.org/FEM_SolverCalculiX) tool.

#### Gmsh

[Gmsh](http://gmsh.info/) is an automatic finite element mesh generator. it is used by the [FEM MeshGmshFromShape](https://wiki.freecad.org/FEM_MeshGmshFromShape) and [Mesh FromPartShape](https://wiki.freecad.org/Mesh_FromPartShape) tools.

#### Elmer

[Elmer](https://www.csc.fi/web/elmer) is a multi-physics simulation software, which was open sourced in 2005. In FreeCAD its Grid and Solver modules are used by the [FEM SolverElmer](https://wiki.freecad.org/FEM_SolverElmer) tool.

#### FEniCS

[FEniCS](https://fenicsproject.org/) is a computing platform to solve partial differential equations (PDEs), which are widely used when solving FEM problems. It is used by the [FEM workbench](docs\workbenches\FEM.md).

#### Z88

[Z88](https://en.z88.de/) is another FEM program, containing a mesher, a solver and converters. It is used by the [FEM SolverZ88](https://wiki.freecad.org/FEM_SolverZ88) tool. FreeCAD requires the open source Z88OS package.

#### OpenFOAM

[OpenFOAM](https://openfoam.org/) is a large collection of libraries for computational fluid dynamics (CFD) simulations. OpenFOAM is used by the [Cfd](https://wiki.freecad.org/Cfd_Workbench) and [CfdOF](https://github.com/jaheyns/CfdOF) [external workbenches](docs\workbenches\external-workbenches.md).

## 相关页面

- [导入导出](https://wiki.freecad.org/Import_Export)
- [导入导出偏好](https://wiki.freecad.org/Import_Export_Preferences)
- [第三方图书馆](https://wiki.freecad.org/Third_Party_Libraries)
