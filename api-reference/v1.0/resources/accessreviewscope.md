---
title: Tipo de recurso accessReviewScope
description: Representa as entidades que precisam ser revisadas em uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8d377bfbf9a69c71d7349724863438ab31ddbe6b
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030974"
---
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="f5b45-103">Tipo de recurso accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="f5b45-103">accessReviewScope resource type</span></span>

<span data-ttu-id="f5b45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5b45-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5b45-105">O **accessReviewScope** define quais entidades serão revisadas em [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f5b45-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="f5b45-106">É um tipo abstrato herdado por [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) e [accessReviewReviewerScope](accessreviewreviewerscope.md).</span><span class="sxs-lookup"><span data-stu-id="f5b45-106">It is an abstract type that is inherited by [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) and [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> 

<span data-ttu-id="f5b45-107">Para **a propriedade scope** em um [accessReviewScheduleDefinition,](accessreviewscheduledefinition.md) consulte [accessReviewQueryScope](accessreviewqueryscope.md) e [principalResourceMembershipsScope](principalresourcemembershipsscope.md).</span><span class="sxs-lookup"><span data-stu-id="f5b45-107">For **scope** property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewQueryScope](accessreviewqueryscope.md) and [principalResourceMembershipsScope](principalresourcemembershipsscope.md).</span></span>

<span data-ttu-id="f5b45-108">Para **a propriedade reviewers** em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md) consulte [accessReviewReviewerScope](accessreviewreviewerscope.md).</span><span class="sxs-lookup"><span data-stu-id="f5b45-108">For **reviewers** property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span>

<span data-ttu-id="f5b45-109">A especificação do tipo  OData no escopo é altamente recomendada para todos os tipos, mas necessária para [o principalResourceMembershipsScope](principalresourcemembershipsscope.md) e [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="f5b45-109">Specifying the OData type in the **scope** is highly recommended for all types but required for [principalResourceMembershipsScope](principalresourcemembershipsscope.md) and [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f5b45-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5b45-110">Properties</span></span>
<span data-ttu-id="f5b45-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f5b45-111">None.</span></span>


## <a name="relationships"></a><span data-ttu-id="f5b45-112">Relações</span><span class="sxs-lookup"><span data-stu-id="f5b45-112">Relationships</span></span>
<span data-ttu-id="f5b45-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5b45-113">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5b45-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5b45-114">JSON representation</span></span>
<span data-ttu-id="f5b45-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5b45-115">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScope"
}
```
