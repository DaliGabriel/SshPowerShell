# SshPowerShell
Como habilitar y usar ssh desde power shell
<br>

<h1>Abrir power shell como administrador y ejecutar el siguiente comando</h1>
<p>Este comando comprueba que la biblioteca ssh esta disponible</p>

```
Get-WindowsCapability -Online | Where-Object Name -like 'OpenSSH*'
```

<h1>Instalar el Cliente OpenSSH </h1>

```
Add-WindowsCapability -Online -Name OpenSSH.Client~~~~0.0.1.0
```

<h1>Conectar con el servidor ssh</h1>

```
ssh domain\username@servername
```

<p>Para mas informacion al respecto consultar el siguiente <a href="https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=powershell">enlace</a></p>

