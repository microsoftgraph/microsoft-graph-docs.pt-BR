# <a name="windowsphone81generalconfiguration-resource-type"></a>Tipo de recurso windowsPhone81GeneralConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso windowsPhone81GeneralConfiguration.

Herda de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsPhone81GeneralConfigurations](../api/intune_deviceconfig_windowsphone81generalconfiguration_list.md)|Coleção [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md)|Listar propriedades e relações dos objetos [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).|
|[Obter windowsPhone81GeneralConfiguration](../api/intune_deviceconfig_windowsphone81generalconfiguration_get.md)|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md)|Ler propriedades e relações do objeto [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).|
|[Criar windowsPhone81GeneralConfiguration](../api/intune_deviceconfig_windowsphone81generalconfiguration_create.md)|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md)|Criar um novo objeto [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).|
|[Excluir windowsPhone81GeneralConfiguration](../api/intune_deviceconfig_windowsphone81generalconfiguration_delete.md)|Nenhum|Excluir um [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).|
|[Atualizar windowsPhone81GeneralConfiguration](../api/intune_deviceconfig_windowsphone81generalconfiguration_update.md)|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md)|Atualizar as propriedades de um objeto [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Última modificação de DateTime do objeto. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|applyOnlyToWindowsPhone81|Booliano|Valor que indica se esta política se aplica somente ao Windows Phone 8.1. Essa propriedade é somente leitura.|
|appsBlockCopyPaste|Booliano|Indica se a função copiar/colar deve ou não ser bloqueada.|
|bluetoothBlocked|Booliano|Indica se o bluetooth deve ou não ser bloqueado.|
|cameraBlocked|Booliano|Indica se a câmera deve ou não ser bloqueada.|
|cellularBlockWifiTethering|Booliano|Indica se o compartilhamento de Internet por Wi-Fi devem ou não ser bloqueado. Não terá impacto se o Wi-Fi estiver bloqueado.|
|compliantAppsList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType). Essa coleção pode conter um máximo de 10000 elementos.|
|compliantAppListType|Cadeia de caracteres|Lista que está em AppComplianceList. Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|diagnosticDataBlockSubmission|Booliano|Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.|
|emailBlockAddingAccounts|Booliano|Indica se as contas de email personalizadas devem ou não ser bloqueadas.|
|locationServicesBlocked|Booliano|Indica se os serviços de localização devem ou não ser bloqueados.|
|microsoftAccountBlocked|Booliano|Indica se o uso de uma conta da Microsoft deve ou não ser bloqueado.|
|nfcBlocked|Booliano|Indica se a comunicação a curta distância deve ou não ser bloqueada.|
|passwordBlockSimple|Booliano|Indica se a sincronização do calendário deve ou não ser bloqueada.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha.|
|passwordMinimumLength|Int32|Comprimento mínimo das senhas.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordMinimumCharacterSetCount|Int32|Número de conjuntos de caracteres que uma senha deve conter.|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear. Valores válidos de 0 a 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Número permitido de falhas de entrada antes da redefinição de fábrica.|
|passwordRequiredType|Cadeia de caracteres|Tipo de senha necessário. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordRequired|Booliano|Indica se uma senha deve ou não ser exigida.|
|screenCaptureBlocked|Booliano|Indica se capturas de tela devem ou não ser bloqueadas.|
|storageBlockRemovableStorage|Booliano|Indica se o armazenamento removível deve ou não ser bloqueado.|
|storageRequireEncryption|Booliano|Indica se a criptografia é ou não necessária.|
|webBrowserBlocked|Booliano|Indica se o navegador da Web deve ou não ser bloqueado.|
|wifiBlocked|Booliano|Indica se o Wi-Fi deve ou não ser bloqueado.|
|wifiBlockAutomaticConnectHotspots|Booliano|Indica se a conexão automática a hotspots Wi-Fi deve ou não ser bloqueada. Não terá impacto se o Wi-Fi estiver bloqueado.|
|wifiBlockHotspotReporting|Booliano|Indica se os relatórios de hotspot Wi-Fi devem ou não ser bloqueados. Não terá impacto se o Wi-Fi estiver bloqueado.|
|windowsStoreBlocked|Booliano|Indica se a Windows Store deve ou não ser bloqueada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Status da instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81GeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```



