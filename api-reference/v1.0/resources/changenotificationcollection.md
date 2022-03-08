---
title: Tipo de recurso changeNotificationCollection
description: Representa uma coleção de notificações de assinatura enviadas ao assinante.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 74af713c082cb8070b2329785647274c29c259bb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335392"
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
| validationTokens | collection(string) | Contém uma matriz de tokens JWT gerados pela Microsoft Graph para o aplicativo validar a origem das notificações. O Microsoft Graph gera um único token para cada par de aplicativos e locatários distintos para um item se ele existir na matriz de valores. Lembre-se de que as notificações podem conter uma combinação de itens para vários aplicativos e locatários que assinaram usando a mesma URL de notificação. Fornecido apenas para [notificações de alteração com dados de recurso](/graph/webhooks-with-resource-data.md) Opcional. |
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
``` json
{
  "@odata.type": "#microsoft.graph.changeNotificationCollection",
  "validationTokens": [
    "String"
  ],
  "value": [
    {
      "@odata.type": "microsoft.graph.changeNotification"
    }
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

