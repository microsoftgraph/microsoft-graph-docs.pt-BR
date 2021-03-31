---
title: Tipo de recurso accessReviewQueryScope
description: Define o que será revisado em uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 976a856755b6bb638719bec6006c3d8d0587c42a
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469731"
---
# <a name="accessreviewqueryscope-resource-type"></a><span data-ttu-id="c12eb-103">Tipo de recurso accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="c12eb-103">accessReviewQueryScope resource type</span></span>

<span data-ttu-id="c12eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c12eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="c12eb-105">Um objeto accessReviewQueryScope define o que será revisado em [um accessReview](../resources/accessreviewsv2-root.md).</span><span class="sxs-lookup"><span data-stu-id="c12eb-105">An accessReviewQueryScope object defines what will be reviewed in an [accessReview](../resources/accessreviewsv2-root.md).</span></span> <span data-ttu-id="c12eb-106">Consulte as consultas com suporte para ver as opções de seleção.</span><span class="sxs-lookup"><span data-stu-id="c12eb-106">See the supported queries to see the selection options.</span></span> <span data-ttu-id="c12eb-107">Para analisar o escopo de uma revisão de acesso a usuários inativos, consulte [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="c12eb-107">To scope an access review to inactive users, see [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span></span> 

<span data-ttu-id="c12eb-108">Herda de [accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="c12eb-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c12eb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c12eb-109">Properties</span></span>
|<span data-ttu-id="c12eb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c12eb-110">Property</span></span>|<span data-ttu-id="c12eb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c12eb-111">Type</span></span>|<span data-ttu-id="c12eb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c12eb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c12eb-113">consulta</span><span class="sxs-lookup"><span data-stu-id="c12eb-113">query</span></span>|<span data-ttu-id="c12eb-114">String</span><span class="sxs-lookup"><span data-stu-id="c12eb-114">String</span></span>|<span data-ttu-id="c12eb-115">A consulta que representa o que será revisado em uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="c12eb-115">The query representing what will be reviewed in an access review.</span></span> <span data-ttu-id="c12eb-116">Exemplos disso incluem /groups/{id}/members?$filter=...</span><span class="sxs-lookup"><span data-stu-id="c12eb-116">Examples of this include /groups/{id}/members?$filter=…</span></span>|
|<span data-ttu-id="c12eb-117">queryRoot</span><span class="sxs-lookup"><span data-stu-id="c12eb-117">queryRoot</span></span>|<span data-ttu-id="c12eb-118">String</span><span class="sxs-lookup"><span data-stu-id="c12eb-118">String</span></span>|<span data-ttu-id="c12eb-119">No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta.</span><span class="sxs-lookup"><span data-stu-id="c12eb-119">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="c12eb-120">Essa propriedade só será necessária se uma consulta relativa for especificada.</span><span class="sxs-lookup"><span data-stu-id="c12eb-120">This property is only required if a relative query is specified.</span></span> <span data-ttu-id="c12eb-121">Por exemplo, `./manager`.</span><span class="sxs-lookup"><span data-stu-id="c12eb-121">For example, `./manager`.</span></span>|
|<span data-ttu-id="c12eb-122">queryType</span><span class="sxs-lookup"><span data-stu-id="c12eb-122">queryType</span></span>|<span data-ttu-id="c12eb-123">String</span><span class="sxs-lookup"><span data-stu-id="c12eb-123">String</span></span>|<span data-ttu-id="c12eb-124">Indica o tipo de consulta.</span><span class="sxs-lookup"><span data-stu-id="c12eb-124">Indicates the type of query.</span></span> <span data-ttu-id="c12eb-125">Os tipos incluem MicrosoftGraph e ARM.</span><span class="sxs-lookup"><span data-stu-id="c12eb-125">Types include MicrosoftGraph and ARM.</span></span>|

### <a name="supported-queries-for-accessreviewqueryscope-as-scope"></a><span data-ttu-id="c12eb-126">Consultas com suporte para accessReviewQueryScope como escopo</span><span class="sxs-lookup"><span data-stu-id="c12eb-126">Supported queries for accessReviewQueryScope as scope</span></span>
<span data-ttu-id="c12eb-127">As consultas são suportadas como a `scope` propriedade em [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c12eb-127">The queries are supported as the `scope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="c12eb-128">Cenário</span><span class="sxs-lookup"><span data-stu-id="c12eb-128">Scenario</span></span>| <span data-ttu-id="c12eb-129">Consulta</span><span class="sxs-lookup"><span data-stu-id="c12eb-129">Query</span></span> | <span data-ttu-id="c12eb-130">Comentários adicionais</span><span class="sxs-lookup"><span data-stu-id="c12eb-130">Additional Comments</span></span> |
|--|--|-- |
| <span data-ttu-id="c12eb-131">Revisão de todos os usuários atribuídos a um grupo</span><span class="sxs-lookup"><span data-stu-id="c12eb-131">Review of all users assigned to a group</span></span> | <span data-ttu-id="c12eb-132">/groups/{group id}/transitiveMembers</span><span class="sxs-lookup"><span data-stu-id="c12eb-132">/groups/{group id}/transitiveMembers</span></span> ||
| <span data-ttu-id="c12eb-133">Revisão de usuários convidados atribuídos a um grupo</span><span class="sxs-lookup"><span data-stu-id="c12eb-133">Review of guest users assigned to a group</span></span> | <span data-ttu-id="c12eb-134">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="c12eb-134">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> ||
| <span data-ttu-id="c12eb-135">Revisão de usuários convidados atribuídos a todos os grupos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c12eb-135">Review of guest users assigned to all Microsoft 365 groups</span></span> | <span data-ttu-id="c12eb-136">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="c12eb-136">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> | <span data-ttu-id="c12eb-137">Observe que a instância correspondenteEnumerationScope também deve ser passada para accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="c12eb-137">Note that the corresponding instanceEnumerationScope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="c12eb-138">Consulte a tabela abaixo para consulta instanceEnumerationScope.</span><span class="sxs-lookup"><span data-stu-id="c12eb-138">See table below for instanceEnumerationScope query.</span></span> |
| <span data-ttu-id="c12eb-139">Avaliações de atribuição de pacote de acesso ao gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="c12eb-139">Entitlement Management Access Package Assignment Reviews</span></span> | <span data-ttu-id="c12eb-140">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')</span><span class="sxs-lookup"><span data-stu-id="c12eb-140">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')</span></span>| <span data-ttu-id="c12eb-141">Observe que somente READ é suportado para Avaliações de Atribuição de Pacote do Access</span><span class="sxs-lookup"><span data-stu-id="c12eb-141">Note that only READ is supported for Access Package Assignment Reviews</span></span>|
| <span data-ttu-id="c12eb-142">Revisão das Entidades de Serviço atribuídas a funções privilegiadas</span><span class="sxs-lookup"><span data-stu-id="c12eb-142">Review of Service Principals assigned to privileged roles</span></span> | <span data-ttu-id="c12eb-143">/beta/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') e roleDefinitionId eq '{role ID}')</span><span class="sxs-lookup"><span data-stu-id="c12eb-143">/beta/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')</span></span> | |

