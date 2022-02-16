---
title: Tipo de recurso activateService
description: Representa um serviço a ser ativado.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d007512113ab46b25714942f93002936c97fe083
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854547"
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
    "service": "String",
    "skuId": "GUID",
    "servicePlanId": "GUID"
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
