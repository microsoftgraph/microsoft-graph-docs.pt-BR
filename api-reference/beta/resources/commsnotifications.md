---
title: tipo de recurso commsNotifications
description: Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8a6be0d41a95f75130796e1073750c3e90d65a9a
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006709"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="4bb80-103">tipo de recurso commsNotifications</span><span class="sxs-lookup"><span data-stu-id="4bb80-103">commsNotifications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bb80-104">Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.</span><span class="sxs-lookup"><span data-stu-id="4bb80-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="4bb80-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4bb80-105">Properties</span></span>

| <span data-ttu-id="4bb80-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bb80-106">Property</span></span>       | <span data-ttu-id="4bb80-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bb80-107">Type</span></span>                                                 | <span data-ttu-id="4bb80-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bb80-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="4bb80-109">valor</span><span class="sxs-lookup"><span data-stu-id="4bb80-109">value</span></span>          | <span data-ttu-id="4bb80-110">coleção [commsNotification](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="4bb80-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="4bb80-111">A notificação de uma alteração no recurso.</span><span class="sxs-lookup"><span data-stu-id="4bb80-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4bb80-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4bb80-112">JSON representation</span></span>

<span data-ttu-id="4bb80-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4bb80-113">The following is a JSON representation of the resource.</span></span>

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
