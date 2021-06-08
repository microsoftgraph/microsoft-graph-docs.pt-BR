---
title: Tipo de recurso timeCardBreak
description: Representa uma quebra de cartão de ponto específica.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 509667ec1fad41f956ee5ee6d6a4371b8d17fc2e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786360"
---
# <a name="timecardbreak-resource-type"></a><span data-ttu-id="7db12-103">Tipo de recurso timeCardBreak</span><span class="sxs-lookup"><span data-stu-id="7db12-103">timeCardBreak resource type</span></span>

<span data-ttu-id="7db12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7db12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7db12-105">Representa uma quebra de cartão de ponto [específica.](timecard.md)</span><span class="sxs-lookup"><span data-stu-id="7db12-105">Represents a specific [timeCard](timecard.md) break.</span></span>

## <a name="properties"></a><span data-ttu-id="7db12-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7db12-106">Properties</span></span>
|<span data-ttu-id="7db12-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7db12-107">Property</span></span>               |<span data-ttu-id="7db12-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7db12-108">Type</span></span>           |<span data-ttu-id="7db12-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7db12-109">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="7db12-110">breakId</span><span class="sxs-lookup"><span data-stu-id="7db12-110">breakId</span></span>                   |`Edm.string`  |<span data-ttu-id="7db12-111">ID do **timeCardBreak**.</span><span class="sxs-lookup"><span data-stu-id="7db12-111">ID of the **timeCardBreak**.</span></span>|
| <span data-ttu-id="7db12-112">iniciar</span><span class="sxs-lookup"><span data-stu-id="7db12-112">start</span></span>                 |[<span data-ttu-id="7db12-113">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="7db12-113">timeCardEvent</span></span>](timecardevent.md)    | <span data-ttu-id="7db12-114">O evento de início do **timeCardBreak**.</span><span class="sxs-lookup"><span data-stu-id="7db12-114">The start event of the **timeCardBreak**.</span></span>|
| <span data-ttu-id="7db12-115">end</span><span class="sxs-lookup"><span data-stu-id="7db12-115">end</span></span>                   |[<span data-ttu-id="7db12-116">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="7db12-116">timeCardEvent</span></span>](timecardevent.md)    | <span data-ttu-id="7db12-117">O evento de início do **timeCardBreak**.</span><span class="sxs-lookup"><span data-stu-id="7db12-117">The start event of the **timeCardBreak**.</span></span>|
| <span data-ttu-id="7db12-118">notes</span><span class="sxs-lookup"><span data-stu-id="7db12-118">notes</span></span>                 |[<span data-ttu-id="7db12-119">itemBody</span><span class="sxs-lookup"><span data-stu-id="7db12-119">itemBody</span></span>](itembody.md)  | <span data-ttu-id="7db12-120">Observações sobre **o timeCardBreak**.</span><span class="sxs-lookup"><span data-stu-id="7db12-120">Notes about the **timeCardBreak**.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7db12-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7db12-121">JSON representation</span></span>

<span data-ttu-id="7db12-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7db12-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardBreak"
}-->
```json
{
    "breakId":"string",
    "notes":{
        "content": "string",
        "contentType": "string"
    },
    "start":{
        "dateTime":"String (timestamp)",
        "atApprovedLocation":true,
        "notes":{
            "content": "string",
            "contentType": "text"
        },
    },
    "end":null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCardBreak resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
