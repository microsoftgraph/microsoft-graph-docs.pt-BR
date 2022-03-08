---
title: Tipo de recurso activateService
description: Representa um serviço a ser ativado.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6645da51b2f292d787c277096465b0a4b65e0347
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63331864"
---
# <a name="activateservice-resource-type"></a>Tipo de recurso activateService

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um serviço a ser ativado.

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo         | Descrição                           |
| ----------------- | ------------ | ------------------------------------- |
| service| Cadeia de caracteres | O nome do serviço a ser ativado. |
| servicePlanId | Guid | O identificador de plano do plano de serviço a ser ativado. |
| skuId | Guid | O identificador SKU do plano de serviço. |

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
    "service": "String",
    "skuId": "Guid",
    "servicePlanId": "Guid"
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
