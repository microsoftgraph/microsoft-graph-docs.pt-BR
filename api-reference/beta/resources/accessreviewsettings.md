---
title: tipo de recurso accessReviewSettings
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 978b8f80b6a357ffeb2efced005e395787fedabf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457092"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="179b8-102">tipo de recurso accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="179b8-102">accessReviewSettings resource type</span></span>

<span data-ttu-id="179b8-103">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="179b8-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="179b8-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="179b8-104">Properties</span></span>
|<span data-ttu-id="179b8-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="179b8-105">Property</span></span>|<span data-ttu-id="179b8-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="179b8-106">Type</span></span>|<span data-ttu-id="179b8-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="179b8-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="179b8-108">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="179b8-108">mailNotificationsEnabled</span></span> | <span data-ttu-id="179b8-109">booliano</span><span class="sxs-lookup"><span data-stu-id="179b8-109">boolean</span></span> |  |
| <span data-ttu-id="179b8-110">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="179b8-110">remindersEnabled</span></span> | <span data-ttu-id="179b8-111">booliano</span><span class="sxs-lookup"><span data-stu-id="179b8-111">boolean</span></span> |  |
| <span data-ttu-id="179b8-112">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="179b8-112">justificationRequiredOnApproval</span></span> | <span data-ttu-id="179b8-113">booliano</span><span class="sxs-lookup"><span data-stu-id="179b8-113">boolean</span></span> |  |
| <span data-ttu-id="179b8-114">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="179b8-114">recurrenceSettings</span></span> | <span data-ttu-id="179b8-115">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="179b8-115">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="179b8-116">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="179b8-116">autoReviewEnabled</span></span> | <span data-ttu-id="179b8-117">booliano</span><span class="sxs-lookup"><span data-stu-id="179b8-117">boolean</span></span> |  |
| <span data-ttu-id="179b8-118">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="179b8-118">activityDurationInDays</span></span> | <span data-ttu-id="179b8-119">Int32</span><span class="sxs-lookup"><span data-stu-id="179b8-119">Int32</span></span> |  |
| <span data-ttu-id="179b8-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="179b8-120">autoReviewSettings</span></span> | <span data-ttu-id="179b8-121">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="179b8-121">autoReviewSettings</span></span> |  |
| <span data-ttu-id="179b8-122">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="179b8-122">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="179b8-123">booliano</span><span class="sxs-lookup"><span data-stu-id="179b8-123">boolean</span></span> |  |
| <span data-ttu-id="179b8-124">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="179b8-124">accessRecommendationsEnabled</span></span> | <span data-ttu-id="179b8-125">booliano</span><span class="sxs-lookup"><span data-stu-id="179b8-125">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="179b8-126">Relações</span><span class="sxs-lookup"><span data-stu-id="179b8-126">Relationships</span></span>
<span data-ttu-id="179b8-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="179b8-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="179b8-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="179b8-128">JSON Representation</span></span>
<span data-ttu-id="179b8-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="179b8-129">Here is a JSON representation of the resource.</span></span>
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



