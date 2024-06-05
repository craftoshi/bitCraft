---
description: Artifacts can be Recycled to recover the components used to Craft it.
---

# ♻️ Recycling an Artifact

An Artifact can be dismantled to Recycle the Artifacts and Materials used to craft it. \
When an Artifact is Recycled the crafter recovers all the Artifacts used to create it in their entirety, and 50% of the Materials used.

As an outline, this is what an operation of recycling would look like in a JSON format text inscription.&#x20;

{"p":"bitcraft"\
"op":"recycle"\
"code": code of the Artifact to recycle\
"qty": the quantity to be recycled\
}\
\
The crafter should have the quantity requested available in their Inventory.\
When an Artifact is Recycled, it is essentially burned as it does not get deducted from the crafted supply of its relative Spec. \


Example:\
{"p":"bitcraft"\
"op":"recycle"\
"c": "A1"\
"qty": "1"\
}
