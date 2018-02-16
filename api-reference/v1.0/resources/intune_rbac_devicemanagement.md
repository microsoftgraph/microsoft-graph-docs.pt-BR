# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune_rbac_devicemanagement_get.md)|[deviceManagement](../resources/intune_rbac_devicemanagement.md)|Ler propriedades e relações de objetos de [deviceManagement](../resources/intune_rbac_devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune_rbac_devicemanagement_update.md)|[deviceManagement](../resources/intune_rbac_devicemanagement.md)|Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune_rbac_devicemanagement.md).|
|[Função getEffectivePermissions](../api/intune_rbac_devicemanagement_geteffectivepermissions.md)|Conjunto [rolePermission](../resources/intune_rbac_rolepermission.md)|Recupera permissões efetivas de usuário autenticado no momento|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|roleDefinitions|Conjunto [roleDefinition](../resources/intune_rbac_roledefinition.md)|As definições da função.|
|roleAssignments|Conjunto [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|As atribuições da função|
|resourceOperations|Conjunto [resourceOperation](../resources/intune_rbac_resourceoperation.md)|As operações de recurso.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



