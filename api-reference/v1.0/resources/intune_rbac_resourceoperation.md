# <a name="resourceoperation-resource-type"></a>Tipo de recurso resourceOperation

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Isso define uma operação ou ação que pode ser executada em um recurso (ou entidade) do Intune.  As operações comuns são Ler, Excluir, Atualizar ou Criar.  Essas operações fornecem gerenciamento básico do recurso do Intune subjacente em si.  Em alguns casos, um recurso do Intune pode ter operações usadas pelo recurso para agir em combinação com outros recursos.  Por exemplo, a operação Assign é usada para atribuir um recurso MobileApp a um grupo de segurança AAD.  Não é possível modificar as operações de recursos para funções internas. Isso define uma operação ou ação que pode ser executada em um recurso (ou entidade) do Intune.  As operações comuns são Obter, Listar, Excluir, Atualizar ou Criar.  Essas operações fornecem gerenciamento básico do recurso do Intune subjacente em si.  Em alguns casos, um recurso do Intune pode ter operações usadas pelo recurso para agir em combinação com outros recursos.  Por exemplo, a operação “Assign” é usada para atribuir um recurso MobileApp a um grupo de segurança AAD.  Não é possível modificar as operações de recursos para funções internas.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar resourceOperations](../api/intune_rbac_resourceoperation_list.md)|Coleção [resourceOperation](../resources/intune_rbac_resourceoperation.md)|Listar propriedades e relações dos objetos [resourceOperation](../resources/intune_rbac_resourceoperation.md).|
|[Obter resourceOperation](../api/intune_rbac_resourceoperation_get.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md)|Ler propriedades e relações do objeto [resourceOperation](../resources/intune_rbac_resourceoperation.md).|
|[Criar resourceOperation](../api/intune_rbac_resourceoperation_create.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md)|Criar um novo objeto [resourceOperation](../resources/intune_rbac_resourceoperation.md).|
|[Excluir resourceOperation](../api/intune_rbac_resourceoperation_delete.md)|Nenhum|Excluir um [resourceOperation](../resources/intune_rbac_resourceoperation.md)|
|[Atualizar resourceOperation](../api/intune_rbac_resourceoperation_update.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md)|Atualizar as propriedades de um objeto [resourceOperation](../resources/intune_rbac_resourceoperation.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da operação de recurso. Somente leitura, gerada automaticamente.|
|resourceName|Cadeia de caracteres|Nome do recurso em que essa operação é executada.|
|actionName|Cadeia de caracteres|Tipo de ação em que essa operação será executada. O actionName deve ser conciso e limitado ao mínimo de palavras possível.|
|description|Cadeia de caracteres|Descrição da operação de recurso. A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resourceName": "String",
  "actionName": "String",
  "description": "String"
}
```



