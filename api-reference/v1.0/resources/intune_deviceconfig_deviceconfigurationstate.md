# <a name="deviceconfigurationstate-resource-type"></a>Tipo de recurso deviceConfigurationState

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Estado de configuração do dispositivo para um determinado dispositivo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceConfigurationStates](../api/intune_deviceconfig_deviceconfigurationstate_list.md)|Conjunto [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Lista de propriedades e relações de objetos de [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).|
|[Obter deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_get.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Ler propriedades e relações de objetos de [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).|
|[Criar deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_create.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Criar um novo objeto de [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).|
|[Excluir deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_delete.md)|Nenhum|Excluir [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).|
|[Atualizar deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_update.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Atualizar as propriedades de um objeto de [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|settingStates|Conjunto [deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md)|Ainda não documentado|
|displayName|Cadeia de caracteres|O nome da política dessa policyBase|
|versão|Int32|A versão da política.|
|platformType|Cadeia de caracteres|Tipo de plataforma ao qual a política se aplica Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.|
|estado|Cadeia de caracteres|O estado de conformidade da política Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.|
|settingCount|Int32|Contagem de quantas configurações uma política contém|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "String",
      "settingName": "String",
      "instanceDisplayName": "String",
      "state": "String",
      "errorCode": 1024,
      "errorDescription": "String",
      "userId": "String",
      "userName": "String",
      "userEmail": "String",
      "userPrincipalName": "String",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "String",
          "displayName": "String"
        }
      ],
      "currentValue": "String"
    }
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024
}
```



