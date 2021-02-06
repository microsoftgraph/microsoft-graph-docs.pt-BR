---
title: Tipo de recurso accessReviewRecurrenceSettings
description: Especifica que a revisão de acesso recorre a intervalos regulares.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 208d3e8f8c73c8de98a34aadbd616dc9f268925c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136637"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="96651-103">Tipo de recurso accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="96651-103">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="96651-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96651-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96651-105">O tipo de recurso **accessReviewRecurrenceSettings** é usado no recurso [accessReviewSettings](accessreviewsettings.md) e especifica que a revisão de acesso recorre a intervalos regulares.</span><span class="sxs-lookup"><span data-stu-id="96651-105">The **accessReviewRecurrenceSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies that the access review recurs at regular intervals.</span></span>

## <a name="properties"></a><span data-ttu-id="96651-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96651-106">Properties</span></span>

| <span data-ttu-id="96651-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96651-107">Property</span></span> | <span data-ttu-id="96651-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="96651-108">Type</span></span> | <span data-ttu-id="96651-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="96651-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="96651-110">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="96651-110">recurrenceType</span></span> | <span data-ttu-id="96651-111">String</span><span class="sxs-lookup"><span data-stu-id="96651-111">String</span></span> | <span data-ttu-id="96651-112">O intervalo de recorrência.</span><span class="sxs-lookup"><span data-stu-id="96651-112">The recurrence interval.</span></span> <span data-ttu-id="96651-113">Vaules possíveis: `onetime` `weekly` , , ou `monthly` `quarterly` `halfyearly` `annual` .</span><span class="sxs-lookup"><span data-stu-id="96651-113">Possible vaules: `onetime`, `weekly`, `monthly`, `quarterly`, `halfyearly` or `annual`.</span></span>                                                                   |
| <span data-ttu-id="96651-114">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="96651-114">recurrenceEndType</span></span> | <span data-ttu-id="96651-115">String</span><span class="sxs-lookup"><span data-stu-id="96651-115">String</span></span> | <span data-ttu-id="96651-116">Como termina a recorrência.</span><span class="sxs-lookup"><span data-stu-id="96651-116">How the recurrence ends.</span></span> <span data-ttu-id="96651-117">Valores possíveis: `never` `endBy` , , ou `occurrences` `recurrenceCount` .</span><span class="sxs-lookup"><span data-stu-id="96651-117">Possible values: `never`, `endBy`, `occurrences`, or `recurrenceCount`.</span></span> <span data-ttu-id="96651-118">Se `never` for, não haverá fim explícito da série de recorrência.</span><span class="sxs-lookup"><span data-stu-id="96651-118">If it is `never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="96651-119">Se `endBy` for, a recorrência terminará em uma determinada data.</span><span class="sxs-lookup"><span data-stu-id="96651-119">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="96651-120">Se `occurrences` for, a série terminará `recurrenceCount` após a conclusão das instâncias da revisão.</span><span class="sxs-lookup"><span data-stu-id="96651-120">If it is `occurrences`, then the series ends after `recurrenceCount` instances of the review have completed.</span></span> |
| <span data-ttu-id="96651-121">durationInDays</span><span class="sxs-lookup"><span data-stu-id="96651-121">durationInDays</span></span> | <span data-ttu-id="96651-122">Int32</span><span class="sxs-lookup"><span data-stu-id="96651-122">Int32</span></span> | <span data-ttu-id="96651-123">A duração em dias para recorrência.</span><span class="sxs-lookup"><span data-stu-id="96651-123">The duration in days for recurrence.</span></span> |
| <span data-ttu-id="96651-124">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="96651-124">recurrenceCount</span></span> | <span data-ttu-id="96651-125">Int32</span><span class="sxs-lookup"><span data-stu-id="96651-125">Int32</span></span> | <span data-ttu-id="96651-126">A contagem de recorrências, se o valor de **recurrenceEndType** for , ou 0 caso `occurrences` contrário.</span><span class="sxs-lookup"><span data-stu-id="96651-126">The count of recurrences, if the value of **recurrenceEndType** is `occurrences`, or 0 otherwise.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="96651-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96651-127">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
```json
{
  "recurrenceType": "string",
  "recurrenceEndType": "string",
  "durationInDays": 1024,
  "recurrenceCount": 1024
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewRecurrenceSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
