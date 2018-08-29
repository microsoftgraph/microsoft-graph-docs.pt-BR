# <a name="deviceconfigurationsettingstate-resource-type"></a>tipo de recurso deviceConfigurationSettingState

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Estado da definição de configuração de um determinado dispositivo.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|configuração|Cadeia de caracteres|A configuração que está sendo relatada|
|settingName|Cadeia de caracteres|Nome traduzido/amigável para o usuário da configuração que está sendo relatada|
|instanceDisplayName|Cadeia de caracteres|Nome da instância de configuração está sendo relatada.|
|state|[complianceStatus](../resources/intune_shared_compliancestatus.md)|O estado de conformidade da configuração. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.|
|errorCode|Int64|Código de erro da configuração|
|errorDescription|Cadeia de caracteres|Descrição do erro|
|userId|Cadeia de caracteres|UserId|
|userName|Cadeia de caracteres|UserName|
|userEmail|Cadeia de caracteres|UserEmail|
|userPrincipalName|Cadeia de caracteres|UserPrincipalName.|
|sources|Coleção [settingSource](../resources/intune_deviceconfig_settingsource.md)|Políticas colaboradoras|
|currentValue|Cadeia de caracteres|Valor atual da configuração no dispositivo|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
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
```



