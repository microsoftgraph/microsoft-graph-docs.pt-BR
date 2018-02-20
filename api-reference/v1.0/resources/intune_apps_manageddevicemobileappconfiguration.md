# <a name="manageddevicemobileappconfiguration-resource-type"></a>Tipo de recurso managedDeviceMobileAppConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceMobileAppConfigurations](../api/intune_apps_manageddevicemobileappconfiguration_list.md)|Coleção [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)|Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md).|
|[Obter managedDeviceMobileAppConfiguration](../api/intune_apps_manageddevicemobileappconfiguration_get.md)|[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)|Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|targetedMobileApps|Coleção de cadeias de caracteres|o aplicativo associado.|
|createdDateTime|DateTimeOffset|Data e hora em que o objeto foi criado.|
|description|Cadeia de caracteres|Descrição fornecida pelo administrador da Configuração do dispositivo.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|displayName|Cadeia de caracteres|Nome fornecido pelo administrador da configuração do dispositivo.|
|version|Int32|Versão da configuração do dispositivo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|A lista de atribuições de grupo para configuração de aplicativos.|
|userStatuses|Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)|Lista de ManagedDeviceMobileAppConfigurationUserStatus.|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|Resumo do status do dispositivo de configuração do aplicativo.|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|Resumo do status do usuário de configuração do aplicativo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



