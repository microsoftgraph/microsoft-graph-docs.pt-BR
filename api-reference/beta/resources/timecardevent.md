---
title: Tipo de recurso timeCardEvent
description: Representa um evento de cartão de ponto específico.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a8be7d000b3d55368f7378e9b993b5015b7ef632
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786361"
---
# <a name="timecardevent-resource-type"></a><span data-ttu-id="7c429-103">Tipo de recurso timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="7c429-103">timeCardEvent resource type</span></span>

<span data-ttu-id="7c429-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c429-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c429-105">Representa um evento [timeCard](timecard.md) específico.</span><span class="sxs-lookup"><span data-stu-id="7c429-105">Represents a specific [timeCard](timecard.md) event.</span></span>

## <a name="properties"></a><span data-ttu-id="7c429-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c429-106">Properties</span></span>
|<span data-ttu-id="7c429-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c429-107">Property</span></span>               |<span data-ttu-id="7c429-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c429-108">Type</span></span>           |<span data-ttu-id="7c429-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c429-109">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="7c429-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="7c429-110">dateTime</span></span>                  |`Edm.dateTimeOffset`  |<span data-ttu-id="7c429-111">A hora em que a entrada é gravada.</span><span class="sxs-lookup"><span data-stu-id="7c429-111">The time the entry is recorded.</span></span> |
| <span data-ttu-id="7c429-112">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="7c429-112">atApprovedLocation</span></span> |`Edm.boolean `  |<span data-ttu-id="7c429-113">Indica se a entrada foi registrada no local aprovado.</span><span class="sxs-lookup"><span data-stu-id="7c429-113">Indicates whether the entry was recorded at the approved location.</span></span> |
| <span data-ttu-id="7c429-114">notes</span><span class="sxs-lookup"><span data-stu-id="7c429-114">notes</span></span>                 |[<span data-ttu-id="7c429-115">itemBody</span><span class="sxs-lookup"><span data-stu-id="7c429-115">itemBody</span></span>](itembody.md)  | <span data-ttu-id="7c429-116">Observações sobre **o timeCardEvent**.</span><span class="sxs-lookup"><span data-stu-id="7c429-116">Notes about the **timeCardEvent**.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7c429-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c429-117">JSON representation</span></span>

<span data-ttu-id="7c429-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c429-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardEvent"
}-->
```json
{
   "atApprovedLocation":true,
   "notes":{ "@odata.type":"microsoft.graph.itemBody" }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCardEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
