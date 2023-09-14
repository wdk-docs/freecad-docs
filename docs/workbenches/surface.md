# 表面工作台

## 介绍

![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/97a67f8d-39f6-42cc-925c-76b2e7c841ca) **表面工作台**提供了创建和修改简单的[NURBS 曲面](https://en.wikipedia.org/wiki/Non-uniform_rational_B-spline)的工具。当使用**Face from edges**选项时，这些工具具有类似于![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/39ab694b-29be-4607-a170-b2905efa6e6b) [零件构建器](https://wiki.freecad.org/Part_Builder)工具的功能。然而，与该工具不同的是，Surface Workbench 的工具是参数化的，并提供了额外的选项。在这方面，本工作台中的工具类似于![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/f1ad8001-04b6-4496-984f-c6fe597c8603) [零件设计增材阁楼](https://wiki.freecad.org/PartDesign_AdditiveLoft)和![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/479f50c0-96be-45f1-a110-f4cb158e2080) [零件设计](https://wiki.freecad.org/PartDesign_AdditivePipe)。

Some of the features provided are:

- Creation of surfaces from boundary edges.
- Alignment of the curvature from neighboring faces.
- Constraining of surfaces to additional curves and vertices.
- Extension of faces.
- A mesh can be used as a template to create spline curves on its surface.

![Surface workbench icon](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/ba8681df-5f3f-4772-9b81-f458b612593a)  
_Surface workbench icon_

![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/d00b5223-0dcb-4db8-8b0c-bb2420121174)

## Usage

The Surface Workbench intends to create faces with shapes, which is not possible to do with the standard tools in other workbenches.

![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/90bf3d6e-9684-4c6e-aaca-9bd19f72a969)  
_Surface created with sketches placed in datum planes with the tools of the [PartDesign Workbench](docs\workbenches\part-design.md)_

The Surface Workbench integrates with other workbenches of FreeCAD. The above example was created from ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/d43eb877-0534-4d14-a82f-2a995ed0be1b) [Sketches](https://wiki.freecad.org/Sketch) placed on ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/f0771a36-d2d9-4227-b9b8-88d2d5921dca) [PartDesign Datum planes](https://wiki.freecad.org/PartDesign_Plane) in the ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/3fd990e9-04a9-4adb-8458-fcc12d764b38) [PartDesign Workbench](docs\workbenches\part-design.md). The design can be fully parametric if all datum planes and sketches are defined accordingly. In most cases it is sufficient to draw a closed sketch to define the boundary of a face, and then use different options to further modify its shape.

The generated surface cannot be placed inside a ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/6a0d4b48-9ea5-407d-9cff-66b68b65fece) [PartDesign Body](https://wiki.freecad.org/PartDesign_Body). However, the generated surface can be contained inside a ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/fb4ab93e-494f-429c-81db-058a26e2af59) [Std Part](https://wiki.freecad.org/Std_Part) together with the associated ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/3d2ec5ec-3984-463d-b05b-4357c4d839a1) [PartDesign Body](https://wiki.freecad.org/PartDesign_Body) that holds the datum planes and sketches. The non-parametric ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/157725f8-701f-4969-964e-888cd390b47f) [Part Builder](https://wiki.freecad.org/Part_Builder) tool can then be used in order to create a [shell](https://wiki.freecad.org/Glossary#Shell) and finally a [solid](https://wiki.freecad.org/Glossary#Solid).

## Tools

- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/b662c9a2-1732-46eb-bcab-9adf8eec581e) [Filling](https://wiki.freecad.org/Surface_Filling): fills a series of boundary curves with a surface.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/3826e1ce-eb13-40e2-98b0-235b7f582eb8) [Fill boundary curves](https://wiki.freecad.org/Surface_GeomFillSurface): creates a surface from two, three or four boundary edges.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/a4a699a0-0548-44e9-beee-135d1ceddc3b) [Sections](https://wiki.freecad.org/Surface_Sections): creates a surface from edges that represent transversal sections of surface.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/569debe1-d7e8-4bc0-ab7f-b318047faf39) [Extend face](https://wiki.freecad.org/Surface_ExtendFace): extrapolates the surface at the boundaries with its local U parameter and V parameter.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/dff66f82-6816-41a5-a172-dc5fd11e2263) [Curve on mesh](https://wiki.freecad.org/Surface_CurveOnMesh): creates approximated spline segments on top of a selected mesh.
- ![image](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus/assets/100439627/ede8a53b-79e8-4670-840e-16430d8bef01) [Blend Curve](https://wiki.freecad.org/Surface_BlendCurve): creates a Bezier curve between two edges, with desired continuity.
