---
description: >-
  To create an Artifact, a Spec needs to be created which determines the
  properties of the Artifact.
---

# 🔎 Creating a Spec

To create a Spec that defines the properties of an object, we have to first take an inscription as reference. The most common type of reference inscription should be 3D models, but in theory any file can be used as a reference for the spec.

As an outline, this is what the operation of creating a Spec would look like in a JSON format text inscription. The inscription should be made as a child inscription of the reference inscription (3D model or anything we want the object to be).

{"p":"bitcraft"\
"op": "spec"\
"name": name of the object\
"code": code, should start with A followed by integers (e.g. A1), if not specified the first available code is assigned starting from A0, digit limit 16\
"spec": the list of materials and/or artifacts needed to craft this object. eg. \[1000M1,1000M420]\
"ref": the id of the inscription used as reference \
"max": how many Artifacts can be created with this Spec in total\
"qty": how many Artifacts to self-craft in the Spec operation\
}

If qty>0 the crafter should have enough resources to craft the quantity requested, if he does the Artifact is created and the Materials or Artifacts used to create the new Artifacts are detracted from the crafter's inventory. \
Materials and Artifacts must have been Discovered or Crafted before when included in a Spec.\
Materials can be decimals, Objects must be integers.\
Max limit shouldn't be exceeded (FCFS).\
An inscription can only be used as reference once (nothing stops people to create "fake" versions of the same artifact without the provenance).\
If any condition fails the entire operation fails and no Materials or Artifacts are affected.

Example:

{"p":"bitcraft"\
"op": "spec"\
"name": "TABLE"\
"code": "A1"\
"spec": "\[10000M1]"\
"ref": "INSERT INSCRIPTION ID HERE" \
"max": "100000"\
"qty": 1\
}\


Example using another Artifact in the Spec:

{"p":"bitcraft"\
"op": "spec"\
"name": "STRONG\_TABLE"\
"code": "A1"\
"spec": "\[1A1,5000M1]"\
"ref": "INSERT INSCRIPTION ID HERE" \
"max": "100"\
"qty": 1\
}\
