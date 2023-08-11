# Ambiente-wsl2-docker-win11pro-EXECUTANDO

### criar maquina virtual win 11 pro

### logar na maquina

### executar power shell como administrador

### wsl – -install

### pesquisar loja

### baixar ubuntu-22.04

### baixar Windows Terminal

### instalar cli power shell
- https://aka.ms/installazurecliwindowsx64

### habilitar tabulação no poswer shell

<pre>
Register-ArgumentCompleter -Native -CommandName az -ScriptBlock {
    param($commandName, $wordToComplete, $cursorPosition)
    $completion_file = New-TemporaryFile
    $env:ARGCOMPLETE_USE_TEMPFILES = 1
    $env:_ARGCOMPLETE_STDOUT_FILENAME = $completion_file
    $env:COMP_LINE = $wordToComplete
    $env:COMP_POINT = $cursorPosition
    $env:_ARGCOMPLETE = 1
    $env:_ARGCOMPLETE_SUPPRESS_SPACE = 0
    $env:_ARGCOMPLETE_IFS = "`n"
    $env:_ARGCOMPLETE_SHELL = 'powershell'
    az 2>&1 | Out-Null
    Get-Content $completion_file | Sort-Object | ForEach-Object {
        [System.Management.Automation.CompletionResult]::new($_, $_, "ParameterValue", $_)
    }
    Remove-Item $completion_file, Env:\_ARGCOMPLETE_STDOUT_FILENAME, Env:\ARGCOMPLETE_USE_TEMPFILES, Env:\COMP_LINE, Env:\COMP_POINT, Env:\_ARGCOMPLETE, Env:\_ARGCOMPLETE_SUPPRESS_SPACE, Env:\_ARGCOMPLETE_IFS, Env:\_ARGCOMPLETE_SHELL
}
</pre>


### install docker desktop win 11 pro
https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe?utm_source=docker&utm_medium=webreferral&utm_campaign=dd-smartbutton&utm_location=module&_gl=1*bbgtto*_ga*MTA2MzkwMTEyLjE2OTE3NTMyNTE.*_ga_XJWPQMJYHQ*MTY5MTc1MzI1MC4xLjEuMTY5MTc1MzI1MS41OS4wLjA.

### install git
https://github.com/git-for-windows/git/releases/download/v2.41.0.windows.3/Git-2.41.0.3-64-bit.exe

### install primeirta container app
https://learn.microsoft.com/en-us/azure/container-apps/overview

### install visual studio code
[https://code.visualstudio.com/download#](https://code.visualstudio.com/Download)https://code.visualstudio.com/Download
