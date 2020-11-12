---
title: tipo de recurso accessReviewScope
description: 'No recurso de revisões do Azure AD Access, o `accessReviewScope` representa quais entidades serão revisadas em uma revisão do Access.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: af5a9bde0763f8aea9e28dc74832586c9e0d2e82
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000767"
---
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="766ab-103">tipo de recurso accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="766ab-103">accessReviewScope resource type</span></span>

<span data-ttu-id="766ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="766ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="766ab-105">O **accessReviewScope** define quais entidades serão revisadas em um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="766ab-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="766ab-106">Isso é expresso como uma consulta OData.</span><span class="sxs-lookup"><span data-stu-id="766ab-106">This is expressed as an odata query.</span></span> <span data-ttu-id="766ab-107">O tipo de consulta também deve ser expresso para que os cenários possam ter suporte para revisar entidades fora do MicrosoftGraph, como ARM.</span><span class="sxs-lookup"><span data-stu-id="766ab-107">The query type must also be expressed so that scenarios can be supported to review entities outside of MicrosoftGraph, such as ARM.</span></span>

## <a name="properties"></a><span data-ttu-id="766ab-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="766ab-108">Properties</span></span>
| <span data-ttu-id="766ab-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="766ab-109">Property</span></span>   | <span data-ttu-id="766ab-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="766ab-110">Type</span></span>  | <span data-ttu-id="766ab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="766ab-111">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="766ab-112">consulta</span><span class="sxs-lookup"><span data-stu-id="766ab-112">query</span></span> |<span data-ttu-id="766ab-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="766ab-113">String</span></span>  | <span data-ttu-id="766ab-114">A consulta que especifica o que será revisado.</span><span class="sxs-lookup"><span data-stu-id="766ab-114">The query specifying what will be reviewed.</span></span> <span data-ttu-id="766ab-115">Consulte a tabela para obter exemplos.</span><span class="sxs-lookup"><span data-stu-id="766ab-115">See table for examples.</span></span> |
|<span data-ttu-id="766ab-116">queryType</span><span class="sxs-lookup"><span data-stu-id="766ab-116">queryType</span></span>  |<span data-ttu-id="766ab-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="766ab-117">String</span></span> | <span data-ttu-id="766ab-118">O tipo de consulta.</span><span class="sxs-lookup"><span data-stu-id="766ab-118">The type of query.</span></span> <span data-ttu-id="766ab-119">Os exemplos incluem MicrosoftGraph e ARM.</span><span class="sxs-lookup"><span data-stu-id="766ab-119">Examples include MicrosoftGraph and ARM.</span></span> |

