---
title: Tipo de recurso activateService
description: Representa um serviço a ser ativado.
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a1ab2112406d0049df002327be784c46b7e879e6
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109052"
---
# <a name="activateservice-resource-type"></a>Tipo de recurso activateService

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um serviço a ser ativado.

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo         | Descrição                           |
| ----------------- | ------------ | ------------------------------------- |
| service| Cadeia de caracteres | O nome do serviço a ser ativado. |
| servicePlanId | GUID | O identificador de plano do plano de serviço a ser ativado. |
| skuId | GUID | O identificador SKU do plano de serviço. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activateService"
}-->

```json
{
    "service": "string",
    "skuId": "guid",
    "servicePlanId": "guid"
}

```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "activateService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
