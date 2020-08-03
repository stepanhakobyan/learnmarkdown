---
layout: page
title: "CutParentLink ֆունկցիա"
---

# CutParentLink ֆունկցիա

Для указанного документа разрывает связь с родителем.

## Շարահյուսություն

```vb
CutParentLink (nISN, [nParentISN])
```
Բաղադրիչներն են՝
    
| Պարամետր | Նկարագրություն |
|--|--|
| nISN | Փաստաթղթի ներքին նույնականացման համար, որի համար խզվում է կապը ծնողի հետ։ численное выражение типа Long, определяющее ISN документа, для которого разрывается связь с родителем. |
| nParentISN | Կապը խզած ծնողի ներքին նույնականացման համար։ Եթե պարամետրը առկա չի, ապա կապը խզվում է բոլոր առկա ծնողների հետ հետ։ необязательное численное выражение типа Long, определяющее ISN родительского документа, с которым разрывается связь. Если параметр опущен, то разрываются связи со всеми существующими родителями. |

## Շարահյուսություն

[DOCP](../../../Database/DocP.html) աղյուսակի մեջից ջնջվում է տվյալ փաստաթղթին համապատասխան տողը։

Из таблицы [DOCP](../../../Database/DocP.html) удаляется строка, соответствующая данному документу.

[Տես նաև](MakeParentLink.md)