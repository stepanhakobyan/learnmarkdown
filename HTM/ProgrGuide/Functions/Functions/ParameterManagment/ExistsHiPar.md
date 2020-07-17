---
layout: page
title: "ExistsHiPar ֆունկցիա"
---

# ExistsHiPar ֆունկցիա

Վերադարձնում է տրված նույնականացուցիչով պարամետրի առկայության նշանը տրված ամսաթվով։ 

Վերադարձվող արժեքը տրամաբանական է։

Возвращает признак существования параметра с заданным идентификатором на указанную дату.

Возвращаемое значение логическое.


## Շարահյուսություն

```vb
ExistsHiPar(sParId, dDate, bSoftGet)
```

Բաղադրիչներն են՝

| Պարամետր | Նկարագրություն |
|--|--|
| sParId | Պարամետրի ներքին համար։ строковое выражение, определяющее идентификатор параметра |
| dDate | Սահմանում է ամսաթվի տիպ, որը ցույց է տալիս պարամերի փոփոխման ամսաթիվը։ выражение типа даты, указывающее на дату изменения параметра |
| bSoftGet |  bSoftGet = True-ի դեպում որոնումը կատարվում է վերջին առկա ամսաթվով, իսկ եթե bSoftGet = False, ապա կատարվում է հստակ որոնում ըստ նշված ամսաթվի։ логическое выражение, определяющее признак мягкого поиска параметра. Если <em>bSoftGet = </em> 	True, то проводится поиск по последней имеющейся дате, а если <em>bSoftGet = </em> 	False, то проводится точный поиск параметра по указанной дате. |




## Նկատառումներ

[Տես նաև](../../../functions.html)