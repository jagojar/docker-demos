FROM mcr.microsoft.com/windows/servercore:ltsc2022

LABEL owner="cloudarchitectureteam@contoso.com"

RUN powershell -Command Add-WindowsFeature Web-Server

ADD ServiceMonitor.exe /ServiceMonitor.exe

EXPOSE 80

ENTRYPOINT ["C:\\ServiceMonitor.exe", "w3svc"]