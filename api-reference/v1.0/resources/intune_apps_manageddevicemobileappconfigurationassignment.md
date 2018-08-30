# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a>Tipo de recurso managedDeviceMobileAppConfigurationAssignment

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém as propriedades usadas para atribuir uma configuração de aplicativo MDM a um grupo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceMobileAppConfigurationAssignments](../api/intune_apps_manageddevicemobileappconfigurationassignment_list.md)|Conjunto [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|Listar propriedades e relações de objetos de [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).|
|[Obter managedDeviceMobileAppConfigurationAssignment](../api/intune_apps_manageddevicemobileappconfigurationassignment_get.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).|
|[Criar managedDeviceMobileAppConfigurationAssignment](../api/intune_apps_manageddevicemobileappconfigurationassignment_create.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|Criar um novo objeto de [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).|
|[Excluir managedDeviceMobileAppConfigurationAssignment](../api/intune_apps_manageddevicemobileappconfigurationassignment_delete.md)|Nenhum|Excluir um [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).|
|[Atualizar managedDeviceMobileAppConfigurationAssignment](../api/intune_apps_manageddevicemobileappconfigurationassignment_update.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Destino de atribuição ao qual a política de T&C foi designada.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



