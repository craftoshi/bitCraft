---
description: >-
  Materials are the basic resources needed to build. Bitcraft allows bitmap
  landlords to extract resources from their land.
---

# 🪵 Discovering Materials

Material discovery follows the principles of DMT/NAT paradigm and theory, but is implemented in a slightly different way. Anybody can discover a material, using patterns that are intrinsic to the blockchain data of Bitcoin.

At first, the framework includes block data, but in the future in can be extended to transaction and UTXO data, which might be interpreted as more atomicals layer of matter, such as atoms and particles.&#x20;

\
As an outline, this is what an operation of discovery would look like in a JSON format text inscription:

{"p": "bitcraft"\
"op": "discover"\
"name": name of the material\
"pattern": field or pattern in the block data used to calculate the Material in each bitmap\
"desc": a description can be given to the material to suggest how it should be used\
"code": code, the material code has to be a string starting with M and whole numbers following (e.g. M1), if not specified, the first available code is assigned starting from M0, max. length 16 digits\
}\


A combination of pattern and field can not be used twice to create different materials (each material is unique), the code should also be unique and never used before.&#x20;

If any of the conditions is not met the operation fails.\
\
Example:\
{"p":"bitcraft"\
"op":"discover"\
"name": "WOOD"\
"pattern": "total\_size"\
"desc": "What wood you do with it?"\
"code": "M1"\
}\
\
{"p":"bitcraft"\
"op":"discover"\
"name": "WEED"\
"pattern": "420.total\_size"\
"desc": "Take it easy."\
"code": "M420"\
}

Optionally, the discovery inscription could be done as a child inscription of an image in order to give it a logo. \
