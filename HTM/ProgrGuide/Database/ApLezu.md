﻿<html>
<head>
<title>Таблица APLEZU</title>
</head>

<body>

<h1><font size="4" face="Arial">Таблица APLEZU</font></h1>

<p><font face="Arial">Таблицa описания констант для подстановки в 
переменные.<br>
</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="20%"><font face="Arial"><b>Поле</b></font></td>
    <td class="label" width="20%"><font face="Arial"><strong>Тип 
	данных</strong></font></td>
    <td class="label" width="20%"><font face="Arial"><strong>Null</strong></font></td>
    <td class="label" width="40%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="20%"><font face="Arial">fOBJECT</font></td>
    <td width="20%"><font face="Arial">char (32)</font></td>
    <td width="20%"><font face="Arial">NOT NULL</font></td>
    <td width="40%"><font face="Arial">идентификатор текстовой 
	константы</font></td>
  </tr>
  <tr>
    <td width="20%"><font face="Arial">fLANG</font></td>
    <td width="20%"><font face="Arial">smallint</font></td>
    <td width="20%"><font face="Arial">NOT NULL</font></td>
    <td width="40%"><font face="Arial">код языка</font></td>
  </tr>
  <tr>
    <td width="20%"><font face="Arial">fTEXT</font></td>
    <td width="20%"><font face="Arial">varchar (255)</font></td>
    <td width="20%"><font face="Arial">NOT NULL</font></td>
    <td width="40%"><font face="Arial">значение текстовой константы</font></td>
  </tr>
  <tr>
    <td width="20%"><font face="Arial">fLEN</font></td>
    <td width="20%"><font face="Arial">tinyint</font></td>
    <td width="20%"><font face="Arial">NOT NULL</font></td>
    <td width="40%"><font face="Arial">длина текста</font></td>
  </tr>
</TBODY>
</table>

<p class="label"><font face="Arial"><b><br>
Индекс</b></font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
  <tr vAlign="top">
    <td class="label" width="33%"><font face="Arial"><b>Имя индекса</b></font></td>
    <td class="label" width="33%"><font face="Arial"><strong>Тип </strong></font></td>
    <td class="label" width="33%"><font face="Arial"><strong>Имя 
	столбцов</strong></font></td>
  </tr>
  <tr>
    <td width="33%"><font face="Arial">iAPLEZU</font></td>
    <td width="33%"><font face="Arial">UNIQUE,&nbsp; CLUSTERED</font></td>
    <td width="33%"><font face="Arial">fOBJECT, fLANG</font></td>
  </tr>
</table>

<p class="label"><font face="Arial"><b><br>
Примечание</b></font></p>

<p class="label"><a href="database_scheme.html"><font face="Arial">См. 
также</font></a></p>
</body>
</html>