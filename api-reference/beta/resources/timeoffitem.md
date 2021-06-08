---
title: Tipo de recurso timeOffItem
description: Representa uma versão do timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8fbe535fcbc63f94a50e65c62c694ffaac1a9aed
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786079"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="8d8b6-103">Tipo de recurso timeOffItem</span><span class="sxs-lookup"><span data-stu-id="8d8b6-103">timeOffItem resource type</span></span>

<span data-ttu-id="8d8b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d8b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d8b6-105">Representa uma versão do [timeOff](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="8d8b6-105">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8d8b6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d8b6-106">Properties</span></span>
| <span data-ttu-id="8d8b6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d8b6-107">Property</span></span>                         | <span data-ttu-id="8d8b6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d8b6-108">Type</span></span>                    | <span data-ttu-id="8d8b6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d8b6-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="8d8b6-110">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="8d8b6-110">timeOffReasonId</span></span>               | <span data-ttu-id="8d8b6-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d8b6-111">string</span></span>                  | <span data-ttu-id="8d8b6-112">ID do `timeOffReason` for this **timeOffItem**.</span><span class="sxs-lookup"><span data-stu-id="8d8b6-112">ID of the `timeOffReason` for this **timeOffItem**.</span></span> <span data-ttu-id="8d8b6-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d8b6-113">Required.</span></span>     |
| <span data-ttu-id="8d8b6-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8d8b6-114">startDateTime</span></span>               | <span data-ttu-id="8d8b6-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d8b6-115">DateTimeOffset</span></span>                  | <span data-ttu-id="8d8b6-116">A data e a hora de início **do timeOffItem**.</span><span class="sxs-lookup"><span data-stu-id="8d8b6-116">The start date and time for the **timeOffItem**.</span></span> <span data-ttu-id="8d8b6-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d8b6-117">Required.</span></span> <span data-ttu-id="8d8b6-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8d8b6-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8d8b6-119">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8d8b6-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="8d8b6-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8d8b6-120">endDateTime</span></span>               | <span data-ttu-id="8d8b6-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d8b6-121">DateTimeOffset</span></span>                  | <span data-ttu-id="8d8b6-122">A data e a hora de término **do timeOffItem**.</span><span class="sxs-lookup"><span data-stu-id="8d8b6-122">The end date and time for the **timeOffItem**.</span></span> <span data-ttu-id="8d8b6-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d8b6-123">Required.</span></span> <span data-ttu-id="8d8b6-124">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8d8b6-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8d8b6-125">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8d8b6-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="8d8b6-126">tema</span><span class="sxs-lookup"><span data-stu-id="8d8b6-126">theme</span></span> | <span data-ttu-id="8d8b6-127">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="8d8b6-127">scheduleEntityTheme</span></span>   | <span data-ttu-id="8d8b6-128">Cores com suporte: branco; azul; verde; roxo; rosa; amarelo; cinza; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="8d8b6-128">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8d8b6-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d8b6-129">JSON representation</span></span>

<span data-ttu-id="8d8b6-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d8b6-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": {"@odata.type": "microsoft.graph.scheduleEntityTheme"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


