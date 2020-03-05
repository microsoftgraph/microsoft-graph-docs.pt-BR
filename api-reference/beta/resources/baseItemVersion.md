---
author: JeremyKelley
description: O recurso baseItemVersion representa uma versão anterior de um item ou de uma entidade.
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 47865e388616763b60ce3cd45195bf9919c7acf2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508035"
---
# <a name="baseitemversion-resource-type"></a>Tipo de recurso BaseItemVersion

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.


## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.baseItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
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


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": []
}
-->
