# Node systems and controls

The saved Blender scene is the project source. It renders independently of the Python tools used to author it.

## Structure

Select **Cavern | continuous vaulted shell**. Its main modifier uses **NV2 | Sunken cathedral**.

| System | Purpose |
|---|---|
| NV2 chamber, bank and retained-rock fields | Continuous cavern mass and major openings |
| NV6 / NV10 foreground geology | Larger structural fractures and ledges |
| NV12 &#124; Left foreground fractured faces | Eight shallow angular cuts into the existing structural mass |
| NV5 &#124; Secondary rock finish | Surface geometry, local joints and smaller strata |
| NV13 &#124; Fractured bedding and edge chips | Shared system for interrupted smaller layers and chipped margins |
| NV13 &#124; Right framing cliff region | Localizes the right-side treatment and protects the shoreline |

Inside **NV5 | Secondary rock finish**, use **Left fractured strata and chips** and **Right fractured strata and chips**. Their controls include layer thickness, width, inclination, relief, chip depth, projection direction and seed. The two sides use different settings. The relief deforms the connected rock; it does not scatter separate slabs over it.

The `NV13_layer_relief` point attribute records the smaller fracture pattern for shading. `NV12_open_fractures` records the earlier local joints, and `NV12_geology_patch` controls the reduction of older bump within the refined regions.

## Mineral growth

The roof-mineral collection contains the drapery and flowstone hosts. Local refined fringes use **NV12 | Thin rooted mineral fringe** and **NV12 | Fine asymmetric mineral pendant**. Other approved arch and wall formations retain their earlier NV8 / NV9 systems.

Controls include placement, curtain depth, fold width, tip count, length, variation, seed, attachment reach and detail quality. Roots raycast to the actual bedrock; tips share their curtain edge. `NV11_distance_to_bedrock` blends mineral contact shading into the supporting rock.

## Materials

- **NV2 | Fractured wet limestone** mixes rough charcoal host rock, earthy iron-bearing faces, crystalline calcite, localized wet films and rough fracture interiors.
- **NV10 | Mineral curtains and flowstone** gives deposits their own response, with host-coloured roots.
- **NV11 | Geological colour and moisture fields** supplies coherent world-space material masks.

Colour and roughness have procedural variation; the geometric fracture attributes also influence the material. Avoid increasing bump to compensate for missing larger forms.

## Look development

The camera and major cavern openings are established. The current stage focuses on the foreground rock hierarchy. Inspect both neutral clay and scene lighting before extending detail further. The saved render settings retain the final target, so lower resolution and samples for working previews.

Useful embedded text blocks include **REPOSITORY | Start here**, **NV12 | Left foreground study**, and **NV11 | Surface controls**. Older embedded breakdowns and packed images document previous stages and may predate NV13.
