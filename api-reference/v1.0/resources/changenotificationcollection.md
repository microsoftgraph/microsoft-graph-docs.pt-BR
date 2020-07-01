---
title: tipo de recurso changeNotificationCollection
description: Representa uma coleção de notificações de assinatura enviadas ao Assinante.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 242ab35d95cfc35c19e6d1f37cefa33ee8bd1632
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45004767"
---
# <a name="changenotificationcollection-resource-type"></a>tipo de recurso changeNotificationCollection

Namespace: microsoft.graph

Representa uma coleção de notificações de alteração de recursos enviadas ao Assinante.

Para obter detalhes, consulte [usar a API do Microsoft Graph para obter notificações de alteração](webhooks.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| valor | coleção ([changeNotification](changenotification.md)) | O conjunto de notificações que estão sendo enviadas à URL de notificação. Obrigatório. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotificationCollection"
}-->

```json
{
  "value": [],
  "validationTokens": [
    "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
  ]
}
```

<!-- uuid: 8cc2599e-9740-4191-93fa-bc13c6f91564
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification collection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
