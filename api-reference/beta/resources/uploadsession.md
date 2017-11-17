# <a name="uploadsession-resource-type"></a>Tipo de recurso UploadSession

O recurso **UploadSession** fornece informações sobre como carregar arquivos grandes no OneDrive, no OneDrive for Business ou em bibliotecas de documentos do SharePoint.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "expirationDateTime": "timestamp",
  "nextExpectedRanges": ["string"],
  "uploadUrl": "url"
}

```
## <a name="properties"></a>Propriedades


| Propriedade	             | Tipo	              |Descrição|
|:-------------------|:------------------|:----------|
| expirationDateTime | DateTimeOffset    | Data e hora em UTC em que a sessão de carregamento expirará. O arquivo completo deve ser carregado antes que esta hora de expiração seja atingida. |
| nextExpectedRanges | Coleção de cadeias de caracteres | Uma coleção de intervalos de bytes que estão ausentes do servidor para o arquivo. Estes intervalos são indexados como zero e têm o formato "início-fim" (por exemplo "0-26" para indicar os primeiros 27 bytes do arquivo). |
| uploadUrl          | String            | O ponto de extremidade de URL que aceita solicitações PUT para intervalos de bytes do arquivo. |

## <a name="additional-resources"></a>Recursos adicionais

Veja [Carregar arquivos grandes com uma sessão de carregamento](../api/item_createUploadSession.md) para obter detalhes sobre como carregar arquivos usando uma sessão de carregamento.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "uploadSession resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->