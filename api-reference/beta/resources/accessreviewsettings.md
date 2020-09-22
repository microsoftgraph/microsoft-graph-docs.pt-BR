---
title: tipo de recurso accessReviewSettings
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 201f0c0ac11a0e26174661aa4d8a63baf23f7f3c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024560"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="d62d1-102">tipo de recurso accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="d62d1-102">accessReviewSettings resource type</span></span>

<span data-ttu-id="d62d1-103">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d62d1-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="d62d1-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d62d1-104">Properties</span></span>
|<span data-ttu-id="d62d1-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d62d1-105">Property</span></span>|<span data-ttu-id="d62d1-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="d62d1-106">Type</span></span>|<span data-ttu-id="d62d1-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d62d1-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="d62d1-108">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="d62d1-108">mailNotificationsEnabled</span></span> | <span data-ttu-id="d62d1-109">booliano</span><span class="sxs-lookup"><span data-stu-id="d62d1-109">boolean</span></span> |  |
| <span data-ttu-id="d62d1-110">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="d62d1-110">remindersEnabled</span></span> | <span data-ttu-id="d62d1-111">booliano</span><span class="sxs-lookup"><span data-stu-id="d62d1-111">boolean</span></span> |  |
| <span data-ttu-id="d62d1-112">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="d62d1-112">justificationRequiredOnApproval</span></span> | <span data-ttu-id="d62d1-113">booliano</span><span class="sxs-lookup"><span data-stu-id="d62d1-113">boolean</span></span> |  |
| <span data-ttu-id="d62d1-114">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="d62d1-114">recurrenceSettings</span></span> | <span data-ttu-id="d62d1-115">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="d62d1-115">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="d62d1-116">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="d62d1-116">autoReviewEnabled</span></span> | <span data-ttu-id="d62d1-117">booliano</span><span class="sxs-lookup"><span data-stu-id="d62d1-117">boolean</span></span> |  |
| <span data-ttu-id="d62d1-118">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="d62d1-118">activityDurationInDays</span></span> | <span data-ttu-id="d62d1-119">Int32</span><span class="sxs-lookup"><span data-stu-id="d62d1-119">Int32</span></span> |  |
| <span data-ttu-id="d62d1-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="d62d1-120">autoReviewSettings</span></span> | <span data-ttu-id="d62d1-121">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="d62d1-121">autoReviewSettings</span></span> |  |
| <span data-ttu-id="d62d1-122">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="d62d1-122">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="d62d1-123">booliano</span><span class="sxs-lookup"><span data-stu-id="d62d1-123">boolean</span></span> |  |
| <span data-ttu-id="d62d1-124">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="d62d1-124">accessRecommendationsEnabled</span></span> | <span data-ttu-id="d62d1-125">booliano</span><span class="sxs-lookup"><span data-stu-id="d62d1-125">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="d62d1-126">Relações</span><span class="sxs-lookup"><span data-stu-id="d62d1-126">Relationships</span></span>
<span data-ttu-id="d62d1-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d62d1-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d62d1-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d62d1-128">JSON Representation</span></span>
<span data-ttu-id="d62d1-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d62d1-129">Here is a JSON representation of the resource.</span></span>
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





