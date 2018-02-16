# <a name="roleassignment-resource-type"></a>Tipo de recurso roleAssignment

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar roleAssignments](../api/intune_rbac_roleassignment_list.md)|Conjunto [roleAssignment](../resources/intune_rbac_roleassignment.md)|Listar propriedades e relações de objeto de [roleAssignment](../resources/intune_rbac_roleassignment.md).|
|[Obter roleAssignment](../api/intune_rbac_roleassignment_get.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|Ler propriedades e relações de objetos de [roleAssignment](../resources/intune_rbac_roleassignment.md).|
|[Create roleAssignment](../api/intune_rbac_roleassignment_create.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|Criar um novo objeto de [roleAssignment](../resources/intune_rbac_roleassignment.md).|
|[Excluir roleAssignment](../api/intune_rbac_roleassignment_delete.md)|Nenhum|Excluir [roleAssignment](../resources/intune_rbac_roleassignment.md).|
|[Atualizar roleAssignment](../api/intune_rbac_roleassignment_update.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|Atualizar as propriedades de um objeto de [roleAssignment](../resources/intune_rbac_roleassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. É somente leitura e é gerada automaticamente.|
|displayName|Cadeia de caracteres|O nome de exibição ou amigável da atribuição de função.|
|descrição|Cadeia de caracteres|Descrição da atribuição de função.|
|resourceScopes|Conjunto de cadeia de caracteres|Lista de IDs dos grupos de segurança de membros de escopo da função.  Estas são as IDs do Azure Active Directory.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune_rbac_roledefinition.md)|A definição de função da qual essa atribuição faz parte.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```



