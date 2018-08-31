# <a name="iosvppebookassignment-resource-type"></a>Tipo de recurso iosVppEBookAssignment

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades usadas para atribuir um livro eletrônico iOS VPP a um grupo.

Herda de [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosVppEBookAssignments](../api/intune_books_iosvppebookassignment_list.md)|Conjunto [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|Listar propriedades e relações de objetos de [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).|
|[Obter iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_get.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|Ler propriedades e relações de objetos de [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).|
|[Criar iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_create.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|Criar um novo objeto de [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).|
|[Excluir iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_delete.md)|Nenhum|Excluir [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).|
|[Atualizar iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_update.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|Atualizar as propriedades de um objeto de [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herda do [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|O destino da atribuição do livro eletrônico. Herda do [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|
|installIntent|[installIntent](../resources/intune_shared_installintent.md)|A tentativa de instalação do livro eletrônico. Herdado do [managedEBookAssignment](../resources/intune_books_managedebookassignment.md). Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedEBookAssignment",
  "@odata.type": "microsoft.graph.iosVppEBookAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```



