---
title: tipo de recurso accessReviewSettings
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: ''
ms.openlocfilehash: 21915811da771bd0eebdb5fb2c16df5cfbdea096
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508454"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="66fb0-102">tipo de recurso accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="66fb0-102">accessReviewSettings resource type</span></span>

<span data-ttu-id="66fb0-103">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="66fb0-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="66fb0-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66fb0-104">Properties</span></span>
|<span data-ttu-id="66fb0-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66fb0-105">Property</span></span>|<span data-ttu-id="66fb0-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="66fb0-106">Type</span></span>|<span data-ttu-id="66fb0-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="66fb0-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="66fb0-108">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="66fb0-108">mailNotificationsEnabled</span></span> | <span data-ttu-id="66fb0-109">booliano</span><span class="sxs-lookup"><span data-stu-id="66fb0-109">boolean</span></span> |  |
| <span data-ttu-id="66fb0-110">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="66fb0-110">remindersEnabled</span></span> | <span data-ttu-id="66fb0-111">booliano</span><span class="sxs-lookup"><span data-stu-id="66fb0-111">boolean</span></span> |  |
| <span data-ttu-id="66fb0-112">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="66fb0-112">justificationRequiredOnApproval</span></span> | <span data-ttu-id="66fb0-113">booliano</span><span class="sxs-lookup"><span data-stu-id="66fb0-113">boolean</span></span> |  |
| <span data-ttu-id="66fb0-114">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="66fb0-114">recurrenceSettings</span></span> | <span data-ttu-id="66fb0-115">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="66fb0-115">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="66fb0-116">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="66fb0-116">autoReviewEnabled</span></span> | <span data-ttu-id="66fb0-117">booliano</span><span class="sxs-lookup"><span data-stu-id="66fb0-117">boolean</span></span> |  |
| <span data-ttu-id="66fb0-118">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="66fb0-118">activityDurationInDays</span></span> | <span data-ttu-id="66fb0-119">Int32</span><span class="sxs-lookup"><span data-stu-id="66fb0-119">Int32</span></span> |  |
| <span data-ttu-id="66fb0-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="66fb0-120">autoReviewSettings</span></span> | <span data-ttu-id="66fb0-121">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="66fb0-121">autoReviewSettings</span></span> |  |
| <span data-ttu-id="66fb0-122">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="66fb0-122">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="66fb0-123">booliano</span><span class="sxs-lookup"><span data-stu-id="66fb0-123">boolean</span></span> |  |
| <span data-ttu-id="66fb0-124">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="66fb0-124">accessRecommendationsEnabled</span></span> | <span data-ttu-id="66fb0-125">booliano</span><span class="sxs-lookup"><span data-stu-id="66fb0-125">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="66fb0-126">Relações</span><span class="sxs-lookup"><span data-stu-id="66fb0-126">Relationships</span></span>
<span data-ttu-id="66fb0-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66fb0-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66fb0-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66fb0-128">JSON Representation</span></span>
<span data-ttu-id="66fb0-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66fb0-129">Here is a JSON representation of the resource.</span></span>
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



