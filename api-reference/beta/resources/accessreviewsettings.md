---
title: tipo de recurso accessReviewSettings
description: ''
localization_priority: Normal
ms.openlocfilehash: b19db8add3143f02f51cc0ef9d38d483d54438e1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348334"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="27862-102">tipo de recurso accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="27862-102">accessReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="27862-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27862-103">Properties</span></span>
|<span data-ttu-id="27862-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27862-104">Property</span></span>|<span data-ttu-id="27862-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="27862-105">Type</span></span>|<span data-ttu-id="27862-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="27862-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="27862-107">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="27862-107">mailNotificationsEnabled</span></span> | <span data-ttu-id="27862-108">booliano</span><span class="sxs-lookup"><span data-stu-id="27862-108">boolean</span></span> |  |
| <span data-ttu-id="27862-109">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="27862-109">remindersEnabled</span></span> | <span data-ttu-id="27862-110">booliano</span><span class="sxs-lookup"><span data-stu-id="27862-110">boolean</span></span> |  |
| <span data-ttu-id="27862-111">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="27862-111">justificationRequiredOnApproval</span></span> | <span data-ttu-id="27862-112">booliano</span><span class="sxs-lookup"><span data-stu-id="27862-112">boolean</span></span> |  |
| <span data-ttu-id="27862-113">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="27862-113">recurrenceSettings</span></span> | <span data-ttu-id="27862-114">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="27862-114">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="27862-115">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="27862-115">autoReviewEnabled</span></span> | <span data-ttu-id="27862-116">booliano</span><span class="sxs-lookup"><span data-stu-id="27862-116">boolean</span></span> |  |
| <span data-ttu-id="27862-117">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="27862-117">activityDurationInDays</span></span> | <span data-ttu-id="27862-118">Int32</span><span class="sxs-lookup"><span data-stu-id="27862-118">Int32</span></span> |  |
| <span data-ttu-id="27862-119">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="27862-119">autoReviewSettings</span></span> | <span data-ttu-id="27862-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="27862-120">autoReviewSettings</span></span> |  |
| <span data-ttu-id="27862-121">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="27862-121">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="27862-122">booliano</span><span class="sxs-lookup"><span data-stu-id="27862-122">boolean</span></span> |  |
| <span data-ttu-id="27862-123">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="27862-123">accessRecommendationsEnabled</span></span> | <span data-ttu-id="27862-124">booliano</span><span class="sxs-lookup"><span data-stu-id="27862-124">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="27862-125">Relações</span><span class="sxs-lookup"><span data-stu-id="27862-125">Relationships</span></span>
<span data-ttu-id="27862-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27862-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="27862-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27862-127">JSON Representation</span></span>
<span data-ttu-id="27862-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27862-128">Here is a JSON representation of the resource.</span></span>
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



