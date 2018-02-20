# <a name="iosvppebook-resource-type"></a>Tipo de recurso iosVppEBook

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma classe que contém as propriedades do livro eletrônico Vpp iOS.

Herda de [managedEBook](../resources/intune_books_managedebook.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosVppEBooks](../api/intune_books_iosvppebook_list.md)|Coleção [iosVppEBook](../resources/intune_books_iosvppebook.md)|Lista propriedades e relações dos objetos [iosVppEBook](../resources/intune_books_iosvppebook.md).|
|[Obter iosVppEBook](../api/intune_books_iosvppebook_get.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|Propriedades de leitura e relações do objeto [iosVppEBook](../resources/intune_books_iosvppebook.md).|
|[Criar iosVppEBook](../api/intune_books_iosvppebook_create.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|Cria um novo objeto [iosVppEBook](../resources/intune_books_iosvppebook.md).|
|[Excluir iosVppEBook](../api/intune_books_iosvppebook_delete.md)|Nenhum|Exclui um [iosVppEBook](../resources/intune_books_iosvppebook.md).|
|[Atualizar iosVppEBook](../api/intune_books_iosvppebook_update.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|Atualiza as propriedades de um objeto [iosVppEBook](../resources/intune_books_iosvppebook.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|displayName|Cadeia de caracteres|Nome do livro eletrônico. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|description|Cadeia de caracteres|Descrição. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|publisher|Cadeia de caracteres|Publicador. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|publishedDateTime|DateTimeOffset|A data e hora em que o livro eletrônico foi publicado. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|largeCover|[mimeContent](../resources/intune_books_mimecontent.md)|Capa do livro. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|createdDateTime|DateTimeOffset|A data e hora em que o livro eletrônico foi modificado pela última vez. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação do livro eletrônico. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|informationUrl|Cadeia de caracteres|A URL de informações adicionais. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|privacyInformationUrl|Cadeia de caracteres|A URL da declaração de privacidade. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|vppTokenId|Guid|A ID de token Vpp.|
|appleId|Cadeia de caracteres|O Apple ID associado ao token Vpp.|
|vppOrganizationName|Cadeia de caracteres|O nome da organização do token Vpp.|
|genres|Coleção de cadeias de caracteres|Gêneros.|
|idioma|Cadeia de caracteres|Idioma.|
|seller|Cadeia de caracteres|Vendedor.|
|totalLicenseCount|Int32|Contagem total de licenças.|
|usedLicenseCount|Int32|Contagem de licenças usadas.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|A lista de atribuições para este livro eletrônico. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|installSummary|[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)|Resumo de instalação do aplicativo móvel. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|deviceStates|Coleção [deviceInstallState](../resources/intune_books_deviceinstallstate.md)|A lista de estados de instalação para este livro eletrônico. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|
|userStateSummary|Coleção [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|A lista de estados de instalação para este livro eletrônico. Herdado de [managedEBook](../resources/intune_books_managedebook.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
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
  "privacyInformationUrl": "String",
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
  "appleId": "String",
  "vppOrganizationName": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "seller": "String",
  "totalLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```