### <a name="supported-queries-for-accessreviewscope-as-scope"></a><span data-ttu-id="766ab-120">Consultas com suporte para o accessReviewScope como escopo</span><span class="sxs-lookup"><span data-stu-id="766ab-120">Supported queries for accessReviewScope as scope</span></span>
<span data-ttu-id="766ab-121">As consultas a seguir são suportadas como a `scope` propriedade em um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="766ab-121">The following are queries supported as the `scope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="766ab-122">Cenário</span><span class="sxs-lookup"><span data-stu-id="766ab-122">Scenario</span></span>| <span data-ttu-id="766ab-123">Consulta</span><span class="sxs-lookup"><span data-stu-id="766ab-123">Query</span></span> | <span data-ttu-id="766ab-124">Comentários adicionais</span><span class="sxs-lookup"><span data-stu-id="766ab-124">Additional Comments</span></span> |
|--|--|-- |
| <span data-ttu-id="766ab-125">Revisão de todos os usuários atribuídos a um grupo</span><span class="sxs-lookup"><span data-stu-id="766ab-125">Review of all users assigned to a group</span></span> | <span data-ttu-id="766ab-126">/groups/{Group ID}/transitiveMembers</span><span class="sxs-lookup"><span data-stu-id="766ab-126">/groups/{group id}/transitiveMembers</span></span> ||
| <span data-ttu-id="766ab-127">Revisão de usuários convidados atribuídos a um grupo</span><span class="sxs-lookup"><span data-stu-id="766ab-127">Review of guest users assigned to a group</span></span> | <span data-ttu-id="766ab-128">/groups/{Group ID}/Microsoft.Graph.User/? $count = true&$filter = (UserType EQ ' Guest ')</span><span class="sxs-lookup"><span data-stu-id="766ab-128">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> ||
| <span data-ttu-id="766ab-129">Revisão de usuários convidados atribuídos a todos os grupos</span><span class="sxs-lookup"><span data-stu-id="766ab-129">Review of guest users assigned to all groups</span></span> | <span data-ttu-id="766ab-130">./Members/Microsoft.Graph.User/? $count = true&$filter = (UserType EQ ' Guest ')</span><span class="sxs-lookup"><span data-stu-id="766ab-130">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> | <span data-ttu-id="766ab-131">Observe que o instanceEnumerationScope correspondente também deve ser passado para o accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="766ab-131">Note that the corresponding instanceEnumerationScope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="766ab-132">Consulte a tabela abaixo para ver instanceEnumerationScope consulta.</span><span class="sxs-lookup"><span data-stu-id="766ab-132">See table below for instanceEnumerationScope query.</span></span> |
| <span data-ttu-id="766ab-133">Revisões de Assigment do pacote de acesso de gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="766ab-133">Entitlement Management Access Package Assigment Reviews</span></span> | <span data-ttu-id="766ab-134">/identityGovernance/entitlementManagement/accessPackageAssignments? $filter = (accessPackageId EQ ' {Package ID} ' e assignmentPolicyId EQ ' {ID} ')</span><span class="sxs-lookup"><span data-stu-id="766ab-134">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')</span></span>| <span data-ttu-id="766ab-135">Observe que somente leitura tem suporte para revisões de atribuição de pacote do Access</span><span class="sxs-lookup"><span data-stu-id="766ab-135">Note that only READ is supported for Access Package Assignment Reviews</span></span>|

### <a name="supported-queries-for-accessreviewscope-as-instanceenumerationscope"></a><span data-ttu-id="766ab-136">Consultas com suporte para o accessReviewScope como instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="766ab-136">Supported queries for accessReviewScope as instanceEnumerationScope</span></span>
<span data-ttu-id="766ab-137">As consultas a seguir são suportadas como a `instanceEnumerationScope` propriedade em um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="766ab-137">The following are queries supported as the `instanceEnumerationScope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="766ab-138">Cenário</span><span class="sxs-lookup"><span data-stu-id="766ab-138">Scenario</span></span>| <span data-ttu-id="766ab-139">Consulta</span><span class="sxs-lookup"><span data-stu-id="766ab-139">Query</span></span> | <span data-ttu-id="766ab-140">Comentários adicionais</span><span class="sxs-lookup"><span data-stu-id="766ab-140">Additional Comments</span></span> |
|--|--|--|
| <span data-ttu-id="766ab-141">Revisão de usuários convidados atribuídos a todos os grupos, excluindo grupos especificados</span><span class="sxs-lookup"><span data-stu-id="766ab-141">Review of guest users assigned to all groups, excluding specified groups</span></span> | <span data-ttu-id="766ab-142">/groups? $filter = (groupTypes/Any (c:c + EQ + ' Unified ') e ID ne ' {ID de grupo} ' e ID ne ' {ID de grupo} ' e ID ne ' {Group ID} ') &$count = true</span><span class="sxs-lookup"><span data-stu-id="766ab-142">/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and id ne '{group id}' and id ne '{group id}' and id ne '{group id}')&$count=true</span></span> | <span data-ttu-id="766ab-143">Observe que o escopo correspondente deve também ser passado para o accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="766ab-143">Note that the corresponding scope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="766ab-144">Consulte "análise de usuários convidados atribuídos a todos os grupos" na tabela de propriedades de escopo acima para a consulta de escopo.</span><span class="sxs-lookup"><span data-stu-id="766ab-144">See "Review of guest users assigned to all groups" in scope property table above for the scope query.</span></span> |

## <a name="relationships"></a><span data-ttu-id="766ab-145">Relações</span><span class="sxs-lookup"><span data-stu-id="766ab-145">Relationships</span></span>
<span data-ttu-id="766ab-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="766ab-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="766ab-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="766ab-147">JSON representation</span></span>
<span data-ttu-id="766ab-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="766ab-148">The following is a JSON representation of the resource.</span></span>
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
