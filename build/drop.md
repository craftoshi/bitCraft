---
description: Now we have a land and objects created from its resources, let's build!
---

# 🏗️ Drop

Now that we have all the ingredients we need, we can build the actual metaverse in a way that is defined on-chain.

An Artifact can be placed inside a bitmap or a specific parcel that we own.\
As an outline, this is what an operation of dropping an Artifact would look like in a JSON format text inscription. It should be inscribed as a child inscription of the bitmap or parcel.

{"p":"bitcraft"\
"op": "drop"\
"code": the code of the Artifact or Material to be dropped \
"coord": the parcel of the district to drop it on in the format parcel.district.bitmap\
"qty": the quantity to be dropped \
}

When an asset is dropped on a bitmap, it "travels" with it. If the bitmap (or parcel) is transferred or sold, the Material or Artifact also gets transferred with it. This allows creators to build entire spaces or experiences on a specific bitmap and then sell or transfer the whole bitmap and everything that's on it at once.

Example:

{"p":"bitcraft"\
"op": "drop"\
"code": "A1"\
"coord": "1.420690.bitmap"\
"qty": the quantity to be dropped \
}

When an Artifact is dropped on a bitmap, it doesn't appear anymore in the Inventory of the crafter.

As what we are utilizing is block data, this first outline considers deploying on a parcel only as a spatial coordinate of where the object should appear when visualizing the whole district. A set of rules should be implemented on how to deploy on detached parcels or bitmaps that "miss" some parcels.
