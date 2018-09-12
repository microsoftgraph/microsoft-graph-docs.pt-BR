# <a name="managedebookassignment-resource-type"></a>Tipo de recurso managedEBookAssignment

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades usadas para atribuir um livro eletrônico a um grupo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedEBookAssignments](../api/intune_books_managedebookassignment_list.md)|Conjunto [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Listar propriedades e relações de objetos de [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|
|[Obter managedEBookAssignment](../api/intune_books_managedebookassignment_get.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Ler propriedades e relações de objetos de [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|
|[Criar managedEBookAssignment](../api/intune_books_managedebookassignment_create.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Criar um novo objeto de [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|
|[Excluir managedEBookAssignment](../api/intune_books_managedebookassignment_delete.md)|Nenhum|Excluir [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|
|[Atualizar managedEBookAssignment](../api/intune_books_managedebookassignment_update.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Atualizar as propriedades de um objeto de [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|O destino da atribuição do livro eletrônico.|
|installIntent|[installIntent](../resources/intune_shared_installintent.md)|A intenção de instalação para eBook. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```








