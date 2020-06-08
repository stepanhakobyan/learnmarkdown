---
layout: page
title: "LoadDocFromFolder ֆունկցիա"
---

# LoadDocFromFolder ֆունկցիա
[Հատկություններ և մեթոդներ](../../Asdoc.md)

Բեռնում է փաստաթուղթը ըստ թղթապանակի և բանալու։

Տրված ներքին նույնականացման համարով կամ բանալիով թղթապանակի բացակայության դեպքում վերադառնում է Nothing։

## Շարահյուսություն

``` vb
Set sDoc = LoadDocFromFolder(FolderId, Key)
```

Բաղադրիչներն են՝

| Պարամետր | Նկարագրություն |
|--|--|
| sDoc | Բեռնված փաստաթղթի հղում։ |
| FolderId | Թղթապանակի ներքին անուն։ |
| Key | Թղթապանակի տարրի բանալին։ |

## Նկատառումներ

[Տես նաև](../../../constructors.html)

## Օրինակ 

Օրինակի մեջ կանչվում է LoadDocFromFolder ֆունկցիան, որտեղ mDoc-ը հղվում է փաստաթուղթ տիպի օբյեկտի վրա նրա բոլոր հատկություններով և մեթոդներով։
ACCCRLN թղթապանակից բեռնվում է փաստաթուղթ doc("CODE") բանալիով։

``` vb
Set mDoc = LoadDocFromFolder("ACCCRLN", doc("CODE"))
```