# <a name="mobileappassignment-resource-type"></a>Tipo de recurso mobileAppAssignment

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma classe com as propriedades usadas para atribuição de grupos de um aplicativo móvel.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppAssignments](../api/intune_apps_mobileappassignment_list.md)|Conjunto [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Listar propriedades e relações de objetos de [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).|
|[Obter mobileAppAssignment](../api/intune_apps_mobileappassignment_get.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Ler propriedades e relações de objetos de [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).|
|[Criar mobileAppAssignment](../api/intune_apps_mobileappassignment_create.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Criar um novo objeto de [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).|
|[Excluir mobileAppAssignment](../api/intune_apps_mobileappassignment_delete.md)|Nenhum|Excluir uma [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).|
|[Atualizar mobileAppAssignment](../api/intune_apps_mobileappassignment_update.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Atualizar as propriedades de um objeto de [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|finalidade|Cadeia de caracteres|A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune_apps_deviceandappmanagementassignmenttarget.md)|A atribuição do grupo de destino definida pelo administrador.|
|configurações|[mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)|As configurações para a atribuição de destino definida pelo administrador.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



