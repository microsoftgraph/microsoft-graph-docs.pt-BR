---
title: tipo de recurso accessReviewSettings
description: ''
localization_priority: Normal
ms.openlocfilehash: b19db8add3143f02f51cc0ef9d38d483d54438e1
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/20/2019
ms.locfileid: "35084065"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="c50b8-102">tipo de recurso accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="c50b8-102">accessReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="c50b8-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c50b8-103">Properties</span></span>
|<span data-ttu-id="c50b8-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c50b8-104">Property</span></span>|<span data-ttu-id="c50b8-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="c50b8-105">Type</span></span>|<span data-ttu-id="c50b8-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="c50b8-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="c50b8-107">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="c50b8-107">mailNotificationsEnabled</span></span> | <span data-ttu-id="c50b8-108">booliano</span><span class="sxs-lookup"><span data-stu-id="c50b8-108">boolean</span></span> |  |
| <span data-ttu-id="c50b8-109">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="c50b8-109">remindersEnabled</span></span> | <span data-ttu-id="c50b8-110">booliano</span><span class="sxs-lookup"><span data-stu-id="c50b8-110">boolean</span></span> |  |
| <span data-ttu-id="c50b8-111">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="c50b8-111">justificationRequiredOnApproval</span></span> | <span data-ttu-id="c50b8-112">booliano</span><span class="sxs-lookup"><span data-stu-id="c50b8-112">boolean</span></span> |  |
| <span data-ttu-id="c50b8-113">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="c50b8-113">recurrenceSettings</span></span> | <span data-ttu-id="c50b8-114">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="c50b8-114">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="c50b8-115">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="c50b8-115">autoReviewEnabled</span></span> | <span data-ttu-id="c50b8-116">booliano</span><span class="sxs-lookup"><span data-stu-id="c50b8-116">boolean</span></span> |  |
| <span data-ttu-id="c50b8-117">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="c50b8-117">activityDurationInDays</span></span> | <span data-ttu-id="c50b8-118">Int32</span><span class="sxs-lookup"><span data-stu-id="c50b8-118">Int32</span></span> |  |
| <span data-ttu-id="c50b8-119">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="c50b8-119">autoReviewSettings</span></span> | <span data-ttu-id="c50b8-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="c50b8-120">autoReviewSettings</span></span> |  |
| <span data-ttu-id="c50b8-121">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="c50b8-121">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="c50b8-122">booliano</span><span class="sxs-lookup"><span data-stu-id="c50b8-122">boolean</span></span> |  |
| <span data-ttu-id="c50b8-123">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="c50b8-123">accessRecommendationsEnabled</span></span> | <span data-ttu-id="c50b8-124">booliano</span><span class="sxs-lookup"><span data-stu-id="c50b8-124">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="c50b8-125">Relações</span><span class="sxs-lookup"><span data-stu-id="c50b8-125">Relationships</span></span>
<span data-ttu-id="c50b8-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c50b8-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c50b8-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c50b8-127">JSON Representation</span></span>
<span data-ttu-id="c50b8-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c50b8-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
``` json
{
    "mailNotificationsEnabled":"boolean",
    "remindersEnabled":"boolean",
    "justificationRequiredOnApproval":"boolean",
    "recurrenceSettings":"microsoft.graph.accessReviewRecurrenceSettings",
    "autoReviewEnabled":"boolean",
    "activityDurationInDays":"Int32",
    "autoReviewSettings":"microsoft.graph.autoReviewSettings",
    "autoApplyReviewResultsEnabled":"boolean",
    "accessRecommendationsEnabled":"boolean"
}
```



