# <a name="roledefinition-resource-type"></a>Tipo de recurso roleDefinition

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso de Definição de Função. A definição da função é a base do acesso baseado em função no Intune. A função combina um recurso do Intune, como um aplicativo móvel e permissões de função associadas, como Criar ou Ler para o recurso. Existem dois tipos de funções: internas e personalizadas. Funções internas não podem ser modificadas. Tanto funções internas quanto personalizadas devem ter atribuições a serem impostas. Crie funções personalizadas se quiser definir uma função que permita que qualquer um dos recursos disponíveis e permissões de funções sejam combinados em uma única função.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar roleDefinitions](../api/intune_rbac_roledefinition_list.md)|Coleção [roleDefinition](../resources/intune_rbac_roledefinition.md)|Listar propriedades e relações dos objetos [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|[Obter roleDefinition](../api/intune_rbac_roledefinition_get.md)|[roleDefinition](../resources/intune_rbac_roledefinition.md)|Ler propriedades e relações do objeto [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|[Criar roleDefinition](../api/intune_rbac_roledefinition_create.md)|[roleDefinition](../resources/intune_rbac_roledefinition.md)|Criar um novo objeto [roleDefinition](../resources/intune_rbac_roledefinition.md)|
|[Excluir roleDefinition](../api/intune_rbac_roledefinition_delete.md)|Nenhum|Excluir um [roleDefinition](../resources/intune_rbac_roledefinition.md)|
|[Atualizar roleDefinition](../api/intune_rbac_roledefinition_update.md)|[roleDefinition](../resources/intune_rbac_roledefinition.md)|Atualizar as propriedades de um objeto [roleDefinition](../resources/intune_rbac_roledefinition.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. É somente leitura e é gerada automaticamente.|
|displayName|Cadeia de caracteres|Nome de exibição da definição de Função.|
|description|Cadeia de caracteres|Descrição da definição de Função.|
|rolePermissions|Coleção [rolePermission](../resources/intune_rbac_rolepermission.md)|Lista de Permissões de Função que esta função está autorizada a executar. Elas devem corresponder ao actionName definido como parte de rolePermission.|
|isBuiltIn|Booliano|Tipo de Função. Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|roleAssignments|Coleção [roleAssignment](../resources/intune_rbac_roleassignment.md)|Lista de atribuições de função para esta definição de função.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.roleDefinition"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
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



