---
title: Configurar o escopo da sua revisão de acesso usando a API Graph Microsoft
description: Saiba como usar a API de críticas de acesso no Microsoft Graph para revisar o acesso aos recursos do Azure AD.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: a4ed9b17d8d2b831071dc8f24e8330e595b543dc
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060295"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a><span data-ttu-id="d36bc-103">Configurar o escopo da sua revisão de acesso usando a API Graph Microsoft</span><span class="sxs-lookup"><span data-stu-id="d36bc-103">Configure the scope of your access review using the Microsoft Graph API</span></span>

<span data-ttu-id="d36bc-104">A [API](/graph/api/resources/accessreviewsv2-root) de revisões de acesso do Azure AD permite que você revise programaticamente o acesso que os usuários, entidades de serviço ou grupos têm aos recursos do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d36bc-104">The Azure AD [access reviews API](/graph/api/resources/accessreviewsv2-root) allows you to programmatically review the access that users, service principals, or groups have to your Azure AD resources.</span></span>

<span data-ttu-id="d36bc-105">Os recursos a revisar são configurados na propriedade **scope** do recurso [access Reviews accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition)</span><span class="sxs-lookup"><span data-stu-id="d36bc-105">The resources to review are configured in the **scope** property of the access reviews [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition) resource.</span></span> <span data-ttu-id="d36bc-106">Essa propriedade é do tipo [accessReviewScope](/graph/api/resources/accessreviewscope), um tipo abstrato herdado pelos seguintes recursos que podem ser usados para configurar recursos ou grupos de recursos em que o acesso será revisado.</span><span class="sxs-lookup"><span data-stu-id="d36bc-106">This property is of the type [accessReviewScope](/graph/api/resources/accessreviewscope), an abstract type inherited by the following resources that can be used to configure resources or groups of resources that access will be reviewed against.</span></span>

|<span data-ttu-id="d36bc-107">Recurso</span><span class="sxs-lookup"><span data-stu-id="d36bc-107">Resource</span></span>|<span data-ttu-id="d36bc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d36bc-108">Description</span></span>|<span data-ttu-id="d36bc-109">Exemplos de cenários</span><span class="sxs-lookup"><span data-stu-id="d36bc-109">Example scenarios</span></span>|
|:---    |:---       |:---             |
|[<span data-ttu-id="d36bc-110">accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="d36bc-110">accessReviewQueryScope</span></span>](/graph/api/resources/accessreviewqueryscope)|<span data-ttu-id="d36bc-111">Melhor aplicável ao analisar o conjunto completo ou o subconjunto de entidades que têm acesso a um recurso ou grupo de recursos relacionados.</span><span class="sxs-lookup"><span data-stu-id="d36bc-111">Best applicable when reviewing the full set or subset of principals who have access to a resource or group of related resources.</span></span>|<ul><li><span data-ttu-id="d36bc-112">Associação de usuários atribuídos a um grupo.</span><span class="sxs-lookup"><span data-stu-id="d36bc-112">Membership of users assigned to a group.</span></span></li><li><span data-ttu-id="d36bc-113">Acesso de usuário convidado a um grupo.</span><span class="sxs-lookup"><span data-stu-id="d36bc-113">Guest user access to one group.</span></span></li><li><span data-ttu-id="d36bc-114">Acesso do usuário convidado a todos Microsoft 365 grupos em um locatário.</span><span class="sxs-lookup"><span data-stu-id="d36bc-114">Guest user access to all Microsoft 365 groups in a tenant.</span></span></li><li><span data-ttu-id="d36bc-115">Entidades de serviço atribuídas a funções privilegiadas.</span><span class="sxs-lookup"><span data-stu-id="d36bc-115">Service principals assigned to privileged roles.</span></span></li><li><span data-ttu-id="d36bc-116">Acesso da entidade de serviço e usuário aos pacotes de acesso gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="d36bc-116">User and service principal access to Entitlement Management access packages.</span></span></li></ul>|
|[<span data-ttu-id="d36bc-117">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="d36bc-117">accessReviewInactiveUsersQueryScope</span></span>](/graph/api/resources/accessreviewinactiveusersqueryscope)|<span data-ttu-id="d36bc-118">Herdado de accessReviewQueryScope.</span><span class="sxs-lookup"><span data-stu-id="d36bc-118">Inherited from accessReviewQueryScope.</span></span> <span data-ttu-id="d36bc-119">Usado quando apenas usuários inativos são revisados.</span><span class="sxs-lookup"><span data-stu-id="d36bc-119">Used when only inactive users are reviewed.</span></span> <span data-ttu-id="d36bc-120">Seu status inativo é especificado pela **propriedade inactiveDuration.**</span><span class="sxs-lookup"><span data-stu-id="d36bc-120">Their inactive status is specified by the **inactiveDuration** property.</span></span> |<ul><li><span data-ttu-id="d36bc-121">Associação de grupo apenas de usuários inativos.</span><span class="sxs-lookup"><span data-stu-id="d36bc-121">Group membership of only inactive users.</span></span></li><ul>|
|[<span data-ttu-id="d36bc-122">principalResourceMembershipsScope</span><span class="sxs-lookup"><span data-stu-id="d36bc-122">principalResourceMembershipsScope</span></span>](/graph/api/resources/principalResourceMembershipsScope)|<span data-ttu-id="d36bc-123">Melhor aplicável para analisar o acesso das entidades aos recursos em que você configura pools exclusivos de entidades e recursos.</span><span class="sxs-lookup"><span data-stu-id="d36bc-123">Best applicable to review principals' access to resources where you configure unique pools of principals and resources.</span></span>|<ul><li><span data-ttu-id="d36bc-124">Revisão do acesso de 3 entidades principais específicas em 1 Microsoft 365 *grupo* e 1 função privilegiada do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d36bc-124">Reviewing access of 3 specific principals across 1 Microsoft 365 group *and* 1 privileged Azure AD role.</span></span></li><ul>|

