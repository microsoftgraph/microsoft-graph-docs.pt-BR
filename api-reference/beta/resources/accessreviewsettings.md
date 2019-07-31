---
title: tipo de recurso accessReviewSettings
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: ''
ms.openlocfilehash: 2c51d94b3143d9929c03093cfb1a6625d6a9e3db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974513"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="88a01-102">tipo de recurso accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="88a01-102">accessReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="88a01-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88a01-103">Properties</span></span>
|<span data-ttu-id="88a01-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88a01-104">Property</span></span>|<span data-ttu-id="88a01-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="88a01-105">Type</span></span>|<span data-ttu-id="88a01-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="88a01-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="88a01-107">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="88a01-107">mailNotificationsEnabled</span></span> | <span data-ttu-id="88a01-108">booliano</span><span class="sxs-lookup"><span data-stu-id="88a01-108">boolean</span></span> |  |
| <span data-ttu-id="88a01-109">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="88a01-109">remindersEnabled</span></span> | <span data-ttu-id="88a01-110">booliano</span><span class="sxs-lookup"><span data-stu-id="88a01-110">boolean</span></span> |  |
| <span data-ttu-id="88a01-111">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="88a01-111">justificationRequiredOnApproval</span></span> | <span data-ttu-id="88a01-112">booliano</span><span class="sxs-lookup"><span data-stu-id="88a01-112">boolean</span></span> |  |
| <span data-ttu-id="88a01-113">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="88a01-113">recurrenceSettings</span></span> | <span data-ttu-id="88a01-114">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="88a01-114">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="88a01-115">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="88a01-115">autoReviewEnabled</span></span> | <span data-ttu-id="88a01-116">booliano</span><span class="sxs-lookup"><span data-stu-id="88a01-116">boolean</span></span> |  |
| <span data-ttu-id="88a01-117">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="88a01-117">activityDurationInDays</span></span> | <span data-ttu-id="88a01-118">Int32</span><span class="sxs-lookup"><span data-stu-id="88a01-118">Int32</span></span> |  |
| <span data-ttu-id="88a01-119">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="88a01-119">autoReviewSettings</span></span> | <span data-ttu-id="88a01-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="88a01-120">autoReviewSettings</span></span> |  |
| <span data-ttu-id="88a01-121">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="88a01-121">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="88a01-122">booliano</span><span class="sxs-lookup"><span data-stu-id="88a01-122">boolean</span></span> |  |
| <span data-ttu-id="88a01-123">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="88a01-123">accessRecommendationsEnabled</span></span> | <span data-ttu-id="88a01-124">booliano</span><span class="sxs-lookup"><span data-stu-id="88a01-124">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="88a01-125">Relações</span><span class="sxs-lookup"><span data-stu-id="88a01-125">Relationships</span></span>
<span data-ttu-id="88a01-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88a01-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="88a01-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88a01-127">JSON Representation</span></span>
<span data-ttu-id="88a01-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88a01-128">Here is a JSON representation of the resource.</span></span>
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



