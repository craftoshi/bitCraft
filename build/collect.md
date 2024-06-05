---
description: Artifacts deployed on a bitmap can be recollected
---

# 🧚‍♂️ Collect

A land owner can collect any Artifact that is attached to one of their bitmaps.

As an outline, this is what an operation of collecting an Artifact would look like in a JSON format text inscription. It should be inscribed as a child inscription of the bitmap or parcel.

{"p":"bitcraft"\
"op": "collect"\
"code": the code of the Artifact or Material to be collected \
"coord": the parcel to collect it from in the format parcel.district.bitmap\
"qty": the quantity to be collected \
}

If an item is collected from a parcel it gets added to the inventory of the crafter.\


Example:

\
{"p":"bitcraft"\
"op": "collect"\
"code": "A1"\
"coord": "1.420690.bitmap"\
"qty": the quantity to be collected \
}