<span data-ttu-id="d36bc-125">Neste artigo, você usará esses tipos de accessReviewScope para configurar uma ampla variedade de recursos do Azure AD como o escopo de sua revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="d36bc-125">In this article, you will use these types of accessReviewScope to configure a wide range of Azure AD resources as the scope of your access review.</span></span> <span data-ttu-id="d36bc-126">Isso pode ajudá-lo a automatizar a revisão proativa e manter o controle sobre o acesso aos recursos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="d36bc-126">This can help you to automate proactive review and keep control over access to resources in your organization.</span></span>  

## <a name="use-accessreviewqueryscope-to-configure-scope"></a><span data-ttu-id="d36bc-127">Usar accessReviewQueryScope para configurar o escopo</span><span class="sxs-lookup"><span data-stu-id="d36bc-127">Use accessReviewQueryScope to configure scope</span></span>

<span data-ttu-id="d36bc-128">Para configurar o escopo usando o **tipo accessReviewQueryScope,** de definir os valores de suas propriedades **de** consulta, **queryRoot** e **queryType.**</span><span class="sxs-lookup"><span data-stu-id="d36bc-128">To configure the scope by using the **accessReviewQueryScope** type, set the values of its **query**, **queryRoot**, and **queryType** properties.</span></span> <span data-ttu-id="d36bc-129">Para descrições dessas propriedades, consulte [tipo de recurso accessReviewQueryScope.](/graph/api/resources/accessreviewqueryscope)</span><span class="sxs-lookup"><span data-stu-id="d36bc-129">For descriptions of these properties, see [accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope) resource type.</span></span>

### <a name="example-1-review-all-users-assigned-to-a-group"></a><span data-ttu-id="d36bc-130">Exemplo 1: Revisar todos os usuários atribuídos a um grupo</span><span class="sxs-lookup"><span data-stu-id="d36bc-130">Example 1: Review all users assigned to a group</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
```
<span data-ttu-id="d36bc-131">Para revisar *somente usuários inativos* atribuídos ao grupo:</span><span class="sxs-lookup"><span data-stu-id="d36bc-131">To review *only inactive users* assigned to the group:</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "inactiveDuration": "P30D",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
````

### <a name="example-2-review-guest-users-assigned-to-a-group"></a><span data-ttu-id="d36bc-132">Exemplo 2: Revisar usuários convidados atribuídos a um grupo</span><span class="sxs-lookup"><span data-stu-id="d36bc-132">Example 2: Review guest users assigned to a group</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-3-review-guest-users-assigned-to-all-microsoft-365-groups"></a><span data-ttu-id="d36bc-133">Exemplo 3: Revisar usuários convidados atribuídos a todos os Microsoft 365 grupos</span><span class="sxs-lookup"><span data-stu-id="d36bc-133">Example 3: Review guest users assigned to all Microsoft 365 groups</span></span>

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true ",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph"
}
```

<span data-ttu-id="d36bc-134">Como essa revisão é aplicada em todos os grupos Microsoft 365, configure **a instânciaEnumerationScope** para especificar os grupos Microsoft 365 a revisar.</span><span class="sxs-lookup"><span data-stu-id="d36bc-134">Because this review is applied on all Microsoft 365 groups, configure the **instanceEnumerationScope** to specify the Microsoft 365 groups to review.</span></span>

### <a name="example-4-review-access-of-all-inactive-guest-users-to-all-groups"></a><span data-ttu-id="d36bc-135">Exemplo 4: Revisar o acesso de todos os usuários convidados inativos a todos os grupos</span><span class="sxs-lookup"><span data-stu-id="d36bc-135">Example 4: Review access of all inactive guest users to all groups</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

