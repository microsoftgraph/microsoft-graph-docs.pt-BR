---
title: tipo de recurso directoryObjectPartnerReference
description: Representa uma referência a um objeto Directory em um locatário do parceiro. Herda do directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cda40de50710c971970d64853b33eebbde8865a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091765"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>tipo de recurso directoryObjectPartnerReference

Namespace: microsoft.graph

Representa uma referência a um objeto Directory em uma organização parceira. Herda de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|description|Cadeia de caracteres| Descrição do objeto retornado. Somente leitura. |
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

