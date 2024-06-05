---
description: Once a Material is discovered, anybody can extract it from their bitmaps.
---

# 🪓 Extracting materials

Anybody can extract a discovered material from a bitmap they own. The material can only be extracted once. Provenance is necessary to extract materials from a bitmap.&#x20;

As an outline, this is what an operation of extraction would look like in a JSON format text inscription. The inscription should be made as a child inscription of the bitmap.

{"p":"bitcraft"\
"op":"extract"\
"code": the code of the desired material to extract\
}

Each material can only be extracted once from each bitmap. The extraction operation extracts the whole available supply of the material in the bitmap.&#x20;

Example:\
{"p":"bitcraft"\
"op":"extract"\
"code": "M1"\
}

Using this method, when looking at the child inscriptions of any particular bitmap, the state of extraction of all different materials can easily be confirmed.

\
