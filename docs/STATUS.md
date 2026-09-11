# Review status

Revision B is a publicly viewable, unbuilt prototype snapshot. No fabrication or assembly release is approved.

## Before a prototype fabrication release

- Verify every assembler-specific rotation, pin-one/cathode orientation and placement origin. The earlier JLC preview showed timer rotation and connector position/orientation mismatches. Browser placement edits were exploratory and are not a validated CPL.
- Review USB differential routing, breakout coupling and stackup impedance. Trace length matching is insufficient.
- Review connector mechanical fit, overhang and assembly fixture requirements.
- Review component ratings, current limit, power-budget behavior and peripheral discharge/reconnect behavior against the selected BOM.
- Regenerate fabrication and placement files from the reviewed native revision; inspect the target assembler's complete preview and DFM results.

## Licensing work still unresolved

- Resolve the license of the supplier-linked SHOUHAN DIP-switch STEP model, or replace it with a newly constructed drawing-based model.
- Review provenance/licensing of the two imported, corrected `ReplugB` footprints. The manufacturer dimensions were checked, but the importer source does not by itself establish redistribution permission.
- Choose a project hardware/documentation license. Retain KiCad's library notice and applicable attribution.

## After building prototypes

Measure disconnect/reconnect timing, held-button behavior, loaded voltage drop, current limit and residual device power. Test representative USB low/full/high-speed devices and self-powered peripherals. Validate USB signal quality and protection behavior before claiming tested 480 Mbps operation or production readiness.

## Included checks

KiCad ERC and DRC/parity were rerun after copying the source into this repository. See `checks/`. The reports disclose ignored rule categories; no new suppressions were introduced for packaging.
