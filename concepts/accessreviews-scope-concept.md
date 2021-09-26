---
title: Configurar o escopo da sua revisão de acesso usando a API Graph Microsoft
description: Saiba como usar a API de críticas de acesso no Microsoft Graph para revisar o acesso aos recursos do Azure AD.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: d261fd40629c75c40bf0c93fd42ac8221fdb09e1
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766723"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a>Configurar o escopo da sua revisão de acesso usando a API Graph Microsoft

A [API](/graph/api/resources/accessreviewsv2-root) de revisões de acesso do Azure AD permite que você revise programaticamente o acesso que os usuários, entidades de serviço ou grupos têm aos recursos do Azure AD.

Os recursos a revisar são configurados na propriedade **scope** do recurso [access Reviews accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition) Essa propriedade é do tipo [accessReviewScope](/graph/api/resources/accessreviewscope), um tipo abstrato herdado pelos seguintes recursos que podem ser usados para configurar recursos ou grupos de recursos em que o acesso será revisado.

|Recurso|Descrição|Exemplos de cenários|
|:---    |:---       |:---             |
|[accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope)|Melhor aplicável ao analisar o conjunto completo ou o subconjunto de entidades que têm acesso a um recurso ou grupo de recursos relacionados.|<ul><li>Associação de usuários atribuídos a um grupo.</li><li>Acesso de usuário convidado a um grupo.</li><li>Acesso do usuário convidado a todos Microsoft 365 grupos em um locatário.</li><li>Entidades de serviço atribuídas a funções privilegiadas.</li><li>Acesso da entidade de serviço e usuário aos pacotes de acesso gerenciamento de direitos.</li></ul>|
|[accessReviewInactiveUsersQueryScope](/graph/api/resources/accessreviewinactiveusersqueryscope)|Herdado de accessReviewQueryScope. Usado quando apenas usuários inativos são revisados. Seu status inativo é especificado pela **propriedade inactiveDuration.** |<ul><li>Associação de grupo apenas de usuários inativos.</li><ul>|
|[principalResourceMembershipsScope](/graph/api/resources/principalResourceMembershipsScope)|Melhor aplicável para analisar o acesso das entidades aos recursos em que você configura pools exclusivos de entidades e recursos.|<ul><li>Revisão do acesso de 3 entidades principais específicas em 1 Microsoft 365 *grupo* e 1 função privilegiada do Azure AD.</li><ul>|

Neste artigo, você usará esses tipos de accessReviewScope para configurar uma ampla variedade de recursos do Azure AD como o escopo de sua revisão de acesso. Isso pode ajudá-lo a automatizar a revisão proativa e manter o controle sobre o acesso aos recursos em sua organização.  

## <a name="use-accessreviewqueryscope-to-configure-scope"></a>Usar accessReviewQueryScope para configurar o escopo

Para configurar o escopo usando o **tipo accessReviewQueryScope,** de definir os valores de suas propriedades **de** consulta, **queryRoot** e **queryType.** Para descrições dessas propriedades, consulte [tipo de recurso accessReviewQueryScope.](/graph/api/resources/accessreviewqueryscope)

### <a name="example-1-review-all-users-assigned-to-a-group"></a>Exemplo 1: Revisar todos os usuários atribuídos a um grupo

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
```

Para revisar *somente usuários inativos* atribuídos ao grupo:

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "inactiveDuration": "P30D",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-2-review-guest-users-assigned-to-a-group"></a>Exemplo 2: Revisar usuários convidados atribuídos a um grupo

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-3-review-guest-users-assigned-to-all-microsoft-365-groups"></a>Exemplo 3: Revisar usuários convidados atribuídos a todos os Microsoft 365 grupos

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified'))",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph"
}
```

Como essa revisão é aplicada em todos os grupos Microsoft 365, configure **a instânciaEnumerationScope** para especificar os grupos Microsoft 365 a revisar.
    
### <a name="example-4-review-of-all-guest-users-assigned-to-all-teams"></a>Exemplo 4: Revisão de todos os usuários convidados atribuídos a todos os Teams

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph"
}
```
    
Como essa revisão é aplicada Teams todos os grupos Microsoft 365 habilitados para Microsoft 365, configure **a instânciaEnumerationScope** para especificar os grupos Microsoft 365 habilitados para Teams para revisão.

### <a name="example-5-review-access-of-all-inactive-guest-users-to-all-groups"></a>Exemplo 5: revisar o acesso de todos os usuários convidados inativos a todos os grupos

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

Como essa revisão é aplicada a usuários inativos, use o **recurso accessReviewInactiveUsersQueryScope** e especifique a propriedade **@odata.type com** o valor `#microsoft.graph.accessReviewInactiveUsersQueryScope` .

### <a name="example-6-review-of-all-inactive-guest-users-assigned-to-all-teams"></a>Exemplo 6: Revisão de todos os usuários convidados inativos atribuídos a todas as equipes

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

Como essa revisão é aplicada a todas as equipes, configure a **propriedade instanceEnumerationScope** para especificar todas as equipes.

### <a name="example-7-review-of-entitlement-management-access-package-assignment"></a>Exemplo 7: Revisão da atribuição do pacote de acesso do Gerenciamento de Direitos

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-8-review-of-all-service-principals-assigned-to-a-privileged-role"></a>Exemplo 8: Revisão de todas as entidades de serviço atribuídas a uma função privilegiada

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```
    
### <a name="example-9-review-of-all-users-assigned-to-a-privileged-role-all-active-and-eligible-assignments-included"></a>Exemplo 9: Revisão de todos os usuários atribuídos a uma função privilegiada (todas as atribuições ativas e qualificadas incluídas)

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleDefinitions/{role ID}",
    "queryType": "MicrosoftGraph"
}
```
    
### <a name="example-10-review-of-all-users-with-eligible-assignment-to-a-privileged-role"></a>Exemplo 10: Revisão de todos os usuários com atribuição qualificada para uma função privilegiada

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleEligibilityScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.user') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```
    
### <a name="example-11-review-of-all-users-with-active-assignment-to-a-privileged-role"></a>Exemplo 11: Revisão de todos os usuários com atribuição ativa para uma função privilegiada

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(assignmentType eq 'Assigned' and isof(principal,'microsoft.graph.user') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a>Usar o principalResourceMembershipsScope para configurar o escopo

O **principalResourceMembershipsScope** expõe as propriedades **principalScopes** e **resourceScopes** para dar suporte a opções de configuração mais personalizadas para o escopo **do accessReviewScheduleDefinition**. Isso inclui a revisão do acesso a várias entidades ou grupos de entidades para vários recursos.

### <a name="example-12-review-access-of-all-inactive-guest-users-to-all-groups"></a>Exemplo 12: Revisar o acesso de todos os usuários convidados inativos a todos os grupos

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

Neste exemplo, as entidades principais são todos usuários convidados inativos com o período de sua inatividade calculado como 30 dias a partir da data de início da instância de revisão de acesso.

### <a name="example-13-review-access-of-all-guest-users-to-a-directory-role"></a>Exemplo 13: Revisar o acesso de todos os usuários convidados a uma função de diretório

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

## <a name="next-steps"></a>Próximas etapas

+ [Atribuir revisadores à sua definição de revisão de acesso](/graph/accessreviews-reviewers-concept)
+ [Experimente tutoriais para](/graph/accessreviews-overview) saber como usar a API de avaliações de acesso para revisar o acesso aos recursos do Azure AD
