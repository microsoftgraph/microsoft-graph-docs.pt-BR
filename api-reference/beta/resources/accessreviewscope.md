---
title: Tipo de recurso accessReviewScope
description: 'No recurso de revisões de acesso do Azure AD, as entidades serão revisadas em `accessReviewScope` uma revisão de acesso.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8739ff822ffc6b0f2989b80a150c7d968880f532
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133431"
---
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="41f0d-103">Tipo de recurso accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="41f0d-103">accessReviewScope resource type</span></span>

<span data-ttu-id="41f0d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41f0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41f0d-105">O **accessReviewScope** define quais entidades serão revisadas em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="41f0d-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="41f0d-106">Isso é expresso como uma consulta odata.</span><span class="sxs-lookup"><span data-stu-id="41f0d-106">This is expressed as an odata query.</span></span> <span data-ttu-id="41f0d-107">O tipo de consulta também deve ser expresso para que os cenários possam ter suporte para revisar entidades fora do MicrosoftGraph, como ARM.</span><span class="sxs-lookup"><span data-stu-id="41f0d-107">The query type must also be expressed so that scenarios can be supported to review entities outside of MicrosoftGraph, such as ARM.</span></span>

## <a name="properties"></a><span data-ttu-id="41f0d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41f0d-108">Properties</span></span>
| <span data-ttu-id="41f0d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41f0d-109">Property</span></span>   | <span data-ttu-id="41f0d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="41f0d-110">Type</span></span>  | <span data-ttu-id="41f0d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="41f0d-111">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="41f0d-112">consulta</span><span class="sxs-lookup"><span data-stu-id="41f0d-112">query</span></span> |<span data-ttu-id="41f0d-113">String</span><span class="sxs-lookup"><span data-stu-id="41f0d-113">String</span></span>  | <span data-ttu-id="41f0d-114">A consulta especificando o que será revisado.</span><span class="sxs-lookup"><span data-stu-id="41f0d-114">The query specifying what will be reviewed.</span></span> <span data-ttu-id="41f0d-115">Consulte a tabela para ver exemplos.</span><span class="sxs-lookup"><span data-stu-id="41f0d-115">See table for examples.</span></span> |
|<span data-ttu-id="41f0d-116">queryType</span><span class="sxs-lookup"><span data-stu-id="41f0d-116">queryType</span></span>  |<span data-ttu-id="41f0d-117">String</span><span class="sxs-lookup"><span data-stu-id="41f0d-117">String</span></span> | <span data-ttu-id="41f0d-118">O tipo de consulta.</span><span class="sxs-lookup"><span data-stu-id="41f0d-118">The type of query.</span></span> <span data-ttu-id="41f0d-119">Exemplos incluem MicrosoftGraph e ARM.</span><span class="sxs-lookup"><span data-stu-id="41f0d-119">Examples include MicrosoftGraph and ARM.</span></span> |

