---
title: tipo de recurso commsNotifications
description: Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f7ff962817d6248adcd1de5748c94e975dc0e60e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507594"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="5b4bc-103">tipo de recurso commsNotifications</span><span class="sxs-lookup"><span data-stu-id="5b4bc-103">commsNotifications resource type</span></span>

<span data-ttu-id="5b4bc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5b4bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b4bc-105">Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.</span><span class="sxs-lookup"><span data-stu-id="5b4bc-105">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="5b4bc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b4bc-106">Properties</span></span>

| <span data-ttu-id="5b4bc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b4bc-107">Property</span></span>       | <span data-ttu-id="5b4bc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b4bc-108">Type</span></span>                                                 | <span data-ttu-id="5b4bc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b4bc-109">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="5b4bc-110">valor</span><span class="sxs-lookup"><span data-stu-id="5b4bc-110">value</span></span>          | <span data-ttu-id="5b4bc-111">coleção [commsNotification](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="5b4bc-111">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="5b4bc-112">A notificação de uma alteração no recurso.</span><span class="sxs-lookup"><span data-stu-id="5b4bc-112">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5b4bc-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b4bc-113">JSON representation</span></span>

<span data-ttu-id="5b4bc-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b4bc-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
