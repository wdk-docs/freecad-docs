# 特性列表

This is an extensive, but not complete, list of features which FreeCAD implements.

## 发布说明

- [Release 0.20](https://wiki.freecad.org/Release_notes_0.20) - June 2022
- [Release 0.19](https://wiki.freecad.org/Release_notes_0.19) - March 2021
- [Release 0.18](https://wiki.freecad.org/Release_notes_0.18) - March 2019
- [Release 0.17](https://wiki.freecad.org/Release_notes_0.17) - April 2018
- [Release 0.16](https://wiki.freecad.org/Release_notes_0.16) - April 2016
- [Release 0.15](https://wiki.freecad.org/Release_notes_0.15) - March 2015
- [Release 0.14](https://wiki.freecad.org/Release_notes_0.14) - March 2014
- [Release 0.13](https://wiki.freecad.org/Release_notes_0.13) - January 2013
- [Release 0.12](https://wiki.freecad.org/Release_notes_0.12) - December 2011
- [Release 0.11](https://wiki.freecad.org/Release_notes_0.11) - March 2011

## 关键特性

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/18b4e939-5746-48b8-8993-c197df5f4611)  
  一个完整的[开放级联技术](http://en.wikipedia.org/wiki/Open_CASCADE)-based **几何内核**允许在复杂形状类型上进行复杂的 3D 操作，具有对[边界表示](https://en.wikipedia.org/wiki/Boundary_representation) (BREP)，[非均匀有理基样条](https://en.wikipedia.org/wiki/Non-uniform_rational_B-spline) (NURBS)曲线和曲面等概念的原生支持，广泛的几何实体，布尔运算和[fillets](<https://en.wikipedia.org/wiki/Fillet_(mechanics)>)，以及内置的[STEP](https://en.wikipedia.org/wiki/ISO_10303)和[IGES](https://en.wikipedia.org/wiki/IGES)格式支持。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/2e318415-ed0c-418f-9860-34865b392023)  
  一个完整的参数模型。所有 FreeCAD 对象本身都是参数化的，这意味着它们的形状可以基于[属性](https://wiki.freecad.org/Property)，甚至依赖于其他对象。根据需要重新计算所有更改，并由撤销/重做堆栈记录。可以很容易地添加新的对象类型，甚至可以[完全用 Python 编程](https://wiki.freecad.org/Scripted_objects)。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/83835ee2-fc88-4048-b8c4-790d9bfe6005)  
  模块化架构，允许插件扩展(模块)向核心应用程序添加功能。扩展可以像用 c++编写的整个新应用程序一样复杂，也可以像 Python 脚本或自记录宏一样简单。您可以从内置的**Python**解释器，宏或外部脚本中完全访问 FreeCAD 的几乎任何部分，无论是[几何图形创建和转换](https://wiki.freecad.org/Topological_data_scripting)，该几何图形的 2D 或 3D 表示([scenegraph](https://wiki.freecad.org/Scenegraph))甚至[FreeCAD 接口](docs\Python-scripting\pyside.md)。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/eb3b2ef4-6e5d-4137-bb54-f9ef60f0d72c)  
  **导入/导出**等标准格式[步骤](http://en.wikipedia.org/wiki/ISO_10303), [IGES](http://en.wikipedia.org/wiki/IGES), [OBJ](http://en.wikipedia.org/wiki/Obj), [STL](http://en.wikipedia.org/wiki/STL_%28file_format%29), [DXF](http://en.wikipedia.org/wiki/Dxf), [SVG](http://en.wikipedia.org/wiki/Svg), [DAE](http://en.wikipedia.org/wiki/COLLADA),[国际金融公司](http://en.wikipedia.org/wiki/Industry_Foundation_Classes),或[关闭](http://people.sc.fsu.edu/~jburkardt/数据/off.html),[NASTRAN](http://en.wikipedia.org/wiki/NASTRAN)， [VRML](http://en.wikipedia.org/wiki/VRML)除了 FreeCAD 的本地**[FCStd](https://wiki.freecad.org/File_Format_FCStd)**)文件格式。FreeCAD 和给定文件格式之间的兼容性级别可能会有所不同，因为它取决于实现它的模块。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/2edcff1e-a597-4694-b277-0bdaafc30bbe)  
  [Sketcher](docs\workbench\Sketcher.md)集成约束求解器，允许您绘制几何约束的 2D 形状。使用 Sketcher 构建的受限 2D 形状可以作为在 FreeCAD 中构建其他对象的基础。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/1440bb6a-fd84-4a7c-a614-1ac8d987d232)  
  一个[机器人仿真](docs\workbench\Robot.md)模块，允许您在图形环境中研究机器人的运动。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/c8ff8f2a-02e4-4ea0-b0d8-d7484527d7f7)  
  一个[技术绘图模块](docs\workbench\techdraw.md)，具有详细视图，横断面视图，尺寸和其他选项，允许您生成现有 3D 模型的 2D 视图。然后，该模块生成准备导出的 SVG 或 PDF 文件。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/f2239533-28f6-4b8b-b0ac-f832a89319f6)  
  一个[Rendering](https://wiki.freecad.org/Raytracing_Workbench)模块，可以导出 3D 对象以使用外部渲染器进行渲染。它目前只支持[povray](http://en.wikipedia.org/wiki/POV-Ray)和[LuxRender](http://en.wikipedia.org/wiki/LuxRender)，但预计将来会扩展到其他渲染器。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/891cecda-f7c7-4677-9e80-912ba32860a8)  
  一个[架构模块](docs\workbench\arch.md)，允许[建筑信息模型](http://en.wikipedia.org/wiki/Building_Information_Modeling) (BIM)类似的工作流与[工业基础类](http://en.wikipedia.org/wiki/Industry_Foundation_Classes) (IFC)兼容。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/6347cfa2-4ca3-4e98-9a9b-0360d9bd8a6e)  
  专用于[计算机辅助制造](https://en.wikipedia.org/wiki/Computer-aided_manufacturing) (CAM)的机械加工的[路径模块](docs\workbench\Path.md)。使用 Path 模块，您可以输出、显示和调整用于控制目标机器的[G 代码](http://en.wikipedia.org/wiki/G-code)。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/e4216e76-cb9d-4416-b3cd-59cb49527d40)  
  一个[集成电子表格](docs\workbench\Spreadsheet.md)和一个[表达式解析器](https://wiki.freecad.org/Expressions)，可用于驱动基于公式的模型并在中心位置组织模型数据。

## 一般特征

- **多平台**: FreeCAD 在 Windows、Linux、macOS 和其他平台上的运行和行为完全相同。
  - **完整 GUI 应用程序**: FreeCAD 拥有基于[Qt](https://www.qt.io/)框架的完整图形用户界面，以及基于[Open Inventor](http://en.wikipedia.org/wiki/Open_Inventor)的 3D 查看器;允许快速渲染 3D 场景和非常易于访问的场景图形表示。
- **作为命令行应用程序运行**: 在命令行模式下，FreeCAD 在没有界面的情况下运行，但是有它所有的几何工具。在这种模式下，它具有相对较低的内存占用，并且可以用作(例如)为其他应用程序生成内容的服务器。
- **可以作为[Python 模块](https://wiki.freecad.org/Embedding_FreeCAD)导入**: FreeCAD 可以导入到任何可以运行 Python 脚本的应用程序中。在命令行模式下，FreeCAD 的界面部分不可用，但所有的几何工具都是可访问的。
- **工作台的概念**: 在 FreeCAD 界面中，工具按工作台分组。这允许您仅显示用于完成特定任务的工具，保持工作区整洁和响应，并允许应用程序快速加载。
- **插件/模块框架，用于后期加载功能/数据类型**: FreeCAD 被划分为核心应用程序，只有在需要时才加载模块。几乎所有的工具和几何类型都存储在模块中。模块的行为就像插件;除了延迟加载之外，还可以在现有的 FreeCAD 安装中添加或删除单个模块。
- **参数化关联文档对象**: FreeCAD 文档中的所有对象都可以通过参数定义。这些参数可以随时修改和重新计算。由于维护了对象关系，因此对一个对象的修改将自动传播到任何依赖的对象。
- **参数原语创建**: 可以通过指定它们的几何约束来创建诸如盒子、球体、圆柱体等基本对象。
- **图形修改操作**: FreeCAD 可以在 3D 空间的任何平面上执行平移，旋转，缩放，镜像，偏移(无论是琐碎的还是如[Jung/Shin/Choi](https://www.researchgate.net/publication/240754626_Self-intersection_Removal_in_Triangular_Mesh_Offsetting)所描述的)或形状转换。
- **[构造立体几何](https://wiki.freecad.org/Constructive_solid_geometry)** (布尔操作): FreeCAD 可以做建设性的立体几何运算(并、差、相交)。
- **平面几何图形的创建**: 线、线、矩形、b 样条、圆弧或椭圆弧可以在三维空间的任何平面上图形化地创建。
- **建模与直或旋转挤出**，**节**，**圆角**。
- **拓扑组件**像**顶点**，**边**，**线**和**面**。
- **测试和修理**: FreeCAD 有测试网格的工具(实体测试、非双流形测试、自交测试)和修复网格的工具(补孔、均匀定向)。
- **注释**: FreeCAD 可以为文本或尺寸插入注释。
- **撤销/重做框架**: FreeCAD 中的所有内容都是可撤销/可重做的，用户可以访问撤销堆栈。可以一次撤消多个步骤。
- **面向事务的**: 撤销/重做堆栈存储文档事务，而不是单个操作，允许每个工具精确定义必须撤销或重做的内容。
- **内置[脚本](https://wiki.freecad.org/Scripting)框架**: FreeCAD 具有内置的[Python](https://wiki.freecad.org/Scripting)解释器，其 API 几乎涵盖了应用程序的任何部分，接口，几何形状以及 3D 查看器中该几何形状的表示。解释器可以运行复杂的脚本，也可以运行单个命令;整个模块可以完全用 Python 编程。
- **内置 Python 控制台**: Python 解释器包括一个带有语法高亮显示、自动完成和类浏览器的控制台。Python 命令可以直接在 FreeCAD 中发出并立即返回结果，允许脚本编写者动态测试功能，探索 FreeCAD 模块的内容并轻松了解 FreeCAD 的内部结构。
- **反映用户交互**: 用户在 FreeCAD 界面中执行的所有操作都执行 Python 代码，这些代码可以打印在控制台上并记录在宏中。
- **完整的宏记录和编辑功能**: 当用户操作界面时发出的 Python 命令可以被记录，如果需要的话可以编辑，并保存以供以后复制。
- **复合(基于 ZIP 的)文档保存格式**: FreeCAD 文档以**[.FCStd](https://wiki.freecad.org/File_Format_FCStd)**扩展名)保存。文档可以包含许多不同类型的信息，如几何图形、脚本或缩略图图标。**.FCStd**文件本身是一个 zip 容器;已保存的 FreeCAD 文件已被压缩。
- **完全可定制/可编写脚本的图形用户界面**: FreeCAD 的[Qt](https://www.qt.io/)-based)接口完全可以通过 Python 解释器访问。除了 FreeCAD 本身提供给工作台的简单函数外，整个 Qt 框架都是可访问的。用户可以在 GUI 上执行任何操作，例如创建、添加、对接、修改或删除小部件和工具栏。
- **缩略图器**: (目前仅限 Linux 系统)FreeCAD 文档图标在大多数文件管理器应用程序(如 Gnome 的 Nautilus)中显示文件内容。
- **模块化 MSI 安装程序**: FreeCAD 的安装程序允许在 Windows 系统上灵活安装。Ubuntu 系统的软件包也被维护。

## 额外的工作台

高级用户创建了各种定制的[外部工作台](docs\workbenches\external-workbenches.md).