### <a name="supported-queries-for-accessreviewscope-as-scope"></a><span data-ttu-id="41f0d-120">Consultas com suporte para accessReviewScope como escopo</span><span class="sxs-lookup"><span data-stu-id="41f0d-120">Supported queries for accessReviewScope as scope</span></span>
<span data-ttu-id="41f0d-121">A seguir estão consultas com suporte como a `scope` propriedade em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="41f0d-121">The following are queries supported as the `scope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="41f0d-122">Cenário</span><span class="sxs-lookup"><span data-stu-id="41f0d-122">Scenario</span></span>| <span data-ttu-id="41f0d-123">Consulta</span><span class="sxs-lookup"><span data-stu-id="41f0d-123">Query</span></span> | <span data-ttu-id="41f0d-124">Comentários adicionais</span><span class="sxs-lookup"><span data-stu-id="41f0d-124">Additional Comments</span></span> |
|--|--|-- |
| <span data-ttu-id="41f0d-125">Revisão de todos os usuários atribuídos a um grupo</span><span class="sxs-lookup"><span data-stu-id="41f0d-125">Review of all users assigned to a group</span></span> | <span data-ttu-id="41f0d-126">/groups/{group id}/transitiveMembers</span><span class="sxs-lookup"><span data-stu-id="41f0d-126">/groups/{group id}/transitiveMembers</span></span> ||
| <span data-ttu-id="41f0d-127">Revisão de usuários convidados atribuídos a um grupo</span><span class="sxs-lookup"><span data-stu-id="41f0d-127">Review of guest users assigned to a group</span></span> | <span data-ttu-id="41f0d-128">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="41f0d-128">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> ||
| <span data-ttu-id="41f0d-129">Revisão de usuários convidados atribuídos a todos os grupos</span><span class="sxs-lookup"><span data-stu-id="41f0d-129">Review of guest users assigned to all groups</span></span> | <span data-ttu-id="41f0d-130">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="41f0d-130">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> | <span data-ttu-id="41f0d-131">Observe que a instanceEnumerationScope correspondente também deve ser passada para accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="41f0d-131">Note that the corresponding instanceEnumerationScope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="41f0d-132">Consulte a tabela abaixo para consultar instanceEnumerationScope.</span><span class="sxs-lookup"><span data-stu-id="41f0d-132">See table below for instanceEnumerationScope query.</span></span> |
| <span data-ttu-id="41f0d-133">Avaliações de asigment do pacote de acesso ao gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="41f0d-133">Entitlement Management Access Package Assigment Reviews</span></span> | <span data-ttu-id="41f0d-134">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' e assignmentPolicyId eq '{id}')</span><span class="sxs-lookup"><span data-stu-id="41f0d-134">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')</span></span>| <span data-ttu-id="41f0d-135">Observe que somente READ é suportado para Revisões de Atribuição de Pacote do Access</span><span class="sxs-lookup"><span data-stu-id="41f0d-135">Note that only READ is supported for Access Package Assignment Reviews</span></span>|

### <a name="supported-queries-for-accessreviewscope-as-instanceenumerationscope"></a><span data-ttu-id="41f0d-136">Consultas com suporte para accessReviewScope como instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="41f0d-136">Supported queries for accessReviewScope as instanceEnumerationScope</span></span>
<span data-ttu-id="41f0d-137">A seguir estão consultas com suporte como a `instanceEnumerationScope` propriedade em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="41f0d-137">The following are queries supported as the `instanceEnumerationScope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="41f0d-138">Cenário</span><span class="sxs-lookup"><span data-stu-id="41f0d-138">Scenario</span></span>| <span data-ttu-id="41f0d-139">Consulta</span><span class="sxs-lookup"><span data-stu-id="41f0d-139">Query</span></span> | <span data-ttu-id="41f0d-140">Comentários adicionais</span><span class="sxs-lookup"><span data-stu-id="41f0d-140">Additional Comments</span></span> |
|--|--|--|
| <span data-ttu-id="41f0d-141">Revisão de usuários convidados atribuídos a todos os grupos, excluindo grupos especificados</span><span class="sxs-lookup"><span data-stu-id="41f0d-141">Review of guest users assigned to all groups, excluding specified groups</span></span> | <span data-ttu-id="41f0d-142">/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and id ne '{group id}' and id ne '{group id}' and id ne '{group id}')&$count=true</span><span class="sxs-lookup"><span data-stu-id="41f0d-142">/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and id ne '{group id}' and id ne '{group id}' and id ne '{group id}')&$count=true</span></span> | <span data-ttu-id="41f0d-143">Observe que o escopo correspondente também deve ser passado para accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="41f0d-143">Note that the corresponding scope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="41f0d-144">Consulte "Revisão de usuários convidados atribuídos a todos os grupos" na tabela de propriedades de escopo acima para a consulta de escopo.</span><span class="sxs-lookup"><span data-stu-id="41f0d-144">See "Review of guest users assigned to all groups" in scope property table above for the scope query.</span></span> |

## <a name="relationships"></a><span data-ttu-id="41f0d-145">Relações</span><span class="sxs-lookup"><span data-stu-id="41f0d-145">Relationships</span></span>
<span data-ttu-id="41f0d-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41f0d-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="41f0d-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41f0d-147">JSON representation</span></span>
<span data-ttu-id="41f0d-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41f0d-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScope",
  "query": "String",
  "queryType": "String"
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
