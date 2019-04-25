---
title: tipo de recurso directoryObjectPartnerReference
description: Representa uma referência a um objeto Directory em um locatário do parceiro. Herda de directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a031586d1f92bf2b8b331e9b71058211b4617382
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543270"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>tipo de recurso directoryObjectPartnerReference

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma referência a um objeto Directory em uma organização parceira. Herda de [directoryObject](directoryobject.md?view=graph-rest-beta).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|description|String| Descrição do objeto retornado. Somente leitura. |
|displayName|Cadeia de caracteres| Nome do objeto de diretório que está sendo retornado, como o grupo ou o aplicativo. Somente leitura. |
|externalPartnerTenantId|Guid| O identificador de locatário para o locatário do parceiro. Somente leitura. |
|id|Cadeia de caracteres| O identificador exclusivo do recurso. Herdado de [directoryObject](directoryobject.md?view=graph-rest-beta). Somente leitura. |
|objectType|String| O tipo do objeto referenciado no locatário do parceiro. Somente leitura. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "string ",
  "displayName": "string",
  "externalPartnerTenantId": "string (identifier)",
  "id": "string (identifier)",
  "objectType": "string"
}
```

## <a name="see-also"></a>Confira também

- [Obter objetos directory a partir de uma lista de ids](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobjectpartnerreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
