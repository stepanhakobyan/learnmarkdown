﻿<html>
<head>
<title>Dialog_Deactivate</title>
</head>

<body>

<p><font size="3" face="Arial"><strong>Пример события 
Dialog_Deactivate</strong></font></p>

<p><font face="Arial">Ниже приведен пример обработчика события <strong>
Dialog_Deactivate</strong> из <a
href="../Defs/Dialog.html">описания диалога</a>, где происходит высвобождение 
ресурсов, захваченных во время активизации диалога.</font></p>

<p><font face="Arial">Sub <strong>Dialog_Activate()</strong><br>
&nbsp;&nbsp;&nbsp; DeleteObject(hBitmap)<br>
End Sub<br>
</font></p>

</body>
</html>