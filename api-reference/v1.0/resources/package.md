---
author: JeremyKelley title: package ms.localizationpriority: medium description: "Indicates that a driveItem is the top-level item in a "package" or a collection of items that should be treated as a collection instead of individual items."
ms.prod: arquivos doc_type: resourcePageType
---

# <a name="package-resource-type"></a>tipo de recurso de pacote

Namespace: microsoft.graph

O **recurso** de pacote indica que um **driveItem** é o item de nível superior em um "pacote" ou uma coleção de itens que devem ser tratados como uma coleção em vez de itens individuais.

Um exemplo de um pacote é um bloco de anotações do OneNote. Embora o bloco de anotações seja composto de arquivos e pastas que representam o conteúdo do bloco de anotações, o item de nível superior que representa o bloco de anotações tem uma faceta **package** para indicar aos clientes que se trata de uma coleção de dados que deve ser tratada de forma especial.

**driveItems** com **a faceta** do pacote não incluem  uma pasta **ou faceta** de arquivo, mas são conceitualmente semelhantes a um item com uma faceta **de** pasta.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| type          | string | Uma cadeia de caracteres que indica o tipo de pacote. Embora `oneNote` seja o único valor definido atualmente, você deve esperar que outros tipos de pacote sejam retornados e lidar com eles da forma apropriada. |

## <a name="remarks"></a>Comentários 

Para obter mais informações sobre as facetas em um DriveItem, consulte [driveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->

