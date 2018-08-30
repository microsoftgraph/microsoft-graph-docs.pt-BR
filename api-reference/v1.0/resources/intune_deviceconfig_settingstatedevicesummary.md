# <a name="settingstatedevicesummary-resource-type"></a>Tipo de recurso settingStateDeviceSummary

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração e política de conformidade de dispositivo para um resumo de estado de configuração
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar settingStateDeviceSummaries](../api/intune_deviceconfig_settingstatedevicesummary_list.md)|Conjunto [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Listar propriedades e relações de objetos de [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).|
|[Obter settingStateDeviceSummary](../api/intune_deviceconfig_settingstatedevicesummary_get.md)|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Ler propriedades e relações de objetos de [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).|
|[Criar settingStateDeviceSummary](../api/intune_deviceconfig_settingstatedevicesummary_create.md)|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Criar um novo objeto de [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).|
|[Excluir settingStateDeviceSummary](../api/intune_deviceconfig_settingstatedevicesummary_delete.md)|Nenhum|Excluir [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).|
|[Atualizar settingStateDeviceSummary](../api/intune_deviceconfig_settingstatedevicesummary_update.md)|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Atualizar as propriedades de um objeto de [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|settingName|Cadeia de caracteres|Nome da configuração|
|instancePath|Cadeia de caracteres|Nome de InstancePath para a configuração|
|unknownDeviceCount|Int32|Contagem desconhecida de dispositivos para a configuração|
|notApplicableDeviceCount|Int32|Contagem não aplicável ao dispositivo para a configuração|
|compliantDeviceCount|Int32|Contagem de dispositivo em conformidade para a configuração|
|remediatedDeviceCount|Int32|Contagem de dispositivo em conformidade para a configuração|
|nonCompliantDeviceCount|Int32|Contagem de dispositivo sem conformidade para a configuração|
|errorDeviceCount|Int32|Contagem de erros de dispositivo para a configuração|
|conflictDeviceCount|Int32|Contagem de erro de conflito de dispositivo para a configuração|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



