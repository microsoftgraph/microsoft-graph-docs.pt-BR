---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade **prepaidUnits** da entidade subscribedSku é do tipo **licenseUnitsDetail**.
localization_priority: Normal
author: 'michaelcurnutt '
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: af038eab4589fcaf98743b34cdc1ce6f43b09bd7b511d1f3a05862862155fa32
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54135061"
---
# <a name="licenseunitsdetail-resource-type"></a>Tipo de recurso licenseUnitsDetail

Namespace: microsoft.graph

A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**. Para obter mais informações sobre os estados de progressão de uma assinatura, consulte [E se minha assinatura expirar?](/microsoft-365/commerce/subscriptions/what-if-my-subscription-expires?view=o365-worldwide)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:-------------|:-----|:----------|
|enabled|Int32| O número de unidades habilitadas para a assinatura ativa do SKU do serviço.  |
|suspended|Int32| O número de unidades suspensas porque a assinatura do SKU do serviço foi cancelada. As unidades não podem ser atribuídas, mas ainda podem ser reativadas antes de serem excluídas. |
|warning|Int32| O número de unidades que estão em status de aviso. Quando a assinatura do SKU do serviço expirou, o cliente tem um período de carência para renovar sua assinatura antes de ser cancelada (movida para um **estado suspenso).**  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

