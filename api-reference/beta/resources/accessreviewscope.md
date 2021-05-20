---
title: Tipo de recurso accessReviewScope
description: 'No recurso de análises de acesso do Azure AD, o representa quais entidades serão revisadas `accessReviewScope` em uma revisão de acesso.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0888aa8666f3335a42dc6686531f88fd0f3325ed
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579722"
---
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="015fd-103">Tipo de recurso accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="015fd-103">accessReviewScope resource type</span></span>

<span data-ttu-id="015fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="015fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="015fd-105">O **accessReviewScope** define quais entidades serão revisadas em [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="015fd-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="015fd-106">É um tipo abstrato herdado por [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) e [accessReviewReviewerScope](accessreviewreviewerscope.md).</span><span class="sxs-lookup"><span data-stu-id="015fd-106">It is an abstract type that is inherited by [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) and [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> 

<span data-ttu-id="015fd-107">Para **a propriedade scope** em um [accessReviewScheduleDefinition,](accessreviewscheduledefinition.md) consulte [accessReviewQueryScope](accessreviewqueryscope.md) e [principalResourceMembershipsScope](principalresourcemembershipsscope.md).</span><span class="sxs-lookup"><span data-stu-id="015fd-107">For **scope** property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewQueryScope](accessreviewqueryscope.md) and [principalResourceMembershipsScope](principalresourcemembershipsscope.md).</span></span>

<span data-ttu-id="015fd-108">Para **a propriedade reviewers** em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md) consulte [accessReviewReviewerScope](accessreviewreviewerscope.md).</span><span class="sxs-lookup"><span data-stu-id="015fd-108">For **reviewers** property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span>

<span data-ttu-id="015fd-109">A especificação do tipo  OData no escopo é altamente recomendada para todos os tipos, mas necessária para [o principalResourceMembershipsScope](principalresourcemembershipsscope.md) e [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="015fd-109">Specifying the OData type in the **scope** is highly recommended for all types but required for [principalResourceMembershipsScope](principalresourcemembershipsscope.md) and [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="015fd-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="015fd-110">Properties</span></span>
<span data-ttu-id="015fd-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="015fd-111">None.</span></span>


## <a name="relationships"></a><span data-ttu-id="015fd-112">Relações</span><span class="sxs-lookup"><span data-stu-id="015fd-112">Relationships</span></span>
<span data-ttu-id="015fd-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="015fd-113">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="015fd-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="015fd-114">JSON representation</span></span>
<span data-ttu-id="015fd-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="015fd-115">The following is a JSON representation of the resource.</span></span>
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
