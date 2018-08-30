# <a name="publicationfacet-resource-type"></a>Tipo de recurso PublicationFacet

O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso [driveItemVersion](driveitemversion.md) ou [driveItem](driveitem.md).

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a>Propriedades

|   Propriedade    |  Tipo  | Descrição |
| :------------ | :----- | :---------- |
| **level**     | Sequência de caracteres | O estado de publicação deste documento. Pode ser `published` ou `checkout`. Somente leitura.  |
| **versionId** | Sequência de caracteres | O identificador exclusivo da versão fica visível para o chamador atual. Somente leitura.  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
