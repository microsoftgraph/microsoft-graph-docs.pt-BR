---
title: tipo de recurso accessReviewRecurrenceSettings
description: Especifica que a revisão do Access se repete em intervalos regulares.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3ca66a818059efac84903f763e6be3c8a3b5c05a
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330162"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="9f101-103">tipo de recurso accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="9f101-103">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="9f101-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f101-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f101-105">O tipo de recurso **accessReviewRecurrenceSettings** é usado no recurso [accessReviewSettings](accessreviewsettings.md) e especifica que a revisão de acesso se repete em intervalos regulares.</span><span class="sxs-lookup"><span data-stu-id="9f101-105">The **accessReviewRecurrenceSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies that the access review recurs at regular intervals.</span></span>

## <a name="properties"></a><span data-ttu-id="9f101-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f101-106">Properties</span></span>

| <span data-ttu-id="9f101-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f101-107">Property</span></span> | <span data-ttu-id="9f101-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f101-108">Type</span></span> | <span data-ttu-id="9f101-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f101-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="9f101-110">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="9f101-110">recurrenceType</span></span> | <span data-ttu-id="9f101-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f101-111">String</span></span> | <span data-ttu-id="9f101-112">O intervalo de recorrência.</span><span class="sxs-lookup"><span data-stu-id="9f101-112">The recurrence interval.</span></span> <span data-ttu-id="9f101-113">Possível vaules: `onetime` , `weekly` , `monthly` , `quarterly` `halfyearly` ou `annual` .</span><span class="sxs-lookup"><span data-stu-id="9f101-113">Possible vaules: `onetime`, `weekly`, `monthly`, `quarterly`, `halfyearly` or `annual`.</span></span>                                                                   |
| <span data-ttu-id="9f101-114">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="9f101-114">recurrenceEndType</span></span> | <span data-ttu-id="9f101-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f101-115">String</span></span> | <span data-ttu-id="9f101-116">Como a recorrência termina.</span><span class="sxs-lookup"><span data-stu-id="9f101-116">How the recurrence ends.</span></span> <span data-ttu-id="9f101-117">Valores possíveis: `never` , `endBy` , `occurrences` ou `recurrenceCount` .</span><span class="sxs-lookup"><span data-stu-id="9f101-117">Possible values: `never`, `endBy`, `occurrences`, or `recurrenceCount`.</span></span> <span data-ttu-id="9f101-118">Se for `never` , não haverá uma extremidade explícita da série de recorrência.</span><span class="sxs-lookup"><span data-stu-id="9f101-118">If it is `never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="9f101-119">Se for `endBy` , a recorrência terminará em uma determinada data.</span><span class="sxs-lookup"><span data-stu-id="9f101-119">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="9f101-120">Se for `occurrences` , a série terminará após a `recurrenceCount` conclusão das instâncias da revisão.</span><span class="sxs-lookup"><span data-stu-id="9f101-120">If it is `occurrences`, then the series ends after `recurrenceCount` instances of the review have completed.</span></span> |
| <span data-ttu-id="9f101-121">durationInDays</span><span class="sxs-lookup"><span data-stu-id="9f101-121">durationInDays</span></span> | <span data-ttu-id="9f101-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9f101-122">Int32</span></span> | <span data-ttu-id="9f101-123">A duração em dias da recorrência.</span><span class="sxs-lookup"><span data-stu-id="9f101-123">The duration in days for recurrence.</span></span> |
| <span data-ttu-id="9f101-124">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="9f101-124">recurrenceCount</span></span> | <span data-ttu-id="9f101-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9f101-125">Int32</span></span> | <span data-ttu-id="9f101-126">A contagem de recorrências, se o valor de **recurrenceEndType** for `occurrences` , ou 0 caso contrário.</span><span class="sxs-lookup"><span data-stu-id="9f101-126">The count of recurrences, if the value of **recurrenceEndType** is `occurrences`, or 0 otherwise.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f101-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f101-127">JSON representation</span></span>

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