### <a name="supported-queries-for-instanceenumerationscope"></a><span data-ttu-id="c12eb-144">Consultas com suporte para instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="c12eb-144">Supported queries for instanceEnumerationScope</span></span> 
<span data-ttu-id="c12eb-145">As consultas são suportadas como a `instanceEnumerationScope` propriedade em [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c12eb-145">The queries are supported as the `instanceEnumerationScope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="c12eb-146">Cenário</span><span class="sxs-lookup"><span data-stu-id="c12eb-146">Scenario</span></span>| <span data-ttu-id="c12eb-147">Consulta</span><span class="sxs-lookup"><span data-stu-id="c12eb-147">Query</span></span> | <span data-ttu-id="c12eb-148">Comentários adicionais</span><span class="sxs-lookup"><span data-stu-id="c12eb-148">Additional Comments</span></span> |
|--|--|--|
|  <span data-ttu-id="c12eb-149">Revisão de usuários convidados atribuídos a todos os grupos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c12eb-149">Review of guest users assigned to all Microsoft 365 groups</span></span>| <span data-ttu-id="c12eb-150">/v1.0/groups? \$ filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true</span><span class="sxs-lookup"><span data-stu-id="c12eb-150">/v1.0/groups?\$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true</span></span> | <span data-ttu-id="c12eb-151">Observe que o escopo correspondente também deve ser passado junto com isso</span><span class="sxs-lookup"><span data-stu-id="c12eb-151">Note that the corresponding scope should also be passed in along with this</span></span>|
| <span data-ttu-id="c12eb-152">Revisão de usuários convidados atribuídos a todas as equipes</span><span class="sxs-lookup"><span data-stu-id="c12eb-152">Review of guest users assigned to all teams</span></span> | <span data-ttu-id="c12eb-153">/v1.0/groups? \$ filter=(groupTypes/any(c:c+eq+'Unified') e resourceProvisioningOptions/Any(x:x eq 'Team'))&$count=true</span><span class="sxs-lookup"><span data-stu-id="c12eb-153">/v1.0/groups?\$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team'))&$count=true</span></span> | <span data-ttu-id="c12eb-154">Observe que o escopo correspondente também deve ser passado junto com isso</span><span class="sxs-lookup"><span data-stu-id="c12eb-154">Note that the corresponding scope should also be passed in along with this</span></span>|

## <a name="relationships"></a><span data-ttu-id="c12eb-155">Relações</span><span class="sxs-lookup"><span data-stu-id="c12eb-155">Relationships</span></span>
<span data-ttu-id="c12eb-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c12eb-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c12eb-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c12eb-157">JSON representation</span></span>
<span data-ttu-id="c12eb-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c12eb-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
