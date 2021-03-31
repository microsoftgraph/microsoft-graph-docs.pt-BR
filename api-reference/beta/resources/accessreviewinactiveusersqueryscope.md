---
title: Tipo de recurso accessReviewInactiveUsersQueryScope
description: Um tipo de accessReviewQueryScope que permite que apenas usuários inativos sejam selecionados no escopo de uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 51fc61ce186b0346bc065ddc5dfea40158758223
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469732"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a><span data-ttu-id="2cacc-103">Tipo de recurso accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="2cacc-103">accessReviewInactiveUsersQueryScope resource type</span></span>

<span data-ttu-id="2cacc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cacc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="2cacc-105">Um tipo de [accessReviewQueryScope](../resources/accessreviewqueryscope.md) que permite que apenas usuários inativos sejam selecionados no escopo de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="2cacc-105">A type of [accessReviewQueryScope](../resources/accessreviewqueryscope.md) that allows only inactive users to be selected in the scope of an access review.</span></span>

<span data-ttu-id="2cacc-106">Herda de [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="2cacc-106">Inherits from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2cacc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2cacc-107">Properties</span></span>
|<span data-ttu-id="2cacc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cacc-108">Property</span></span>|<span data-ttu-id="2cacc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cacc-109">Type</span></span>|<span data-ttu-id="2cacc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cacc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cacc-111">inactiveDuration</span><span class="sxs-lookup"><span data-stu-id="2cacc-111">inactiveDuration</span></span>|<span data-ttu-id="2cacc-112">Duration</span><span class="sxs-lookup"><span data-stu-id="2cacc-112">Duration</span></span>|<span data-ttu-id="2cacc-113">Define o comprimento do período de duração da inatividade.</span><span class="sxs-lookup"><span data-stu-id="2cacc-113">Defines the length of the duration period of inactivity.</span></span> <span data-ttu-id="2cacc-114">A inatividade é baseada na última data de login do usuário.</span><span class="sxs-lookup"><span data-stu-id="2cacc-114">Inactivity is based on the last sign in date of the user.</span></span>|
|<span data-ttu-id="2cacc-115">consulta</span><span class="sxs-lookup"><span data-stu-id="2cacc-115">query</span></span>|<span data-ttu-id="2cacc-116">String</span><span class="sxs-lookup"><span data-stu-id="2cacc-116">String</span></span>|<span data-ttu-id="2cacc-117">Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="2cacc-117">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="2cacc-118">queryRoot</span><span class="sxs-lookup"><span data-stu-id="2cacc-118">queryRoot</span></span>|<span data-ttu-id="2cacc-119">String</span><span class="sxs-lookup"><span data-stu-id="2cacc-119">String</span></span>|<span data-ttu-id="2cacc-120">Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="2cacc-120">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="2cacc-121">queryType</span><span class="sxs-lookup"><span data-stu-id="2cacc-121">queryType</span></span>|<span data-ttu-id="2cacc-122">String</span><span class="sxs-lookup"><span data-stu-id="2cacc-122">String</span></span>|<span data-ttu-id="2cacc-123">Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="2cacc-123">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|

### <a name="supported-queries-for-accessreviewinactiveuserqueryscope-as-scope"></a><span data-ttu-id="2cacc-124">Consultas com suporte para accessReviewInactiveUserQueryScope como escopo</span><span class="sxs-lookup"><span data-stu-id="2cacc-124">Supported queries for accessReviewInactiveUserQueryScope as scope</span></span>
<span data-ttu-id="2cacc-125">As mesmas consultas com suporte no [accessReviewScope](../resources/accessreviewscope.md) também são suportadas no accessReviewInactiveUserQueryScope.</span><span class="sxs-lookup"><span data-stu-id="2cacc-125">The same queries supported on [accessReviewScope](../resources/accessreviewscope.md) are also supported on accessReviewInactiveUserQueryScope.</span></span> <span data-ttu-id="2cacc-126">A seguir estão as consultas.</span><span class="sxs-lookup"><span data-stu-id="2cacc-126">The following are the queries.</span></span> <span data-ttu-id="2cacc-127">Eles são suportados como a `scope` propriedade em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2cacc-127">They are supported as the `scope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span>

|<span data-ttu-id="2cacc-128">Cenário</span><span class="sxs-lookup"><span data-stu-id="2cacc-128">Scenario</span></span>| <span data-ttu-id="2cacc-129">Consulta</span><span class="sxs-lookup"><span data-stu-id="2cacc-129">Query</span></span> |
|--|--|
| <span data-ttu-id="2cacc-130">Revisar todos os usuários convidados inativos atribuídos a um grupo</span><span class="sxs-lookup"><span data-stu-id="2cacc-130">Review all inactive guest users assigned to a group</span></span> | <span data-ttu-id="2cacc-131">/groups/{group ID}/transitiveMembers/microsoft.graph.user/? \$ count=true&$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="2cacc-131">/groups/{group ID}/transitiveMembers/microsoft.graph.user/?\$count=true&$filter=(userType eq 'Guest')</span></span> |
| <span data-ttu-id="2cacc-132">Revisar todos os usuários inativos atribuídos a um grupo</span><span class="sxs-lookup"><span data-stu-id="2cacc-132">Review all inactive users assigned to a group</span></span> | <span data-ttu-id="2cacc-133">/groups/{group ID}/transitiveMembers</span><span class="sxs-lookup"><span data-stu-id="2cacc-133">/groups/{group ID}/transitiveMembers</span></span> |
| <span data-ttu-id="2cacc-134">Revisar todos os usuários convidados inativos atribuídos a todos os grupos</span><span class="sxs-lookup"><span data-stu-id="2cacc-134">Review all inactive guest users assigned to all groups</span></span> | <span data-ttu-id="2cacc-135">./members/microsoft.graph.user/? \$ count=true&$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="2cacc-135">./members/microsoft.graph.user/?\$count=true&$filter=(userType eq 'Guest')</span></span> |


## <a name="relationships"></a><span data-ttu-id="2cacc-136">Relações</span><span class="sxs-lookup"><span data-stu-id="2cacc-136">Relationships</span></span>
<span data-ttu-id="2cacc-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2cacc-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cacc-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2cacc-138">JSON representation</span></span>
<span data-ttu-id="2cacc-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2cacc-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInactiveUsersQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String",
  "inactiveDuration": "String (duration)"
}
```
