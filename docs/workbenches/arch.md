# 拱工作台

## 介绍

![Arch-Workbench](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/4c866953-d6f1-487d-9adf-b0686f135acf) Arch Workbench 为 FreeCAD 提供了一个现代的[**B**建筑**I**信息**M**建模](http://en.wikipedia.org/wiki/Building_Information_Modeling) (BIM)工作流，支持完全参数化的建筑实体，如墙壁、梁、屋顶、窗户、楼梯、管道和家具。
它支持[**I**行业**F**基金会**C**类](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/blob/main/src/pages/workbenches/arch-ifc.md) (IFC)文件，并结合制作 2D 平面图![图片](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/44a4ccdf-bee2-455e-88c0-b07d8514e1b4)
[TechDraw 工作台](docs\workbenches\techdraw.md)。

Arch 工作台从![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/ff077e19-016d-4c8e-bd3a-2b4e1acc355a) [Draft Workbench](docs\workbenches\draft.md)中导入所有工具，因为它使用其 2D 对象来构建 3D 参数化建筑对象。不过，Arch 也可以使用其他工作台创建的实体形状，比如![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/028a5b15-4e61-4a62-aeb5-7585d1f06cbe)
[Part](docs\workbenches\part.md)和![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/56be3f73-55b1-4edb-aeba-1cbb6e72b157) [PartDesign](docs\workbenches\part-design.md)。

FreeCAD 的 BIM 功能现在逐渐分为 Arch Workbench(包含基本的建筑工具)和![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/b6c3b0bc-e1e2-434d-9a29-db571b8e3b40) [BIM 工作台](https://wiki.freecad.org/BIM_Workbench)。可从![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/c547761c-5283-4fcf-8e87-3bdb84912e52) [Addon Manager](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/blob/main/src/pages/std-addonMgr.md)获得。这个 BIM 工作台在 Arch 工具的基础上增加了一个新的界面层，目的是使 BIM 工作流程更加直观和用户友好。参见[FreeCAD BIM 迁移指南](https://yorik.uncreated.net/blog/2020-010-freecad-bim-guide).

Draft、Arch 和 BIM 的开发者也与更大的[OSArch 社区](https://osarch.org/)合作，最终目标是通过使用完全免费的软件来改进建筑设计。

![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/49d6512a-4ec0-4141-9a4f-3497641de6bc)

## 工具

这些是用于创建体系结构对象的工具。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/ba323bb1-ea1f-4b29-b67b-4491aa4b7444) [墙](https://wiki.freecad.org/Arch_Wall): 从头开始或使用选定的对象作为基础创建墙壁。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/85e212c6-2a8e-4f6d-a469-60cfcdc5126a) [结构](https://wiki.freecad.org/Arch_Structure): 从头开始或使用选定的对象作为基创建结构元素。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/3a422b82-e941-43a1-a39f-d74fe267e60b) [力霸工具](https://wiki.freecad.org/Arch_CompRebarStraight): 这些工具只有在安装了[强化工作台](https://wiki.freecad.org/Reinforcement_Workbench)后才可用。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/a5bd2f2f-ef90-44c7-88b4-a14fe67f5411) [直钢筋](https://wiki.freecad.org/Arch_Rebar_Straight): 在选定的结构单元中创建直钢筋。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/f1e931ee-9e86-4e44-a873-8b5080ebe12d) [U 形钢筋](https://wiki.freecad.org/Arch_Rebar_UShape): 在选定的结构单元中创建 U 形钢筋。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/3f3414a8-3c3a-4a85-89ea-d7deef8d9bac) [上海力霸](https://wiki.freecad.org/Arch_Rebar_LShape): 在选定的结构单元中创建 L 形钢筋。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/b2e9a9df-99bc-4ca8-baf4-014fd73b0f55) [箍筋](https://wiki.freecad.org/Arch_Rebar_Stirrup): 在选定的结构元件中创建箍筋钢筋。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/8fa0b0f9-87c4-4e2e-9551-3bc75476e137) [弯曲形状钢筋](https://wiki.freecad.org/Arch_Rebar_BentShape): 在选定的结构单元中创建弯形钢筋。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/9b51f41c-9baa-43e3-af16-575d8ce81e6a) [螺旋钢筋](https://wiki.freecad.org/Arch_Rebar_Helical): 在选定的结构元件中创建螺旋钢筋。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/032cc31b-71c3-49fb-8115-241475e6dbff) [柱钢筋](https://wiki.freecad.org/Arch_Rebar_ColumnReinforcement): 在选定的矩形列中创建钢筋。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/03e7c0eb-6cbf-4534-b271-c7badb6769f5) [梁配筋](https://wiki.freecad.org/Arch_Rebar_BeamReinforcement): 在选定的梁中创建钢筋。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/53ae1981-3386-4f2a-9321-a18e6609e894) [面板钢筋](https://wiki.freecad.org/Arch_Rebar_Slab_Reinforcement): 在选定的板上创建钢筋。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/e6be62de-06cd-4879-967f-c60f75bc9681) [基础钢筋](https://wiki.freecad.org/Arch_Rebar_Footing_Reinforcement): 在选定的基础内创建钢筋。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/6f808878-7418-4902-80eb-82b1b35f1a8b) [自定义钢筋](https://wiki.freecad.org/Arch_Rebar): 使用草图在选定的结构元素中创建自定义钢筋。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/597e506c-a3d7-4725-8f04-e1e352fe29d8) [幕墙](https://wiki.freecad.org/Arch_CurtainWall): 从头开始或使用选定的对象作为基础创建幕墙。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/a8dab72e-ec59-485c-b181-19480a3aea33) [建筑部分](https://wiki.freecad.org/Arch_BuildingPart): 创建包含选定对象的建筑部件。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/efc96ab3-9e46-44d6-aa39-2d73b0502f8e) [项目](https://wiki.freecad.org/Arch_Project): 创建包含选定对象的项目。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/a19687e4-e3f8-4e38-9501-05f43865a898) [网站](https://wiki.freecad.org/Arch_Site): 创建包含选定对象的站点。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/9a30d863-e0fc-4085-9d91-af163b7f5406) [建筑](https://wiki.freecad.org/Arch_Building): 创建包含选定对象的建筑物。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/a2fd9dfd-7fdf-4b20-801f-78c7e6adebaa) [水平](https://wiki.freecad.org/Arch_Floor): 创建包含选定对象的地板。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/952544af-e7b0-4be1-9025-cfd62ef76ad8) [外部引用](https://wiki.freecad.org/Arch_Reference): 将对象从另一个 FreeCAD 文件链接到当前文档。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/9a463af1-741c-4dad-a30d-c31170f65d67) [窗口](https://wiki.freecad.org/Arch_Window): 从头开始或使用选定对象作为基创建窗口。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/414e1a96-0bfb-4431-b79b-c2aa5ed3e382) [屋顶](https://wiki.freecad.org/Arch_Roof): 从选定的电线创建一个倾斜的屋顶。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/fe05dc43-d283-4089-b661-02573b78a0f3) [轴工具](https://wiki.freecad.org/Arch_CompAxis)
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/ed535cd9-394d-450e-bc40-d29735b916c7) [轴](https://wiki.freecad.org/Arch_Axis): 添加一个单向轴数组。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/e2dc2d2e-8eac-4836-8b75-3b3bb0cf7755) [轴系统](https://wiki.freecad.org/Arch_AxisSystem): 添加由多个轴组成的轴系。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/e875d21e-b63e-4d4c-8e4f-999448af4c0f) [网格](https://wiki.freecad.org/Arch_Grid): 添加一个网格状对象。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/85cf2f86-e811-4959-a82d-eeb2f9fa27c9) [剖面](https://wiki.freecad.org/Arch_SectionPlane): 添加一个剖面平面对象。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/c2c43f33-066e-47c2-a2e6-b16b589fb794) [空间](https://wiki.freecad.org/Arch_Space): 创建一个空间对象。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/41ca93e9-30e3-46c1-b04e-8725fa7a4280) [楼梯](https://wiki.freecad.org/Arch_Stairs): 创建一个楼梯对象。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/f7de9cd7-2cc5-49a2-ba4d-d9226ca1e533) [面板工具](https://wiki.freecad.org/Arch_CompPanel)
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/2d19afe9-c2de-4c63-974f-467b337aacba) [面板](https://wiki.freecad.org/Arch_Panel): 从选定的 2D 对象创建面板对象。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/ab436758-67d6-4252-bcf7-aba2789e1a72) [面板切割](https://wiki.freecad.org/Arch_Panel_Cut): 从面板创建 2D 剪切视图。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/6b5bbac7-8259-41ec-b777-f6d35ac90921) [面板表](https://wiki.freecad.org/Arch_Panel_Sheet): 创建 2D 切割工作表，包括面板切割或其他 2D 对象。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/4127b249-dc2b-4c45-bdf4-166bc1d4718c) [巢](https://wiki.freecad.org/Arch_Nest): 允许在容器形状内嵌套多个平面对象。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/b52c8c3f-a252-4e81-bccc-a53f7311b6ac) [设备](https://wiki.freecad.org/Arch_Equipment): 创建设备或家具对象。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/beb9ecf4-f8f7-49b2-a77d-fc712e538445) [框架](https://wiki.freecad.org/Arch_Frame): 从选定的布局创建框架对象。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/923652dd-bd1c-4afc-af49-df4375e50e6e) [栅栏](https://wiki.freecad.org/Arch_Fence): 从选定的柱子和路径创建一个栅栏对象。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/687689e0-09f3-477d-96c3-93124435bd9b) [桁架](https://wiki.freecad.org/Arch_Truss): 从选定的线或从零开始创建桁架。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/12a785a4-5dcb-4968-bb91-90b72674fcf7) [配置文件](https://wiki.freecad.org/Arch_Profile): 创建参数化 2D 轮廓。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/9adefc62-a022-457c-ac92-5ac4a466bb50) [材料工具](https://wiki.freecad.org/Arch_CompSetMaterial)
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/3d07ff7d-a85b-4b40-8c5a-f77ba1b85b25) [材料](https://wiki.freecad.org/Arch_SetMaterial): 创建一个材质并将其属性赋予选定的对象(如果有的话)。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/343230c0-9a3a-4d6c-8bc8-b13787dfed64) [多材料](https://wiki.freecad.org/Arch_MultiMaterial): 创建一个多材质，并将其属性为选定的对象(如果有的话)。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/ef2ec9bd-b09d-4246-acc4-9174d0360794) [时间表](https://wiki.freecad.org/Arch_Schedule): 创建不同类型的时间表。
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/cf1dfae3-673b-4722-a81a-29b016bb6d31) [管工具](https://wiki.freecad.org/Arch_CompPipe)
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/c5095881-fd60-4a43-ac0e-045e38423628) [管](https://wiki.freecad.org/Arch_Pipe): 创建管道。
  - ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/b46c8b14-93cc-4d09-986c-51c98f67f72d) [连接器](https://wiki.freecad.org/Arch_PipeConnector): 在 2 或 3 个选定管道之间创建角连接或 t 型连接。

### 修改工具

这些工具用于修改体系结构对象。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/1ef623ef-31da-4f8c-b0eb-c9ea0c58e887) [平面切割](https://wiki.freecad.org/Arch_CutPlane): Cuts an object according to a plane.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/8be77f60-f71b-4733-a783-21fe26b72e51) [用绳子割断](https://wiki.freecad.org/Arch_CutLine): Cuts an object according to a line.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/c0bc4071-c2ae-477c-8031-7d7583e80854) [添加组件](https://wiki.freecad.org/Arch_Add): Adds objects to a component.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/d636d9ff-9fba-4284-8f80-d62c2e125625) [删除组件](https://wiki.freecad.org/Arch_Remove): Subtracts or removes objects from a component.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/05126f81-e9a9-4f36-937e-7bb21e679bb1) [调查](https://wiki.freecad.org/Arch_Survey): 进入或离开测量模式。

### 公用事业公司

这些是帮助您完成特定任务的附加工具。

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/d368b3f5-63f6-47ac-9ed8-747ab276654c) [组件](https://wiki.freecad.org/Arch_Component): Creates a non-parametric Arch component.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/8ac9cfd6-5b6b-450c-aa9c-3cb3132ac3ee) [克隆组件](https://wiki.freecad.org/Arch_CloneComponent): Produces Arch Components that are clones of selected Arch objects (not to be confused with [Draft Clone](https://wiki.freecad.org/Draft_Clone)).
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/85e4d866-5a2d-4adf-9ec8-f13c50ebb253) [划分网格](https://wiki.freecad.org/Arch_SplitMesh): Splits a selected mesh into separate components.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/1fc1bb06-e03d-4413-8a7f-ed82ed2bc186) [网格形状](https://wiki.freecad.org/Arch_MeshToShape): Converts a mesh into a shape, unifying coplanar faces.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/5ea41fc3-fe0d-45be-9588-90c9b99bd322) [选择非流形网格](https://wiki.freecad.org/Arch_SelectNonSolidMeshes): Selects all non-manifold meshes from the current selection or from the document.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/9b572e4c-27c6-42e3-850b-0afed12840eb) [移除拱门的形状](https://wiki.freecad.org/Arch_RemoveShape): Turns cubic shape-based Arch object fully parametric.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/b9bd4628-ef96-404e-8075-f6cbb6a5c791) [关闭漏洞](https://wiki.freecad.org/Arch_CloseHoles): Closes holes in a selected shape-based object.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/9329ab6d-b310-45be-96b0-e59a06d868c9) [合并墙](https://wiki.freecad.org/Arch_MergeWalls): Merge two or more walls.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/a21e5526-7fc5-41ae-b423-663eba792510) [检查](https://wiki.freecad.org/Arch_Check): Check if the selected objects are solids and don't contain defects.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/742754b8-03ce-4488-8988-d8bfe5d7b45d) [切换 IFC Brep 标志](https://wiki.freecad.org/Arch_ToggleIfcBrepFlag): Forces a selected object to be exported as an [IfcFacetedBrep](http://www.buildingsmart-tech.org/ifc/IFC4/final/html/schema/ifcgeometricmodelresource/lexical/ifcfacetedbrep.htm).
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/95231af1-b0e0-4255-b313-282a7bb3d3e2) [3 网格视图](https://wiki.freecad.org/Arch_3Views): Creates top, front and side views from a mesh.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/3960a841-5886-4cf6-9d7c-658d40dac631) [创建 IFC 电子表格](https://wiki.freecad.org/Arch_IfcSpreadsheet): Creates a spreadsheet to store IFC properties of an object.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/f81df809-d1cd-4cf9-8947-65b2bf64cbcc) [切换子组件](https://wiki.freecad.org/Arch_ToggleSubs): Shows or hides the subcomponents of an Arch object.

### 首选项

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/37cbd046-c8f8-4093-880a-61d14a9dd48e) [首选项](https://wiki.freecad.org/Arch_Preferences): 对墙壁、结构、钢筋、窗户、楼梯、面板、管道、网格和轴线的默认外观的偏好。

### 文件格式

- [IFC](https://wiki.freecad.org/Arch_IFC): 行业基础类
- [DAE](https://wiki.freecad.org/Arch_DAE): Collada 网格格式
- [OBJ](https://wiki.freecad.org/Arch_OBJ): OBJ 网格格式(仅限导出)
- [JSON](https://wiki.freecad.org/Arch_JSON): JavaScript 对象表示法格式(仅限导出)
- [3DS](https://wiki.freecad.org/Arch_3DS): 3DS 格式(仅限导入)
- [SHP](https://wiki.freecad.org/Arch_SHP): GIS Shapefiles(仅限导入)

## API

Arch 模块可以通过[Arch Python API](https://wiki.freecad.org/Macros)函数在[Python](https://wiki.freecad.org/Python)脚本和[macros](docs\python-scripting\macros.md)中使用。

## 教程

- [从 Revit 迁移到 FreeCAD](https://wiki.freecad.org/Migrating_to_FreeCAD_from_Revit)
- [架构的工作流](http://yorik.uncreated.net/guestblog.php?tag=freecad): 一个 FreeCAD 如何开始在架构工作流程中占有初步地位的例子。
- [Arch 教程](https://wiki.freecad.org/Arch_tutorial) (v0.14)
- [快速浏览一下 Yorik 的博客](http://yorik.uncreated.net/guestblog.php?2012=180) (v0.13)
- [Arch 工作台的视频演示](https://www.youtube.com/watch?v=lTDOeHapv_E) (2016)
- [Arch 面板教程](https://wiki.freecad.org/Arch_panel_tutorial) (v0.15)
- [BIM 建模章节从 FreeCAD 手册](https://wiki.freecad.org/Manual:BIM_modeling)
- [从 STL 或 OBJ 导入](https://wiki.freecad.org/Import_from_STL_or_OBJ)
- [导出为 STL 或 OBJ](https://wiki.freecad.org/Export_to_STL_or_OBJ)
