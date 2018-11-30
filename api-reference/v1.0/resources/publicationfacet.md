---
title: Tipo de recurso PublicationFacet
description: O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso driveItemVersion ou driveItem.
ms.openlocfilehash: 429ec649dc9f511a4012e6790842fdd774bead8b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003999"
---
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
| **level**     | String | O estado de publicação deste documento. Pode ser `published` ou `checkout`. Somente leitura.  |
| **versionId** | String | O identificador exclusivo da versão fica visível para o chamador atual. Somente leitura.  |


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
