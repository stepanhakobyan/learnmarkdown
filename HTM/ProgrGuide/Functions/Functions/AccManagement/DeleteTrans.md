---
layout: page
title: "DeleteTrans ֆունկցիա"
---

# DeleteTrans ֆունկցիա

[HI](../../../Database/Hi.html) աղյուսակից ջնջում է գործառույթային գործարքը նշված փաստաթղթի համար։ 

Ջնջելու ժամանակ գեներացվում է հաշվառման [OnDelete](../../../ScriptProcs/OnDelete.md) համակարգային իրադարձությունը, ճշգրտվում են մնացորդները և հետո ստուգվում են հաշվառում օբյեկտի և կուտակող օբյեկտի սահմանափակումները։ 

Սահմանափակումները ստուգելու ժամանակ կարող է սխալ գեներացվել, և կատարված գործողությունների հետխաղացման համար հարկավոր է բացել տրանզակցիա [BeginTrans-ով](../TransactionManagment/BeginTrans.html) մինչև `DeleteTrans` ֆունկցիայի կանչը, իսկ հետո ավարտել տրանզակցիան [CommitTrans-ով](../TransactionManagment/CommitTrans.html)։

Եթե `DeleteHI2Trans`-ի կանչը կատարվել է [Action](../../../ScriptProcs/Action.md) համակարգային իրադարձության մշակիչում, ապա սահմանաչափերի ստուգումը կատարվում է իրադարձության ավարտից հետո։ Այլ դեպքերում սահմանաչափերի ստուգումը կատարվում է ֆունկցիայի ներսում։

## Շարահյուսություն

``` vb
Sub DeleteTrans(ByVal IsnOrDoc As Variant, _
                ByVal Trans As Long, _
       Optional ByVal sType As String)
```
Բաղադրիչներն են՝


| Պարամետր | Նկարագրություն |
|--|--|
| IsnOrDoc | Ջնջվող գործարքի հաշվառող փաստաթղթի ներքին նույնականացման համարը կամ օբյեկտը։ |
| Trans | Ջնջվող գործարքի համարը։ |
| sType | Հեռացվող հաշվառման տեսակը։ |

## Նկատառումներ

[Տես նաև](../TransactionManagment/InTrans.html)