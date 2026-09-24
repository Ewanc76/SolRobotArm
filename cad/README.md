# CAD

Printable parts, source CAD, drawings, and exports belong here.

## Suggested layout

```text
cad/
├── joints/
│   ├── shoulder/
│   ├── elbow/
│   └── wrist/
├── end-effectors/
├── electronics/
├── drawings/
└── exports/
    ├── stl/
    └── step/
```

## CAD rules for the first joint

- Keep the motor mount replaceable.
- Put radial loads through bearings, not the motor shaft.
- Provide mechanical hard stops where practical.
- Make fasteners accessible after assembly.
- Capture nut pockets so maintenance does not require three hands.
- Include wire routing and strain relief from the start.
- Mark revision identifiers on experimental prints.
- Preserve editable source files alongside exported STL/STEP files.

Do not treat the first successful print as production-ready. Record fit corrections and update the source model before duplicating parts.
