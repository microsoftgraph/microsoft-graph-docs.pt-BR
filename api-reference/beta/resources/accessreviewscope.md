---
title: Tipo de recurso accessReviewScope
description: 'No recurso de análises de acesso do Azure AD, o representa quais entidades serão revisadas `accessReviewScope` em uma revisão de acesso.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 04955ba6980dd94995da1610afcc1e33046e4473
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469308"
---
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="fe13b-103">Tipo de recurso accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="fe13b-103">accessReviewScope resource type</span></span>

<span data-ttu-id="fe13b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe13b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="fe13b-105">O **accessReviewScope** define quais entidades serão revisadas em [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fe13b-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="fe13b-106">É um tipo abstrato herdado por [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) e [accessReviewReviewerScope](accessreviewreviewerscope.md).</span><span class="sxs-lookup"><span data-stu-id="fe13b-106">It is an abstract type that is inherited by [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) and [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> 

<span data-ttu-id="fe13b-107">Para `scope` propriedade em um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) consulte [accessReviewQueryScope](accessreviewqueryscope.md) e [principalResourceMembershipsScope](principalresourcemembershipsscope.md).</span><span class="sxs-lookup"><span data-stu-id="fe13b-107">For `scope` property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewQueryScope](accessreviewqueryscope.md) and [principalResourceMembershipsScope](principalresourcemembershipsscope.md).</span></span>

<span data-ttu-id="fe13b-108">Para `reviewers` propriedade em um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) consulte [accessReviewReviewerScope](accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="fe13b-108">For `reviewers` property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewReviewerScope](accessreviewreviewerscope.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fe13b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe13b-109">Properties</span></span>
<span data-ttu-id="fe13b-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fe13b-110">None.</span></span>


## <a name="relationships"></a><span data-ttu-id="fe13b-111">Relações</span><span class="sxs-lookup"><span data-stu-id="fe13b-111">Relationships</span></span>
<span data-ttu-id="fe13b-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fe13b-112">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe13b-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe13b-113">JSON representation</span></span>
<span data-ttu-id="fe13b-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe13b-114">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
