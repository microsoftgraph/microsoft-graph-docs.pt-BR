# <a name="sharedpcconfiguration-resource-type"></a>Tipo de recurso sharedPCConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso sharedPCConfiguration.

Herda de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar sharedPCConfigurations](../api/intune_deviceconfig_sharedpcconfiguration_list.md)|Coleção [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)|Lista propriedades e relações dos objetos [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).|
|[Obter sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_get.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)|Propriedades de leitura e relações do objeto [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).|
|[Criar sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_create.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)|Cria um novo objeto [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).|
|[Excluir sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_delete.md)|Nenhum|Exclui um [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).|
|[Atualizar sharedPCConfiguration](../api/intune_deviceconfig_sharedpcconfiguration_update.md)|[sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md)|Atualiza as propriedades de um objeto [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|accountManagerPolicy|[sharedPCAccountManagerPolicy](../resources/intune_deviceconfig_sharedpcaccountmanagerpolicy.md)|Especifica como as contas são gerenciadas em um PC compartilhado. Aplica-se somente quando disableAccountManager é false.|
|allowedAccounts|[sharedPCAllowedAccountType](../resources/intune_deviceconfig_sharedpcallowedaccounttype.md)|Indica que tipos de contas podem ser usadas em um PC compartilhado. Os valores possíveis são: `guest`, `domain`.|
|allowLocalStorage|Booleano|Especifica se o armazenamento local é permitido em um PC compartilhado.|
|disableAccountManager|Booleano|Desabilita o gerente de contas para o modo de PC compartilhado.|
|disableEduPolicies|Booleano|Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas. Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.|
|disablePowerPolicies|Booleano|Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.|
|disableSignInOnResume|Booleano|Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.|
|enabled|Booleano|Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.|
|idleTimeBeforeSleepInSeconds|Int32|Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão. Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.|
|kioskAppDisplayName|Cadeia de caracteres|Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId. Aplicável somente quando KioskAppUserModelId está definido.|
|kioskAppUserModelId|Cadeia de caracteres|Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.|
|maintenanceStartTime|TimeOfDay|Especifica o horário de início diário da hora de manutenção.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.deviceConfiguration",
  "@odata.type": "microsoft.graph.sharedPCConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "String",
    "cacheAccountsAboveDiskFreePercentage": 1024,
    "inactiveThresholdDays": 1024,
    "removeAccountsBelowDiskFreePercentage": 1024
  },
  "allowedAccounts": "String",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 1024,
  "kioskAppDisplayName": "String",
  "kioskAppUserModelId": "String",
  "maintenanceStartTime": "String (time of day)"
}
```



