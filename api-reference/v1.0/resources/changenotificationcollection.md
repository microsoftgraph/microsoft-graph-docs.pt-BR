---
title: Tipo de recurso changeNotificationCollection
description: Representa uma coleção de notificações de assinatura enviadas ao assinante.
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 62098d3099549893165d60cb55699209e4034ccc
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469317"
---
# <a name="changenotificationcollection-resource-type"></a>Tipo de recurso changeNotificationCollection

Namespace: microsoft.graph

Representa uma coleção de notificações de alteração de recurso enviadas ao assinante.

Para obter detalhes, confira [Usar a API do Microsoft Graph para receber notificações de alteração](webhooks.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| validationTokens | collection(string) | Contém uma matriz de tokens JWT gerados pelo Microsoft Graph para o aplicativo validar a origem das notificações. O Microsoft Graph gera um único token para cada par de aplicativos e locatários distintos para um item se ele existir na matriz de valores. Lembre-se de que as notificações podem conter uma combinação de itens para vários aplicativos e locatários que assinaram usando a mesma URL de notificação. Fornecido apenas para [notificações de alteração com dados de recurso](/graph/webhooks-with-resource-data.md) Opcional. |
| valor | collection([changeNotification](changenotification.md)) | O conjunto de notificações que está sendo enviado para a URL de notificação. Obrigatório. |

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

