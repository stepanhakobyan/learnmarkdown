﻿<html>
<head>
<title>Системное событие GridValid</title>
</head>

<body>

<p><strong><font size="4" face="Arial">Событие GridValid<br>
<br>
</font></strong><font face="Arial"><a href="../scriptstproced.html">См. 
также</a>&nbsp; <a href="../Examples/E_GridValid.html">Пример</a>&nbsp; <a
href="../Defs/doc.html">Применяется к</a></font></p>

<p class="label"><font face="Arial">Активизируется при попытке выхода 
из грид-таблицы в документе. Служит для проверки введенных значений на 
соответствие некоторому условию. <br>
Последовательность генерации системных событий приведена здесь <a href="Events_Sequence.html"><img
src="../../../IMAGES/More.gif" width="12" height="12" alt="More.gif (304 bytes)"
border="0"></a>.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial">Sub <strong>GridValid</strong>(<strong>ByVal 
GridObj</strong>)<br>
&nbsp;&nbsp; <strong>Select Case</strong> <em>GridObj</em>.<a
href="../Functions/ASDOC/AsGrid/Name.html">Name</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>Case</strong> <em>Grid1</em><br>
<em>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; statements1</em><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>Case</strong> <em>Grid2</em><br>
<em>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; statements2</em><br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; . . . . .<br>
</strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>Case</strong> <em>GridN</em><br>
<em>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; statementsN</em><br>
<strong>&nbsp;&nbsp;&nbsp; End Select&nbsp; </strong>&nbsp;&nbsp; <br>
End Sub</font></p>

<p>&nbsp;</p>

<p><font face="Arial">Синтаксис события <strong>GridValid</strong>
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>GridN</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее идентификатор грида в документе. </font></td>
  </tr>
</table>

<p>&nbsp;</p>

<p class="label"><font face="Arial"><b>Примечание<br>
</b><br>
В общем случае в одном документе могут быть несколько грид-таблиц. Для этого в 
обработчике события <strong>GridValid</strong> удобно организовать условие 
выбора в зависимости от <a href="../Defs/doc.html">идентификатора грид-таблицы</a>.<br>
Идентификатор грида передается 
с верхнем регистре (<span lang="en-us">UCASE</span>)<span lang="en-us">.</span></font></p>
</body>
</html>