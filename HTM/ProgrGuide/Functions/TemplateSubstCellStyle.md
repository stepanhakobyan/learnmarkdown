---
layout: page
title: "TemplateSubstCellStyle օբյեկտ"
---

## TemplateSubstCellStyle օբյեկտ

Օբյեկտը նախատեսված է `xlsx` տիպի տպելու ձևի ձևանմուշի աղյուսակի վանդակների ձևաչափի նկարագրության համար։

Объект <strong>TemplateSubstCellStyle</strong> предназначен для описания форматов ячеек таблицы шаблона печати типа <strong>.xlsx</strong>.


| Հատկություններ | Նկարագրություն |
|--|--|
| [BackColor](TemplateSubstCellStyle/BackColor.md) | Վերադարձնում կամ նշանակում է վանդակի տոնային գույնը։ Возвращает или устанавливает фоновый цвет ячейки. |
| [Bold](TemplateSubstCellStyle/Bold.md) | Վերադարձնում կամ նշանակում է վանդակի տառաչափի  թավությունը։ <p>Возвращает или устанавливает жирность шрифта ячейки. </p> |
| [Color](TemplateSubstCellStyle/Color.md) | Վերադարձնում կամ նշանակում է վանդակի տառաչափի գույնը։ <p>Возвращает или устанавливает цвет шрифта ячейки.</p> |
| [Italic](TemplateSubstCellStyle/Italic.md) | Վերադարձնում կամ նշանակում է վանդակի տառաչափ շեղակի ընդգծումը։   <p>Возвращает или устанавливает курсивное начертание шрифта ячейки.</p> |
| [Underline](TemplateSubstCellStyle/Underline.md) | Վերադարձնում կամ նշանակում է վանդակի տառաչափ ընդգծումը։ <p>Возвращает или устанавливает подчеркиваемость шрифта ячейки.</p> |



## Նկատառումներ

Ձևաչափերի նկարագրությունից հետո, մինչև տարրերի արժեների լրացնելը, [UseStyles](TemplateSubstitution/UseStyles.html) հատկությանը հարկավոր է տալ True արժեք։

После описания форматов, перед заполнением значений элементов, необходимо задать свойству [UseStyles](TemplateSubstitution/UseStyles.html) значение True.