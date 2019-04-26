---
title: tipo de recurso directoryObjectPartnerReference
description: Representa uma referência a um objeto Directory em um locatário do parceiro. Herda de directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 658571ce406e74b78a6924ed0290ab672c791e94
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341733"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>tipo de recurso directoryObjectPartnerReference

Representa uma referência a um objeto Directory em uma organização parceira. Herda de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|description|String| Descrição do objeto retornado. Somente leitura. |
|displayName|Cadeia de caracteres| Nome do objeto de diretório que está sendo retornado, como o grupo ou o aplicativo. Somente leitura. |
|externalPartnerTenantId|Guid| O identificador de locatário para o locatário do parceiro. Somente leitura. |
|id|Cadeia de caracteres| O identificador exclusivo do recurso. Herdado de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0). Somente leitura. |
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

- [Obter objetos directory a partir de uma lista de ids](/graph/api/directoryobject-getbyids?view=graph-rest-v1.0)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
