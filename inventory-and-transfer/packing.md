---
description: Materials and Artifacts can be packed in order to be transferred or sold.
---

# 📦 Packing

In order to transfer Materials and/or Artifacts, we need to Pack them. We can Pack any combination and quantity of Materials and/or Artifacts and when we send the inscription containing the Packing operation the content of it gets transferred to the new wallet (similar to BRC20)

As an outline, this is what an operation of packing would look like in a JSON format text inscription.&#x20;

{"p":"bitcraft"\
"op": "pack"\
"pack": the list of materials and/or objects we want to pack eg. \[1000M1,1A1]\
}

When Packed, items can not be used to craft or be dropped on a bitmap.\
