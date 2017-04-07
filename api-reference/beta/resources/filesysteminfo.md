# <a name="filesysteminfo-resource-type"></a>tipo de recurso FileSystemInfo

O recurso **FileSystemInfo** contém propriedades que são relatadas pelo sistema de arquivos local do dispositivo para a versão local de um item. Esta faceta pode ser usada para especificar a data da última modificação ou a data de criação do item como estava no dispositivo local.

**Observação:** A propriedade **FileSystemInfo** não está disponível para DriveItems no SharePoint ou no OneDrive for Business.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSystemInfo"
}-->

```json
{
  "createdDateTime": "datetime",
  "lastModifiedDateTime": "datetime"
}
```

## <a name="properties"></a>Propriedades

| Propriedade	                 | Tipo	           | Descrição                                                   |
|:-------------------------|:---------------|:--------------------------------------------------------------|
| **createdDateTime**      | DateTimeOffset | A data e a hora UTC em que o arquivo foi criado em um cliente.       |
| **lastModifiedDateTime** | DateTimeOffset | A data e hora UTC em que o arquivo foi modificado pela última vez em um cliente. |

## <a name="notes"></a>Observações

Os valores para **createdDateTime** e **lastModifiedDateTime** variam em relação às mesmas propriedades no recurso [DriveItem](driveitem.md). Os valores no recurso DriveItem são a data e a hora de criação e modificação, como visto do serviço. Os valores armazenados no recurso **FileSystemInfo** são fornecidos pelo cliente.

Por exemplo, se um arquivo foi criado no dispositivo na segunda-feira, mas não foi carregado no serviço até terça-feira, o cliente que carrega o arquivo deve gravar a faceta `fileSystemInfo` para incluir a data de criação na segunda-feira. Quando os metadados de item forem recuperados, a data de criação do item refletirá terça-feira, mas a faceta `fileSystemInfo` mostrará a data de criação original na segunda-feira.

Estas propriedades são somente leitura. Se estiver carregando um arquivo e souber os valores do cliente local para estes campos, você deverá incluí-los na solicitação.

Se o conteúdo do arquivo for atualizado e estas propriedades não forem fornecidas, **lastModifiedDateTime** será redefinido automaticamente como a hora atual.

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSystemInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
