---
title: tipo de recurso changeNotificationCollection
description: Representa uma coleção de notificações de assinatura enviadas ao Assinante.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: d93cbc16411d3090ba4133047ad07cd55997fec5
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681743"
---
# <a name="changenotificationcollection-resource-type"></a>tipo de recurso changeNotificationCollection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção de notificações de alteração de recursos enviadas ao Assinante.

Para obter detalhes, consulte [usar a API do Microsoft Graph para obter notificações de alteração](webhooks.md).

## <a name="methods"></a>Methods

Nenhum

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| validationTokens | collection(string) | Contém uma matriz de tokens JWT gerados pelo Microsoft Graph para o aplicativo validar a origem das notificações. O Microsoft Graph gera um único token para cada aplicativo distinto e par de locatários para os quais há um item na matriz valor. Tenha em mente que as notificações podem conter uma mistura de itens para vários aplicativos e locatários que se inscreveram usando a mesma URL de notificação. Fornecido apenas para [notificações de alteração com dados de recurso](/graph/webhooks-with-resource-data.md) opcional. |
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
