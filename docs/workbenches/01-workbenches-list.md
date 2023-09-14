# 工作台

FreeCAD，像许多现代设计应用程序，如[Revit](http://en.wikipedia.org/wiki/Revit)或[CATIA](http://en.wikipedia.org/wiki/CATIA)，是基于[工作台](http://en.wikipedia.org/wiki/Workbench)的概念。工作台可以被看作是一组专门为某项任务分组的工具。在传统的家具车间里，你会有一张工作台给处理木材的人，另一张工作台给处理金属件的人，可能还有第三张工作台给把所有的东西装在一起的人。

在 FreeCAD 中，同样的概念也适用。工具根据与之相关的任务分组到工作台中。

当您从一个工作台切换到另一个工作台时，界面上可用的工具会发生变化。工具栏、命令栏和界面的其他部分可能会切换到新的工作台，但场景的内容不会改变。例如，您可以使用 Draft Workbench 开始绘制 2D 形状，然后使用 Part Workbench 进一步处理它们。

请注意，有时工作台被称为模块。然而，工作台和模块是不同的实体。模块是 FreeCAD 的任何扩展，而工作台是具有 GUI 配置(工具栏和菜单)的特殊类型的模块。

## 内置的工作台

### 当前的

以下工作台与每个 FreeCAD 安装捆绑在一起:

- ![image](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/a1b5489b-e947-4077-bcf2-182be03aba7f) [Std 基地](https://wiki.freecad.org/Std_Base): 这不是一个真正的工作台，而是一个可以在所有工作台中使用的`标准`命令和工具的类别。
- ![Arch workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/9bc2e291-8e10-4ce0-b374-12641eab454b) [Arch 工作台](docs\workbenches\arch.md) 用于处理架构元素。
- ![Draft workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/c25772d8-13c4-42b5-8c8c-eba8f64a2b7e) [草案工作台](docs\workbenches\draft.md) 包含 2D 工具和基本的 2D 和 3D CAD 操作。
- ![FEM workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/0c46ed4f-c7fd-4bf0-b46a-272094dc0950) [FEM 工作台](docs\workbenches\FEM.md) 提供有限元分析(FEA)工作流程。
- ![Inspection workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/7ced53a7-47e0-49e4-b729-3773302cb32a) [检查工作台](https://wiki.freecad.org/Inspection_Workbench) 为您提供用于检查形状的特定工具。它仍在开发中。
- ![Mesh workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/318d08a6-98b7-4ee0-95a2-28690889869d) [网格工作台](docs\workbenches\mesh.md) 用于处理三角网格。
- ![OpenSCAD workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/ce16fe57-0d12-4cb6-b444-f256bc397a02) [OpenSCAD 工作台](docs\workbenches\openSCAD.md) 用于与 OpenSCAD 的互操作性和修复[构造立体几何](https://wiki.freecad.org/Constructive_solid_geometry) (CSG)模型历史。
- ![Part workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/19f56635-c537-4a75-81e2-1e1f28710a91) [零件工作台](docs\workbenches\part.md) 用于处理几何原语和布尔运算。
- ![Part design workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/660dd17a-4d37-4d6c-805a-b18481ecb5ec) [零件设计工作台](docs\workbenches\part-design.md) 用于从草图中构建零件形状。
- ![Path workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/26670d8a-4368-4b10-97e1-0353e58d4dc6) [路径工作台](docs\workbenches\path.md) 用于生成 G-Code 指令。它仍在开发中。
- ![Points workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/bd5219d3-3525-4d57-b5f2-722d78527c4b) [点工作台](docs\workbenches\points.md) 用于处理点云。
- ![Reverse engineering workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/595f8bfe-d76a-4483-9c79-15919a78b989) [逆向工程工作台](https://wiki.freecad.org/Reverse_Engineering_Workbench) 旨在提供特定的工具来将形状/实体/网格转换为参数化的 freecad 兼容功能。它仍在开发中。
- ![Robot workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/76a45cc5-ab25-487e-afbf-a27d1e9826da) [机器人工作台](docs\workbenches\robot.md) 用来研究机器人的动作。
- ![Sketcher workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/99c4b539-a016-411b-90ab-e0411f37b4db) [舞台布景设计者工作台](docs\workbenches\sketcher.md) 用于处理几何约束的草图。
- ![Spreadsheet workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/29cc4d05-5850-4cc2-a5d4-6188cf06bfae) [电子表格工作台](docs\workbenches\spreadsheet.md) 用于创建和操作电子表格数据。
- ![image](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/ef4538cf-4880-442c-8de6-e6115b9195fd) [启动中心工作台](https://wiki.freecad.org/Start_Workbench) 允许您快速跳转到最常见的工作台之一。
- ![Surface workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/3cc434a8-1e49-483e-8fc9-65710d005ddf) [表面工作台](docs\workbenches\surface.md) 提供创建和修改表面的工具。它类似于[零件生成器](https://wiki.freecad.org/Part_Builder)从边缘选择面。
- ![TechDraw workbench logo](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/6fd5f4c1-b941-4047-b8fa-e14eb5ae8c60) [TechDraw 工作台](docs\workbenches\techdraw.md) 用于从 3D 模型生成技术图纸。它是[绘图工作台](https://wiki.freecad.org/Drawing_Workbench)的继承者。
- ![image](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/5e3df28c-0bf9-4d17-972c-7ed06656c222) [测试框架工作台](https://wiki.freecad.org/Testing) 用于调试 FreeCAD。
- ![image](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/178b7150-cce0-471e-a5be-a990eb83ea63) [Web 工作台](https://wiki.freecad.org/Web_Workbench) 为您提供了一个浏览器窗口，而不是[3D 视图](https://wiki.freecad.org/3D_view)在 FreeCAD。

### 过时了

以下工作台在 0.20 版本之后不再包含:

- ![image](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/f7332799-41a3-4e1c-b0cf-8f36162fb52a) [绘制工作台](https://wiki.freecad.org/Drawing_Workbench)用于制作技术图纸。 [TechDraw 工作台](https://wiki.freecad.org/TechDraw_Workbench)是它更先进的替代品。
- ![image](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/c822d08d-0fa3-4d78-872c-9ea127ab3c5f) [图像工作台](https://wiki.freecad.org/Image_Workbench)用于处理位图图像。 它的功能已经集成在[Std Base](https://wiki.freecad.org/Std_Base)中。参见[Std Import](https://wiki.freecad.org/Std_Import)和[Std ViewLoadImage](https://wiki.freecad.org/Std_ViewLoadImage)。
- ![image](https://github.com/gauriimaheshwarii/FreeCAD-documentation/assets/100439627/e0f3dc95-6648-4037-9f45-86ec7abc49f0) [射线追踪工作台](https://wiki.freecad.org/Raytracing_Workbench) 用于光线追踪(渲染)。 应该使用外部的[渲染工作台](https://github.com/FreeCAD/FreeCAD-render)。

## 外部的工作台

FreeCAD 工作台很容易在[Python](docs\python-scripting\pyside.md)中编程，因此有许多人在 FreeCAD 主开发区域之外开发额外的工作台。

[外部工作台](docs\workbenches\external-workbench.md)页面列出了这个社区所知道的所有内容。大多数很容易安装从 FreeCAD 内，使用[插件管理器](https://wiki.freecad.org/Std_AddonMgr)，在菜单下找到**工具 →![图像](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/ce42afc3-28a7-4f16-8fff-31b4e5f27237)插件管理器**。
