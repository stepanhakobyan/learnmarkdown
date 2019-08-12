---
layout: page
title: "AsCallBackOnTimer/Label"
---


# Label հատկություն

[См. также](../AsCallBackOnTimer.md) [Օրինակ](../../Examples/E_AsCallBackOnTimer.html) [Применяется к](../AsCallBackOnTimer.md) 

Վերադարձնում կամ նշանակում է օբյեկտի կողմից կատարած աշխատանքների ընթացիկ վիճակի նկարագրությունը։

Այս հատկությունը հարկավոր է փոխել ֆունկցիայի հերթական ավտոմատ կանչից հետո։  
Այսինքն, եթե հերթական քայլից հետո արժեքն է՝

``` 
Մշակված տողերի քանակ - 500
Բարեհաջող մշակված - 497
Սխալների քանակ - 3
```
Ապա հաջորդ քայլից հետո կարող է դառնալ 
``` 
Մշակված տողերի քանակ - 520
Բարեհաջող մշակված - 416
Սխալների քանակ - 4
```

## Շարահյուսություն

``` vb
object.Label = [sValue]
```
Բաղադրիչներն են՝


| Պարամետր | Նկարագրություն |
|--|--|
| object | Ժամաչափով պարբերաբար ֆունկցիա աշխատացնեղ օբյեկտի հղում։|
| sValue  | Նոր արժեք։ |

## Նկատառումներ 
Հատկության նախնական արժեքը է հարկավոր տալ [Show](Show.md) կանչից առաջ, որպեսզի որոշվի պատուհանի վրա վիճակի ցույց տալու համար նախատեսվող տեղի չափը։

Հատկությանը հարկավոր է տալ 1 մեկ կամ մի քանի տողանոց արժեք։
``` vb
callback.Label = "Մշակված տողերի քանակ - " & CStr(allCount) & vbCrLf _
                 "Բարեհաջող մշակված - " & CStr(processedCount) & vbCrLf _
                 "Սխալների քանակ - " & CStr(errorCount)
```


## Տվյալի տիպ

Տող