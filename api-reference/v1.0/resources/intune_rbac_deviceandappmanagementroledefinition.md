# <a name="deviceandappmanagementroledefinition-resource-type"></a>Tipo de recurso deviceAndAppManagementRoleDefinition

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.

Herda de [roleDefinition](../resources/intune_rbac_roledefinition.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceAndAppManagementRoleDefinitions](../api/intune_rbac_deviceandappmanagementroledefinition_list.md)|Coleção [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|Lista propriedades e relações dos objetos [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).|
|[Obter deviceAndAppManagementRoleDefinition](../api/intune_rbac_deviceandappmanagementroledefinition_get.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|Propriedades de leitura e relações do objeto [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).|
|[Criar deviceAndAppManagementRoleDefinition](../api/intune_rbac_deviceandappmanagementroledefinition_create.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).|
|[Excluir deviceAndAppManagementRoleDefinition](../api/intune_rbac_deviceandappmanagementroledefinition_delete.md)|Nenhum|Exclui um [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).|
|[Atualizar deviceAndAppManagementRoleDefinition](../api/intune_rbac_deviceandappmanagementroledefinition_update.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|Atualiza as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. É somente leitura e é gerada automaticamente. Herdado de [roleDefinition](../resources/intune_rbac_roledefinition.md)|
|displayName|Cadeia de caracteres|Nome de exibição da definição de Função. Herdado de [roleDefinition](../resources/intune_rbac_roledefinition.md)|
|descrição|Cadeia de caracteres|Descrição da definição de Função. Herdado de [roleDefinition](../resources/intune_rbac_roledefinition.md)|
|rolePermissions|Coleção [rolePermission](../resources/intune_rbac_rolepermission.md)|Lista de Permissões de Função que esta função está autorizada a executar. Elas devem corresponder ao actionName definido como parte de rolePermission. Herdado de [roleDefinition](../resources/intune_rbac_roledefinition.md)|
|isBuiltIn|Booliano|Tipo de Função. Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada. Herdado de [roleDefinition](../resources/intune_rbac_roledefinition.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|roleAssignments|Coleção [roleAssignment](../resources/intune_rbac_roleassignment.md)|Lista de atribuições de função para esta definição de função. Herdado de [roleDefinition](../resources/intune_rbac_roledefinition.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.roleDefinition",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



