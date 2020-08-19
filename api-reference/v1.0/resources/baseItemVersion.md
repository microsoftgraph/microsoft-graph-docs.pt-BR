---
title: Tipo de recurso BaseItemVersion
description: O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cc432af84b67e1781be4193a3e8d2bba29ff67a7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808288"
---
# <a name="baseitemversion-resource-type"></a>Tipo de recurso BaseItemVersion

Namespace: microsoft.graph

O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.


## <a name="json-representation"></a>Representação JSON

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a>Propriedades

|      Nome da propriedade       |                         Tipo                         |                               Descrição                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | A ID da versão. Somente leitura.                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | Identidade do usuário que modificou a versão pela última vez. Somente leitura.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Data e hora em que a versão foi modificada pela última vez. Somente leitura.                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | Indica o status de publicação desta versão específica. Somente leitura. |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
