# Third-party material and licensing status

## Official KiCad libraries

Official embedded symbol definitions, the named official footprint libraries, and standard package STEP models come from the KiCad 10 installation. They are compiled by the KiCad community and distributed under CC-BY-SA 4.0 with the KiCad electronic-design exception. The retained [KiCad license notice](libraries/KiCad-LICENSE.md) explains the exception and the separate rules for redistributed library collections.

Sources: https://www.kicad.org/libraries/ and https://gitlab.com/kicad/libraries/

Official footprint copies use project-relative model paths. The `ReplugB` library is custom/imported material, not an official KiCad library, despite the generic description in the library table.

## Connector models

`models/Connector_USB.3dshapes/USB_A_Molex_48037-2200_Horizontal.step` is an original simplified, drawing-based model, not manufacturer-exact CAD. Reference: Molex 480372200 sales drawing, https://www.molex.com/content/dam/molex/molex-dot-com/products/automated/en-us/salesdrawingpdf/480/48037/480372200_sd.pdf

`models/ReplugB.3dshapes/Jingtuo_902-131A1011D10100.step` is an original simplified, drawing-based model. Supplier-linked CAD with a mismatched envelope was rejected. Reference: https://www.lcsc.com/product-detail/C2345.html

Both simplify contacts and stamped/internal details; do not assume full enclosure clearance or mating fidelity from the render alone.

## Imported DIP model and corrected footprints

`models/ReplugB.3dshapes/SHOUHAN_1.27-2P_TPPT.step` was imported from supplier-linked CAD and offset vertically to align with the board. Reference part: https://www.lcsc.com/product-detail/C7421516.html . A redistribution license has not been established. The two `ReplugB.pretty` footprints were imported and corrected against those manufacturers' drawings, including pad and drill dimensions. Their source licensing also needs review before public distribution.

The repository is publicly viewable, but these permissions remain unresolved. Inclusion does not establish a redistribution license. The assembled STEP export and render also include the imported model.

## Original design

No public license is selected yet for the original circuit, layout, documentation or drawing-based models. Public visibility does not waive third-party rights or grant an open-source license. Supplier datasheet PDFs and rejected/unused CAD are not bundled; use the source links and BOM references.
