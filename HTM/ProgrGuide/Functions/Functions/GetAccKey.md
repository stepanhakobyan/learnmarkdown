---
layout: page
title: "GetAccKey ֆունկցիա"
---

# GetAccKey ֆունկցիա

Բանկային հաշվի մեջ տեղադրում է ստուգիչ նիշ և վերադարձնում ստացված հաշիվը։  
Ստուգիչ նիշը տեղադրվում է հաշվի մեջ 7-րդ նիշի փոխարեն։

## Շարահյուսություն

``` vb
Function GetAccKey(ByVal cBank As String, ByVal SmallCod As String) As String
```

Բաղադրիչներն են՝

| Պարամետր | Նկարագրություն |
|--|--|
| cBank | Բանկի կոդը, որտեղ գտնվում է բանկային հաշիվը։ |
| SmallCod | Բանկային հաշիվը։ Նվազագույնը 6-անիշ տող։ |

## Օրինակ

CODE դաշտի մեջ ուղղում է ստուգիչ նիշը և հետ վերագրում։

``` vb
Doc("CODE") = GetAccKey(Param("CODBANK"), Doc("CODE"))    
```

## Նկատառումներ

[Տես նաև](../../functions.html)
