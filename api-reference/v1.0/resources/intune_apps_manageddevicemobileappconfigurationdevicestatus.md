# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a>tipo de recurso de managedDeviceMobileAppConfigurationDeviceStatus

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades, propriedades herdadas e ações para um status de configuração de um aplicativo móvel de MDM para um dispositivo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceMobileAppConfigurationDeviceStatuses](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_list.md)|coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)|Listar propriedades e relações de objetos [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).|
|[Obter managedDeviceMobileAppConfigurationDeviceStatus](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_get.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)|Ler as propriedades e relações do objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).|
|[Criar managedDeviceMobileAppConfigurationDeviceStatus](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_create.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)|Criar um novo objeto[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).|
|[Excluir managedDeviceMobileAppConfigurationDeviceStatus](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_delete.md)|Nenhum|Exclui um [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).|
|[Atualizar managedDeviceMobileAppConfigurationDeviceStatus](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_update.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)|Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|deviceDisplayName|Cadeia de caracteres|Nome do dispositivo de DevicePolicyStatus.|
|userName|Cadeia de caracteres|O nome de usuário que está sendo relatado|
|deviceModel|Cadeia de caracteres|O modelo do dispositivo que está sendo relatado|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|DateTime em que o período de cortesia de conformidade do dispositivo termina|
|status|[complianceStatus](../resources/intune_shared_compliancestatus.md)|Status de conformidade do relatório de política. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Data e hora da última modificação do relatório de políticas.|
|userPrincipalName|Cadeia de caracteres|UserPrincipalName.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```