<span data-ttu-id="d36bc-136">Como essa revisão é aplicada a usuários inativos, use o **recurso accessReviewInactiveUsersQueryScope** e especifique a propriedade **@odata.type com** o valor `#microsoft.graph.accessReviewInactiveUsersQueryScope` .</span><span class="sxs-lookup"><span data-stu-id="d36bc-136">Because this review is applied on inactive users, use the **accessReviewInactiveUsersQueryScope** resource and specify the **@odata.type** type property with the value `#microsoft.graph.accessReviewInactiveUsersQueryScope`.</span></span>

### <a name="example-5-review-of-all-inactive-guest-users-assigned-to-all-teams"></a><span data-ttu-id="d36bc-137">Exemplo 5: Revisão de todos os usuários convidados inativos atribuídos a todas as equipes</span><span class="sxs-lookup"><span data-stu-id="d36bc-137">Example 5: Review of all inactive guest users assigned to all teams</span></span>

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

<span data-ttu-id="d36bc-138">Como essa revisão é aplicada a todas as equipes, configure a **propriedade instanceEnumerationScope** para especificar todas as equipes.</span><span class="sxs-lookup"><span data-stu-id="d36bc-138">Because this review is applied on all teams, configure the **instanceEnumerationScope** property to specify all teams.</span></span>

### <a name="example-6-review-of-entitlement-management-access-package-assignment"></a><span data-ttu-id="d36bc-139">Exemplo 6: Revisão da atribuição do pacote de acesso do Gerenciamento de Direitos</span><span class="sxs-lookup"><span data-stu-id="d36bc-139">Example 6: Review of Entitlement Management access package assignment</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-7-review-of-service-principals-assigned-to-privileged-roles"></a><span data-ttu-id="d36bc-140">Exemplo 7: Revisão das entidades de serviço atribuídas a funções privilegiadas</span><span class="sxs-lookup"><span data-stu-id="d36bc-140">Example 7: Review of service principals assigned to privileged roles</span></span> 

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a><span data-ttu-id="d36bc-141">Usar o principalResourceMembershipsScope para configurar o escopo</span><span class="sxs-lookup"><span data-stu-id="d36bc-141">Use principalResourceMembershipsScope to configure scope</span></span>

<span data-ttu-id="d36bc-142">O **principalResourceMembershipsScope** expõe as propriedades **principalScopes** e **resourceScopes** para dar suporte a opções de configuração mais personalizadas para o escopo **do accessReviewScheduleDefinition**.</span><span class="sxs-lookup"><span data-stu-id="d36bc-142">The **principalResourceMembershipsScope** exposes the **principalScopes** and **resourceScopes** properties to support more tailored configuration options for the scope of the **accessReviewScheduleDefinition**.</span></span> <span data-ttu-id="d36bc-143">Isso inclui a revisão do acesso a várias entidades ou grupos de entidades para vários recursos.</span><span class="sxs-lookup"><span data-stu-id="d36bc-143">This includes reviewing access for multiple principals or groups of principals to multiple resources.</span></span>

### <a name="example-1-review-access-of-all-inactive-guest-users-to-groups"></a><span data-ttu-id="d36bc-144">Exemplo 1: revisar o acesso de todos os usuários convidados inativos a grupos</span><span class="sxs-lookup"><span data-stu-id="d36bc-144">Example 1: Review access of all inactive guest users to groups</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
            "query": "/users?$filter=(userType eq 'Guest')",
            "queryType": "MicrosoftGraph",
            "inactiveDuration": "P30D"
        }
    ],
    "resourceScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/groups",
            "queryType": "MicrosoftGraph"
        }
    ]
}
```

<span data-ttu-id="d36bc-145">Neste exemplo, as entidades principais são todos usuários convidados inativos com o período de sua inatividade calculado como 30 dias a partir da data de início da instância de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="d36bc-145">In this example, the principals are all inactive guest users with the period of their inactivity calculated as 30 days from the start date of the access review instance.</span></span>

### <a name="example-2-review-access-of-all-guest-users-to-a-directory-role"></a><span data-ttu-id="d36bc-146">Exemplo 2: revisar o acesso de todos os usuários convidados a uma função de diretório</span><span class="sxs-lookup"><span data-stu-id="d36bc-146">Example 2: Review access of all guest users to a directory role</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/users?$filter=(userType eq 'Guest')",
            "queryType": "MicrosoftGraph"
        }
    ],
    "resourceScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/roleManagement/directory/roleDefinitions/{role id}",
            "queryType": "MicrosoftGraph"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="d36bc-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="d36bc-147">See also</span></span>

+ [<span data-ttu-id="d36bc-148">Atribuir revisadores à sua definição de revisão de acesso</span><span class="sxs-lookup"><span data-stu-id="d36bc-148">Assign reviewers to your access review definition</span></span>](/graph/accessreviews-reviewers-concept)
