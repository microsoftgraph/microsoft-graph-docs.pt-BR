---
title: tipo de recurso de commsNotifications
description: Lista de notificações usado pelos servidores Communications para envio de notificações de vários em um único lote.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9ce629e17c85806d7e05bce99d6a62f9fa9cbff8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851496"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="f29bc-103">tipo de recurso de commsNotifications</span><span class="sxs-lookup"><span data-stu-id="f29bc-103">commsNotifications resource type</span></span>

> <span data-ttu-id="f29bc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f29bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f29bc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f29bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f29bc-106">Lista de notificações usado pelos servidores Communications para envio de notificações de vários em um único lote.</span><span class="sxs-lookup"><span data-stu-id="f29bc-106">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="f29bc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f29bc-107">Properties</span></span>

| <span data-ttu-id="f29bc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f29bc-108">Property</span></span>       | <span data-ttu-id="f29bc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f29bc-109">Type</span></span>                                                 | <span data-ttu-id="f29bc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f29bc-110">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="f29bc-111">valor</span><span class="sxs-lookup"><span data-stu-id="f29bc-111">value</span></span>          | <span data-ttu-id="f29bc-112">coleção [commsNotification](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="f29bc-112">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="f29bc-113">A notificação de alteração no recurso.</span><span class="sxs-lookup"><span data-stu-id="f29bc-113">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f29bc-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f29bc-114">JSON representation</span></span>

<span data-ttu-id="f29bc-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f29bc-115">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
