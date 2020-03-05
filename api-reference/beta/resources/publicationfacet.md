---
author: JeremyKelley
description: O recurso publicationFacet fornece detalhes sobre o status de publicado em um recurso driveItemVersion ou driveItem.
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 46e5a8925e6f2521763bd1b1830e967a08df3abb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521310"
---
# <a name="publicationfacet-resource-type"></a>Tipo de recurso PublicationFacet

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": []
}
-->
