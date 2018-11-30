---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
ms.openlocfilehash: 28788090ccda113d6f4cd669e89777be84e6c2d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005640"
---
# <a name="sharepointids-resource-type"></a>Tipo de recurso SharePointIds

O recurso **SharePointIds** agrupa os vários identificadores de um item armazenado em um site do SharePoint ou no OneDrive for Business em uma única estrutura.

**Observação:** itens retornados do OneDrive pessoal não incluirão uma faceta **SharePointIds**.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "webId": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo         | Descrição
|:-----------------|:-------------|:-------------------------------------------
| listId           | string       | O identificador exclusivo (guid) para a lista do item no SharePoint.
| listItemId       | string       | Um identificador inteiro para o item na lista contida.
| listItemUniqueId | string       | O identificador exclusivo (guid) do item dentro do OneDrive for Business ou de um site do SharePoint.
| siteId           | string       | O identificador exclusivo (guid) do conjunto de sites do item (SPSite).
| siteUrl          | string (url) | A URL do SharePoint do site que contém o item.
| webId            | string       | O identificador exclusivo (guid) do site do item (SPWeb).

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
