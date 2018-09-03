# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a>Tipo de recurso deviceCompliancePolicySettingStateSummary

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Resumo de estado de configuração de política de conformidade do dispositivo por toda a conta.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceCompliancePolicySettingStateSummaries](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_list.md)|Conjunto [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|Listar propriedades e relações de objetos de [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).|
|[Obter deviceCompliancePolicySettingStateSummary](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_get.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|Ler propriedades e relações de objetos de [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).|
|[Criar deviceCompliancePolicySettingStateSummary](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_create.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|Criar um novo objeto de [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).|
|[Excluir deviceCompliancePolicySettingStateSummary](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_delete.md)|Nenhum|Excluir [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).|
|[Atualizar deviceCompliancePolicySettingStateSummary](../api/intune_deviceconfig_devicecompliancepolicysettingstatesummary_update.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|Atualizar as propriedades de um objeto de [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|configuração|Cadeia de caracteres|O nome da classe de configuração e o nome da propriedade.|
|settingName|Cadeia de caracteres|Nome da configuração.|
|platformType|[policyPlatformType](../resources/intune_deviceconfig_policyplatformtype.md)|Plataforma de configuração. Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|id|Cadeia de caracteres|Chave da entidade.|
|unknownDeviceCount|Int32|Número de dispositivos desconhecidos|
|notApplicableDeviceCount|Int32|Número de dispositivos não aplicáveis|
|compliantDeviceCount|Int32|Número de dispositivos em conformidade|
|remediatedDeviceCount|Int32|Número de dispositivos corrigidos|
|nonCompliantDeviceCount|Int32|Número de dispositivos sem conformidade|
|errorDeviceCount|Int32|Número de dispositivos com erro|
|conflictDeviceCount|Int32|Número de dispositivos em conflito|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceComplianceSettingStates|Conjunto [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|Ainda não documentado|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "String",
  "settingName": "String",
  "platformType": "String",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



