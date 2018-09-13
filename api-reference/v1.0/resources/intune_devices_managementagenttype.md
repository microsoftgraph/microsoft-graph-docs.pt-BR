# <a name="managementagenttype-enum-type"></a>tipo enumerado managementAgentType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Tipo de agente de gerenciamento.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|eas|1|O dispositivo é gerenciado pelo Exchange server.|
|mdm|2|O dispositivo é gerenciado pelo gerenciamento de dispositivo móvel Intune.|
|easMdm|3|O dispositivo é gerenciado pelo Exchange Server e pelo gerenciamento de dispositivo móvel Intune.|
|intuneClient|4|Gerenciado pelo cliente Intune.|
|easIntuneClient|5|O dispositivo é gerenciado pelo EAS e pelo cliente Intune.|
|configurationManagerClient|8|O dispositivo é gerenciado pelo Gerenciador de Configurações.|
|configurationManagerClientMdm|10|O dispositivo é gerenciado pelo Gerenciador de Configurações e pelo gerenciamento de dispositivo móvel.|
|configurationManagerClientMdmEas|11|O dispositivo é gerenciado pelo Gerenciador de Configurações, pelo gerenciamento de dispositivo móvel e pelo Eas.|
|unknown|16|Tipo de agente de gerenciamento desconhecido.|
|jamf|32|Os atributos de dispositivo são obtidos no Jamf.|
|googleCloudDevicePolicyController|64|O dispositivo é gerenciado por CloudDPC do Google.|








