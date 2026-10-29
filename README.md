# computers-delivery-schema

The JSON Schema of the delivery JSON of the practical exercises of Computers (URV): the
`comp_XX-progY-phaseM-callT.json` file each student delivers.

Deliveries reference it with their `$schema` key, so that the editors that support it (e.g. VS Code or the JetBrains
IDEs) show their errors while filling them in:

```json
{
  "$schema": "https://raw.githubusercontent.com/URV-teacher/computers-delivery-schema/master/computers-urv-delivery-schema-1.0.json",
  ...
}
```

The schema is versioned by its filename: a released version is never changed in a way that breaks the deliveries that
reference it, a new version is added as a new file instead (e.g. `computers-urv-delivery-schema-1.1.json`).

Used by [tot](https://github.com/URV-teacher/tot), which validates the deliveries against it and writes their template.
