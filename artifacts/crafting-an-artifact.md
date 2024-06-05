---
description: >-
  Once a Spec exists and until the max limit is not reached, anybody can craft
  an Artifact
---

# 🛠️ Crafting an Artifact

Once a crafting Spec is created anybody can craft using the Spec as long as the max supply is not hit.\
\
As an outline, this is what an operation of crafting would look like in a JSON format text inscription.&#x20;

{"p":"bitcraft"\
"op":"craft"\
"code": code of the Artifact to craft\
"qty": how many copies of the Artifact to be crafted in this operation\
}

The user should have enough resources to craft the quantity requested, if he does the Artifact(s) are created and the Materials or Artifacts used to create the new Artifact(s) are detracted from the crafter's inventory. \
Max limit shouldn't be exceeded (FCFS).\
If any condition fails the entire operation fails.

Example:

{"p":"bitcraft"\
"op":"craft"\
"c": \[A1]\
"qty": "1"\
}
