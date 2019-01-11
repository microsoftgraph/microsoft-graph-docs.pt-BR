---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: 4cb3a56b5bdb4c3e7c9fc9fe69c0b34cae134a0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805604"
---
# <a name="publicationfacet-resource-type"></a>Tipo de recurso PublicationFacet

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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
  "tocPath": "Facets/Photo"
} -->
