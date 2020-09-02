---
layout: page
title: "Split ֆունկցիա"
---

## Split ֆունկցիա

Վերադարձնում է միակողմանի մասիվը, որը պարունակում է նշված քանակի ենթատողեր։ Նշված տողը բաժանվում է ենթատողերի ըստ նշված բաժանարարի։
Возвращает одномерный массив, содержащий указанное количество подстрок. Заданная строка разбивается на подстроки по заданному разделителю.


## Շարահյուսություն

```vb
Split (sExpression, [sDelimiter, [nCount, [Compare]]])
```

Բաղադրիչներն են՝


| Պարամետր | Նկարագրություն |
|--|--|
| sExpression | Սահմանում է հիմնական տող, որը բաղկացած է բառերից և բաժանարարներից։ Եթե տվյալ արգումենտը համարվում է դատարկ տող (""), ֆունկցիան վերադարձնում է առանց տարրերի դատարկ մասիվ։ строковое выражение, определяющее исходную строку, состоящую из слов и разделителей. Если данным аргументом является пустая строка (&quot;&quot;), функция возвращает пустой массив без элементов. |
| sDelimiter | Սահմանում է տողի մեջ բաժանարարի նշանը։ Այն սահմանում է ենթատողերի սահմանները։ Լռությամբ որպես բաժանարարի  նշան կչիրառվում է բացակը " "։ Եթե բածանարարը համարվում է դատարկ տողը (""), ապա ֆունկցիան վերադարձնում է ամբողջ տողը, մասիվի մեկ տարրի մեջ։   необязательное строковое выражение, определяющее символ разделителя в строке. Она определяет границы подстрок. По умолчанию в качестве разделителя принимается значение &quot; &quot; пробел. Если разделителем является пустая строка (&quot;&quot;), то функция возвращает целиком всю строку, в одном элементе массива. |
| nCount | Վերադարձվող ենթատողերի քանակ։ Լռությամբ ստանում է -1 արժեք, որը ցույց է տալիս, որ վերադառնում են բոլոր առկա ենթատողերը։ необязательное численное выражение, определяющее количество возвращаемых подстрок. По умолчанию это (-1), указывающий что возвращаются все существующие подстроки. |
| Compare | необязательное численное выражение, указывающее на вид сравнения при получении подстрок. |



## Նկատառումներ

`Compare` արգումենտը ստանում է հետևյալ արժեքները։
Аргумент <em>Compare</em> принимает следующие значения:


| Հաստատուն | Արժեք | Նկարագրություն |
|--|--|--|
| vbUseCompareOption | -1 | Համեմատություն է անցկացնում ըստ Option Compare տեղադրման/սահմանման։ Производит сравнение в соответствии с установкой Option Compare. |
| vbBinaryCompare | 0 | Լռությամբ արժեք։ Անցկացվում է երկուական համեմատություն։ Значение по умолчанию. Производится бинарное сравнение. |
| vbTextCompare | 1 | Անցկացվում է տեքստային համեմատություն։ Производится текстовое сравнение. |
| vbDatabaseCompare | 2 | Կիրառվում է Microsoft Access-ի սյունակների։ Անցկացվում է համեմատություն տվյալների պահոցի մեջ պահպանվող  տեղեկության պահպանման հիմքի վրա։ Применяется для таблиц Microsoft Access. Производит сравнение на основе хранящейся информации в базе данных. |


## Նկատառումներ

[Տես նաև](Join.md)