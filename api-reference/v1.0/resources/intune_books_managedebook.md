# <a name="managedebook-resource-type"></a>Tipo de recurso managedEBook

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedEBooks](../api/intune_books_managedebook_list.md)|Coleção [managedEBook](../resources/intune_books_managedebook.md)|Lista propriedades e relações dos objetos [managedEBook](../resources/intune_books_managedebook.md).|
|[Obter managedEBook](../api/intune_books_managedebook_get.md)|[managedEBook](../resources/intune_books_managedebook.md)|Propriedades de leitura e relações do objeto [managedEBook](../resources/intune_books_managedebook.md).|
|[ação assign](../api/intune_books_managedebook_assign.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|displayName|Cadeia de caracteres|Nome do livro eletrônico.|
|description|Cadeia de caracteres|Descrição.|
|publisher|Cadeia de caracteres|Publicador.|
|publishedDateTime|DateTimeOffset|A data e hora em que o livro eletrônico foi publicado.|
|largeCover|[mimeContent](../resources/intune_shared_mimecontent.md)|Capa do livro.|
|createdDateTime|DateTimeOffset|A data e hora em que o livro eletrônico foi modificado pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação do livro eletrônico.|
|informationUrl|String|A URL de informações adicionais.|
|privacyInformationUrl|String|A URL da declaração de privacidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|A lista de atribuições para este livro eletrônico.|
|installSummary|[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)|Resumo de instalação do aplicativo móvel.|
|deviceStates|Coleção [deviceInstallState](../resources/intune_books_deviceinstallstate.md)|A lista de estados de instalação para este livro eletrônico.|
|userStateSummary|Coleção [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|A lista de estados de instalação para este livro eletrônico.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



