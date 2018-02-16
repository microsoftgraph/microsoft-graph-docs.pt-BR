# <a name="devicecompliancepolicystate-resource-type"></a>Tipo de recurso deviceCompliancePolicyState

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Estado de política de conformidade de dispositivo para um determinado dispositivo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceCompliancePolicyStates](../api/intune_deviceconfig_devicecompliancepolicystate_list.md)|Conjunto [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Listar propriedades e relações de objetos de [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).|
|[Obter deviceCompliancePolicyState](../api/intune_deviceconfig_devicecompliancepolicystate_get.md)|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Ler propriedades e relações de objetos de [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).|
|[Criar deviceCompliancePolicyState](../api/intune_deviceconfig_devicecompliancepolicystate_create.md)|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Criar um novo objeto de [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).|
|[Excluir deviceCompliancePolicyState](../api/intune_deviceconfig_devicecompliancepolicystate_delete.md)|Nenhum|Exclui [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).|
|[Atualizar deviceCompliancePolicyState](../api/intune_deviceconfig_devicecompliancepolicystate_update.md)|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Atualizar as propriedades de um objeto de [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|settingStates|Conjunto [deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md)|Ainda não documentado|
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
  "@odata.type": "microsoft.graph.deviceCompliancePolicyState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
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



