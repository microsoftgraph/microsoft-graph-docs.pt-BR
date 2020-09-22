---
title: tipo de recurso commsNotifications
description: Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 750c0d0a19e4ec8bbf99a95235573d67d87701ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033948"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="717dc-103">tipo de recurso commsNotifications</span><span class="sxs-lookup"><span data-stu-id="717dc-103">commsNotifications resource type</span></span>

<span data-ttu-id="717dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="717dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="717dc-105">Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.</span><span class="sxs-lookup"><span data-stu-id="717dc-105">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="717dc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="717dc-106">Properties</span></span>

| <span data-ttu-id="717dc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="717dc-107">Property</span></span>       | <span data-ttu-id="717dc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="717dc-108">Type</span></span>                                                 | <span data-ttu-id="717dc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="717dc-109">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="717dc-110">valor</span><span class="sxs-lookup"><span data-stu-id="717dc-110">value</span></span>          | <span data-ttu-id="717dc-111">coleção [commsNotification](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="717dc-111">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="717dc-112">A notificação de uma alteração no recurso.</span><span class="sxs-lookup"><span data-stu-id="717dc-112">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="717dc-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="717dc-113">JSON representation</span></span>

<span data-ttu-id="717dc-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="717dc-114">The following is a JSON representation of the resource.</span></span>

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


