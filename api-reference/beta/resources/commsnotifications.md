---
title: tipo de recurso de commsNotifications
description: Lista de notificações usado pelos servidores Communications para envio de notificações de vários em um único lote.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2d002b74bffe0911e2ba1fef4eed324b52ebcc49
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520589"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="f2fae-103">tipo de recurso de commsNotifications</span><span class="sxs-lookup"><span data-stu-id="f2fae-103">commsNotifications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2fae-104">Lista de notificações usado pelos servidores Communications para envio de notificações de vários em um único lote.</span><span class="sxs-lookup"><span data-stu-id="f2fae-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="f2fae-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2fae-105">Properties</span></span>

| <span data-ttu-id="f2fae-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2fae-106">Property</span></span>       | <span data-ttu-id="f2fae-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2fae-107">Type</span></span>                                                 | <span data-ttu-id="f2fae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2fae-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="f2fae-109">valor</span><span class="sxs-lookup"><span data-stu-id="f2fae-109">value</span></span>          | <span data-ttu-id="f2fae-110">coleção [commsNotification](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="f2fae-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="f2fae-111">A notificação de alteração no recurso.</span><span class="sxs-lookup"><span data-stu-id="f2fae-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f2fae-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2fae-112">JSON representation</span></span>

<span data-ttu-id="f2fae-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2fae-113">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/commsnotifications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
