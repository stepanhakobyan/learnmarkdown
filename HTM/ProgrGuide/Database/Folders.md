﻿<html>
<head>
<title>Таблица FOLDERS</title>
</head>

<body>

<h1><font size="4" face="Arial">Таблица FOLDERS</font></h1>

<p><font face="Arial">Таблицa папок.<br>
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
    <td width="20%"><font face="Arial">fFOLDERID</font></td>
    <td width="20%"><font face="Arial">varchar (20)</font></td>
    <td width="20%"><font face="Arial">NOT NULL</font></td>
    <td width="40%"><font face="Arial">идентификатор папки</font></td>
  </tr>
  <tr>
    <td width="20%"><font face="Arial">fNAME</font></td>
    <td width="20%"><font face="Arial">char (8)</font></td>
    <td width="20%"><font face="Arial">NOT NULL</font></td>
    <td width="40%"><font face="Arial">имя документа основания</font></td>
  </tr>
  <tr>
    <td width="20%"><font face="Arial">fKEY</font></td>
    <td width="20%"><font face="Arial">varchar (24)</font></td>
    <td width="20%"><font face="Arial">NULL</font></td>
    <td width="40%"><font face="Arial">ключ определяющий порядок 
	документов в папке</font></td>
  </tr>
  <tr>
    <td width="20%"><font face="Arial">fISN</font></td>
    <td width="20%"><font face="Arial">int</font></td>
    <td width="20%"><font face="Arial">NOT NULL</font></td>
    <td width="40%"><font face="Arial">внутрисистемный 
	идентификационный код (ISN)&nbsp; документа</font></td>
  </tr>
  <tr>
    <td width="20%"><font face="Arial">fSTATUS</font></td>
    <td width="20%"><font face="Arial">tinyint</font></td>
    <td width="20%"><font face="Arial">NOT NULL</font></td>
    <td width="40%"><font face="Arial">статус элемента папки</font></td>
  </tr>
  <tr>
    <td width="20%"><font face="Arial">fCOM</font></td>
    <td width="20%"><font face="Arial">varchar (50)</font></td>
    <td width="20%"><font face="Arial">NULL</font></td>
    <td width="40%"><font face="Arial">комментарий</font></td>
  </tr>
  <tr>
    <td width="20%"><font face="Arial">fSPEC</font></td>
    <td width="20%"><font face="Arial">varchar (255)</font></td>
    <td width="20%"><font face="Arial">NULL</font></td>
    <td width="40%"><font face="Arial">специальная строка</font></td>
  </tr>
  <tr>
    <td width="20%"><font face="Arial">fECOM</font></td>
    <td width="20%"><font face="Arial">varchar (50)</font></td>
    <td width="20%"><font face="Arial">NULL</font></td>
    <td width="40%"><font face="Arial">комментарий в иностранном языке</font></td>
  </tr>
  <tr>
    <td width="20%"><font face="Arial">fDCDATE</font></td>
    <td width="20%"><font face="Arial">datetime</font></td>
    <td width="20%"><font face="Arial">NOT NULL</font></td>
    <td width="40%"><font face="Arial">дата создания документа</font></td>
  </tr>
	<tr>
    <td width="20%">fDCBRANCH </td>
    <td width="20%"><font face="Arial">char (3)</font></td>
    <td width="20%"><font face="Arial">NOT NULL</font></td>
    <td width="40%"><font face="Arial">код филиала</font></td>
  </tr>
	<tr>
    <td width="20%">fDCDEPART </td>
    <td width="20%"><font face="Arial">char (3)</font></td>
    <td width="20%"><font face="Arial">NOT NULL</font></td>
    <td width="40%"><font face="Arial">код отдела</font></td>
  </tr>
  <tr>
    <td width="20%">fDCACSTYPE </td>
    <td width="20%"><font face="Arial">char (2)</font></td>
    <td width="20%"><font face="Arial">NOT NULL</font></td>
    <td width="40%"><font face="Arial">код типа доступа</font></td>
  </tr>
</TBODY>
</table>

<p class="label"><font face="Arial"><b><br>
Индекс</b></font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
  <tr vAlign="top">
    <td class="label" width="33%" nowrap><font face="Arial"><b>Имя 
	индекса</b></font></td>
    <td class="label" width="33%" nowrap><font face="Arial"><strong>
	Тип </strong></font></td>
    <td class="label" width="33%" nowrap><font face="Arial"><strong>
	Имя столбцов</strong></font></td>
  </tr>
  <tr>
    <td width="33%" nowrap><font face="Arial">iFOLDERS1</font></td>
    <td width="33%" nowrap><font face="Arial">UNIQUE, CLUSTERED</font></td>
    <td width="33%" nowrap><font face="Arial">fFOLDERID, fKEY</font></td>
  </tr>
  <tr>
    <td width="33%" nowrap><font face="Arial">iFOLDERS2</font></td>
    <td width="33%" nowrap>&nbsp;</td>
    <td width="33%" nowrap><font face="Arial">fISN</font></td>
  </tr>
</table>

<p class="label"><font face="Arial"><b><br>
<br>
Примечание</b></font></p>

<p class="label"><a href="database_scheme.html"><font face="Arial">См. 
также</font></a></p>
</body>
</html>