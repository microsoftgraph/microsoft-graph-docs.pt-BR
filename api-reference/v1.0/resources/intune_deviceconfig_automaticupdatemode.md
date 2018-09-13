# <a name="automaticupdatemode-enum-type"></a>tipo enumerado automaticUpdateMode

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para o modo de atualização automática.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Definido pelo usuário, valor padrão, sem intenção.|
|notifyDownload|1|Notificar ao baixar.|
|autoInstallAtMaintenanceTime|2|Instalar automaticamente no período de manutenção.|
|autoInstallAndRebootAtMaintenanceTime|3|Instalar automaticamente e reinicializar no período de manutenção.|
|autoInstallAndRebootAtScheduledTime|4|Instalar automaticamente e reinicializar no horário agendado.|
|autoInstallAndRebootWithoutEndUserControl|5|Instalar automaticamente e reiniciar sem controle de usuário final|








