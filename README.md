<html>
<head>
    <title>Application Executer</title>
    <HTA:APPLICATION ID="oMyApp" 
	    APPLICATIONNAME="Application Executer" 
	    BORDER="no"
	    CAPTION="no"
	    SHOWINTASKBAR="yes"
	    SINGLEINSTANCE="yes"
	    SYSMENU="yes"
	    SCROLL="no"
	    WINDOWSTATE="normal">
    <script type="text/javascript" language="javascript">
        function RunFile() {
		WshShell = new ActiveXObject("WScript.Shell");
		WshShell.Run("c:/windows/system32/notepad.exe", 1, false);
        }
    </script>
</head>
<body>
	<input type="button" value="Run Notepad" onclick="RunFile();"/>
</body>
</html>
