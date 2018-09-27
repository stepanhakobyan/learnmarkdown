﻿<html>
<head>
<title>Константы типов курсоров</title>
</head>

<body>

<p><font face="Arial"><big>Константы типов курсоров</big></font></p>

<p><font face="Arial">Т.к. эти константы объявлены в системном ядре, 
то нет необходимости в их дополнительном объявлении. Их можно использовать везде 
в скриптах, взамен их значений.</font></p>

<table border="1">
  <tr>
    <td width="15%"><font size="3" face="Arial"><b>Константа</b></font></td>
    <td width="15%"><font size="3" face="Arial"><b>Значение</b></font></td>
    <td width="70%"><font size="3" face="Arial"><b>Описание</b></font></td>
  </tr>
  <tr>
    <td width="15%"><font face="Arial"><strong>ASOpenForwardOnly</strong></font></td>
    <td width="15%"><font face="Arial"><strong>0</strong></font></td>
    <td width="70%"><font face="Arial">по умолчанию, открывает курсор 
	типа forward-only. Это значит, что поиск по строкам курсора может 
	производиться&nbsp; только от начала курсора к концу; текущая позиция строки не 
	может быть перемещена назад, к первой строке, и в каждый момент времени 
	доступна только одна строка. Данный тип курсора удобен для быстрого поиска и 
	обработки данных.</font></td>
  </tr>
  <tr>
    <td width="15%"><font face="Arial"><strong>ASOpenKeyset</strong></font></td>
    <td width="15%"><font face="Arial"><strong>1</strong></font></td>
    <td width="70%"><font face="Arial">открывает курсор типа keyset. 
	Результат запроса может содержать обновляемые строчки, которые можно 
	изменять, &nbsp; удалять, добавлять новые. Передвижение маркера в курсоре не 
	ограничено. Курсор может содержать колонки из различных таблиц и их членство 
	в курсоре фиксировано.</font></td>
  </tr>
  <tr>
    <td width="15%"><font face="Arial"><strong>ASOpenDynamic</strong></font></td>
    <td width="15%"><font face="Arial"><strong>2</strong></font></td>
    <td width="70%"><font face="Arial">открывает курсор типа dynamic. 
	Результат запроса может содержать обновляемые строчки, которые можно 
	изменять, &nbsp; удалять, добавлять новые. Передвижение маркера в курсоре не 
	ограничено. Курсор может содержать колонки из различных таблиц и их членство 
	в курсоре не фиксировано.</font></td>
  </tr>
  <tr>
    <td width="15%"><font face="Arial"><strong>ASOpenStatic</strong></font></td>
    <td width="15%"><font face="Arial"><strong>3</strong></font></td>
    <td width="70%"><font face="Arial">открывает курсор типа static. 
	Порядок сортировки, значения, число колонок в курсоре фиксировано. 
	Обновленные со стороны других пользователей строчки сразу не отражаются в 
	открытом курсоре данного типа. Для обновления нужно его закрыть и открыть 
	еще раз.</font></td>
  </tr>
</table>

<blockquote>
</blockquote>

<p><font face="Arial"><br>
Эти константы могут быть также использованы в качестве параметров метода <a
href="../Functions/ASDATA/OpenCursor.html">OpenCursor</a> источника данных, для 
определения вида открываемого курсора данных.</font></p>
</body>
</html>