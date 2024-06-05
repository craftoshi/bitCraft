---
description: Not all Artifacts can be hosted on any bitmap
---

# ⛓️ Non-Arbitrary Constraints (Proportionality)

To encourage standardization and the development of an economy based on non-arbitrary constraints, the concept of Proportionality is introduced.

Materials will not only be used to craft Artifacts, but also to determine the space inside a bitmap and its compatibility with Artifacts. The supply of a Material in a bitmap determines how much an object made from that material occupies in terms of percentage of the land, regardless of the state of extraction of the Material.

\
For example, on a bitmap that has a supply of 400000 WOOD, the TABLE A1 should occupy 1/40 of the available space, or 2.5%. If a bitmap has a supply of WOOD lower than 10000, the Artifact A1 can not be deployed on that bitmap.

If an Artifact is crafted using more than one Material, both material relative percentages are averaged in calculating how much space they occupy on the bitmap.&#x20;

In addition to specific material constraints, a total space constraint is to be considered. In the first example, the bitmap would still have 97.5% of available space. Let's consider a second material STONE M2 that is present on the bitmap with a supply of 100. If an object made from 50 STONE is deployed on this same bitmap, the occupied space would now be 52.5%. Even though we theoretically still have WOOD space, we couldn't deploy another object made of 300000 WOOD because the Total Space is occupied by the object made of STONE.

These constraints allow Material Engineering to take place, because the Materials and proportions between them used in the Spec will determine their dimensions in the 3D space. So Materials that are relatively well distributed can be used to give similar proportions on different bitmaps, while Artifacts made from rare Materials could be considered as more valuable but could only be deplpyed on bitmaps that have that Material in the first place. This adds a layer of differentiation between bitmaps based on different value propositions.
