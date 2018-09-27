﻿<html>
<head>
<title>Системное событие PrintExcel</title>
</head>

<body>

<p><font size="4" face="Arial"><strong>Событие PrintExcel<br>
<br>
</strong></font><font face="Arial"><a href="PrintWord.html">См. также</a>&nbsp;
<u>Пример</u>&nbsp; <a href="../Defs/doc.html">Применяется к</a></font></p>

<p class="label"><font face="Arial">Происходит при вызове печатной 
формы документа в формате Excel и служит для подстановки параметров в шаблонную 
форму Excel-а. В шаблонной форме в качестве макропеременных могут выступать как 
реквизиты документа, так и другие переменные.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial">Sub <strong>PrintExcel</strong>([<em>TemplateName</em>])<br>
<em>&nbsp;&nbsp; statements</em><br>
End Sub</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>TemplateName</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее имя шаблона подстановки.</font></td>
  </tr>
    </table>

<p class="label"><font face="Arial"><b>Примечание</b></font></p>

<p class="label"><font face="Arial">Файл шаблонной формы должен быть 
предварительно создан и загружен в систему.<br>Вместо обработки события PrintExcel 
желаельно обрабатывать TemplateSubstitution, которая обладет большими 
возможностями и менее зависит от конкретного шаблона.</font></p>
</body>
</html>