---
title: tipo de recurso commsNotifications
description: Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4497e2e1ba28e7f2d0b203f8f982053c5eb8ae1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341434"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="7d64e-103">tipo de recurso commsNotifications</span><span class="sxs-lookup"><span data-stu-id="7d64e-103">commsNotifications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d64e-104">Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.</span><span class="sxs-lookup"><span data-stu-id="7d64e-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="7d64e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d64e-105">Properties</span></span>

| <span data-ttu-id="7d64e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d64e-106">Property</span></span>       | <span data-ttu-id="7d64e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d64e-107">Type</span></span>                                                 | <span data-ttu-id="7d64e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d64e-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="7d64e-109">valor</span><span class="sxs-lookup"><span data-stu-id="7d64e-109">value</span></span>          | <span data-ttu-id="7d64e-110">coleção [commsNotification](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="7d64e-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="7d64e-111">A notificação de uma alteração no recurso.</span><span class="sxs-lookup"><span data-stu-id="7d64e-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7d64e-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d64e-112">JSON representation</span></span>

<span data-ttu-id="7d64e-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d64e-113">The following is a JSON representation of the resource.</span></span>

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
