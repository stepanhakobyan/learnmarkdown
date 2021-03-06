---
layout: page
title: "LoadDoc ֆունկցիա"
---

# LoadDoc ֆունկցիա
[Հատկություններ և մեթոդներ](../../Asdoc.md)

Բեռնում է տվյալների պահոցում գոյություն ունեցող փաստաթուղթը ըստ ներքին նույնականացման համարի։

Եթե տրված ISN-ով փաստաթուղթը գույություն չունի, առաջանում է սխալ։  

## Շարահյուսություն

``` vb
Function LoadDoc(ByVal nISN As Long, _
        Optional ByVal nLockDoc As Integer = 0, _
        Optional ByVal bNotRaiseErr As Boolean = False, _
        Optional ByVal bLookInArc As Boolean = True) As AsDoc
```

Բաղադրիչներն են՝

| Պարամետր | Նկարագրություն |
|--|--|
| nISN | Բեռնվող փաստաթղթի ներքին նույնականացման համարը։ |
| nLockDoc | Տվյալների պահոցում արգելափակման (lock) միացման հայտանիշ։ 1 արժեքի դեպքում դրվում է թարմացման (update) արգելափակում։ 0 կամ 1 արժեք ընդունող։ Լռությամբ արժեքը 0: |
| bNotRaiseErr | `True` արժեքի դեպքում բեռնում է նաև ջնջված փաստաթղթերը (վիճակը 999)։ Լռությամբ արժեքը `False`՝ առաջացնում է սխալ ջնջված փաստաթղթի բեռնամ փորձի ժամանակ։ |
| bLookInArc | Արխիվացված փաստաթղթի բեռնման հայտանիշ։ `True` արժեքի դեպքում փաստաթղթի բեռնումը փորձում է կատարել նաև արխիվային տվյկալների պահոցից, եթե այնտեղ նույնպես փաստաթութը առկա չէ, առաջանում է սխալ։ |

## Նկատառումներ

[Տես նաև](../../../constructors.html)

## Օրինակ

Օրինակի մեջ կանչվում է LoadDoc ֆունկցիան, որտեղ mDoc-ը հղվում է փաստաթուղթ տիպի օբյեկտի վրա նրա բոլոր հատկություններով և մեթոդներով։  
Դիտելու ձևի ընտրված տողի համար բեռնվում է փաստաթուղթ։

``` vb
Set mDoc = LoadDoc(CurrentView.Value("fISN"))
Set xDoc = CreateDoc("HTN92", mDoc.ISN)
xDoc("CATEGORY") = xMsgType
xDoc("BMDOCNUM") = nDoc.ISN
xDoc("REFERENC") = mDoc("BMDOCNUM")
xDoc("DATE") = mDoc("BMIODATE")
xDoc("TYPE") = xMsgType
xDoc.State=0
xDoc.Show
```
