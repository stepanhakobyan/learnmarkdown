﻿<html>
<head>
<title>AsErrorsFreeExecutor</title>
<style type="text/css">
.style1 {
	font-family: Arial;
}
</style>
</head>

<body>

<p><strong><font size="3" face="Arial">Пример </font><font
face="Arial">методов <span lang="en-us">Run </span>и </font>
<font size="3" face="Arial"><span lang="en-us">SetErrSubParams</span></font></strong></p>

<p><font face="Arial">В примере вызывается функция 
<a href="../Functions/Functions/CreateErrorsFreeExecutor.html">
CreateErrorsFreeExecutor</a>, задаются имена скриптовых процедур (<span lang="en-us"><em>SubName</em>-</span>имя 
исполняемой процедуры,&nbsp; <em>Err</em><span lang="en-us"><em>SubName</em></span>-имя 
процедуры, которая вызывается только при возникновении ошибки во время 
исполнения<span lang="en-us"> <em>SubName</em></span>). Устанавливается отчет
<span lang="en-us">(</span><strong>RepViewer</strong><span lang="en-us">)</span> 
в котором сохраняются все сообщения об ошибках<span lang="en-us">. </span>Далее, 
в цикле выполняется процедура <span lang="en-us"><em>SubName</em></span> при 
помощи метода <strong>Run.</strong> Перед вызовом метода <strong>Run </strong>
передаются параметры для процедуры <em>Err</em><span lang="en-us"><em>SubName</em></span> 
при помощи метода <strong>SetErrSubParams</strong>.</font></p>

<p><font face="Arial">Set errFee =
<a href="../Functions/Functions/CreateErrorsFreeExecutor.html">
CreateErrorsFreeExecutor</a>(&quot;<span lang="en-us">ModuleName</span>&quot;, &quot;<span lang="en-us">SubName</span>&quot;, 
&quot;Err<span lang="en-us">SubName</span>&quot;)<br>
Set errRep = <a href="../Functions/Functions/CreateRepViewer.html">
CreateRepViewer</a><br>
Set errFee.<strong>RepViewer</strong> = errRep<br>
<strong>....</strong><br>
Set rs = Util.ExecuteQuery(sSql, True, ASOpenKeyset, , , 6000)<br>
Do While Not rs.EOF<br>
&nbsp;&nbsp;&nbsp; i += 1<br>
&nbsp;&nbsp;&nbsp; <strong>....</strong><br>
&nbsp;&nbsp;&nbsp; errFee.<strong>SetErrSubParams </strong>(i, docAgr, errRep)<br>
&nbsp;&nbsp;&nbsp; errFee.<strong>Run </strong>(docAgr)<br>
<br>
&nbsp;&nbsp;&nbsp; <span lang="en-us">rs</span>.MoveNext<br>
Loop <br>
<span lang="en-us">rs.close</span><br>
</font></p>
<p><font face="Arial">Ниже приведены сигнатуры процедур <span lang="en-us"><em>
SubName</em></span> и <span lang="en-us"><em>ErrSubName</em></span>.</font></p>
<p><span class="style1"><span lang="en-us">Public Sub</span> </span><font face="Arial">
<span lang="en-us"><em>SubName</em></span> (<span lang="en-us">ByVal docAgr As 
AsDoc</span>)</font><span class="style1"><span lang="en-us"><br>
Public Sub <em>ErrSubName</em></span> <span lang="en-us">(ByVal lErrNumber As 
Long, ByVal docAgr As AsDoc, ByVal errRep as AsRepViewer)</span></span></p>
<p class="style1">Если параметры для процедуры <font face="Arial"><em>Err</em><em><span lang="en-us">SubName</span>
</em></font>не переданы методом <font face="Arial"><strong>SetErrSubParams</strong>, 
то параметры передаются вызовом метода <span lang="en-us"><strong>Run</strong></span>. 
То есть&nbsp; и <span lang="en-us"><em>SubName</em></span> и&nbsp;
<span lang="en-us"><em>ErrSubName</em></span> должны иметь одну и туже сигнатуру<span lang="en-us">.</span></font></p>
</body>
</html>