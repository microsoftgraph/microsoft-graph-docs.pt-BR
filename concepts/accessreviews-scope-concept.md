---
title: Configurar o escopo da sua revisão de acesso usando a API Graph Microsoft
description: Saiba como usar a API de críticas de acesso no Microsoft Graph para revisar o acesso aos recursos do Azure AD.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 731ebcb9ab27baf4ea30553d4f6a598d61e37d59
ms.sourcegitcommit: 2d0daa446c7b37ced1d214e0c6e18e2b8243bb09
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2021
ms.locfileid: "53010188"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a>Configurar o escopo da sua revisão de acesso usando a API Graph Microsoft

A [API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) de revisões de acesso do Azure AD permite que você revise programaticamente o acesso que os usuários, entidades de serviço ou grupos têm aos recursos do Azure AD.

> [!NOTE]
> A [API de críticas de acesso](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) está disponível apenas no ponto de extremidade Graph beta da Microsoft. Não o use em aplicativos de produção, pois ele está sujeito a alterações sem aviso prévio.

Os recursos a revisar são configurados na propriedade **scope** do recurso [access Reviews accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true) Essa propriedade é do tipo [accessReviewScope](/graph/api/resources/accessreviewscope?view=graph-rest-beta&preserve-view=true), um tipo abstrato herdado pelos seguintes recursos que podem ser usados para configurar recursos ou grupos de recursos em que o acesso será revisado.

|Recurso|Descrição|Exemplos de cenários|
|:---    |:---       |:---             |
|[accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope?view=graph-rest-beta&preserve-view=true)|Melhor aplicável ao analisar o conjunto completo ou o subconjunto de entidades que têm acesso a um recurso ou grupo de recursos relacionados.|<ul><li>Associação de usuários atribuídos a um grupo.</li><li>Acesso de usuário convidado a um grupo.</li><li>Acesso do usuário convidado a todos Microsoft 365 grupos em um locatário.</li><li>Entidades de serviço atribuídas a funções privilegiadas.</li><li>Acesso da entidade de serviço e usuário aos pacotes de acesso gerenciamento de direitos.</li></ul>|
|[accessReviewInactiveUsersQueryScope](/graph/api/resources/accessreviewinactiveusersqueryscope?view=graph-rest-beta&preserve-view=true)|Herdado de accessReviewQueryScope. Usado quando apenas usuários inativos são revisados. Seu status inativo é especificado pela **propriedade inactiveDuration.** |<ul><li>Associação de grupo apenas de usuários inativos.</li><ul>|
|[principalResourceMembershipsScope](/graph/api/resources/principalResourceMembershipsScope?view=graph-rest-beta&preserve-view=true)|Melhor aplicável para analisar o acesso das entidades aos recursos em que você configura pools exclusivos de entidades e recursos.|<ul><li>Revisão do acesso de 3 entidades principais específicas em 1 Microsoft 365 *grupo* e 1 função privilegiada do Azure AD.</li><ul>|

Neste artigo, você usará esses tipos de accessReviewScope para configurar uma ampla variedade de recursos do Azure AD como o escopo de sua revisão de acesso. Isso pode ajudá-lo a automatizar a revisão proativa e manter o controle sobre o acesso aos recursos em sua organização.  

## <a name="use-accessreviewqueryscope-to-configure-scope"></a>Usar accessReviewQueryScope para configurar o escopo

Para configurar o escopo usando o **tipo accessReviewQueryScope,** de definir os valores de suas propriedades **de** consulta, **queryRoot** e **queryType.** Para descrições dessas propriedades, consulte [tipo de recurso accessReviewQueryScope.](/graph/api/resources/accessreviewqueryscope?view=graph-rest-beta&preserve-view=true)

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
````

### <a name="example-2-review-guest-users-assigned-to-a-group"></a>Exemplo 2: Revisar usuários convidados atribuídos a um grupo

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-3-review-guest-users-assigned-to-all-microsoft-365-groups"></a>Exemplo 3: Revisar usuários convidados atribuídos a todos os Microsoft 365 grupos

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

Como essa revisão é aplicada em todos os grupos Microsoft 365, configure **a instânciaEnumerationScope** para especificar os grupos Microsoft 365 a revisar.

### <a name="example-4-review-access-of-all-inactive-guest-users-to-all-groups"></a>Exemplo 4: Revisar o acesso de todos os usuários convidados inativos a todos os grupos

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

Como essa revisão é aplicada a usuários inativos, use o **recurso accessReviewInactiveUsersQueryScope** e especifique a propriedade **@odata.type com** o valor `#microsoft.graph.accessReviewInactiveUsersQueryScope` .

### <a name="example-5-review-of-all-inactive-guest-users-assigned-to-all-teams"></a>Exemplo 5: Revisão de todos os usuários convidados inativos atribuídos a todas as equipes

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

Como essa revisão é aplicada a todas as equipes, configure a **propriedade instanceEnumerationScope** para especificar todas as equipes.

### <a name="example-6-review-of-entitlement-management-access-package-assignment"></a>Exemplo 6: Revisão da atribuição do pacote de acesso do Gerenciamento de Direitos

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-7-review-of-service-principals-assigned-to-privileged-roles"></a>Exemplo 7: Revisão das entidades de serviço atribuídas a funções privilegiadas 

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/beta/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a>Usar o principalResourceMembershipsScope para configurar o escopo

O **principalResourceMembershipsScope** expõe as propriedades **principalScopes** e **resourceScopes** para dar suporte a opções de configuração mais personalizadas para o escopo **do accessReviewScheduleDefinition**. Isso inclui a revisão do acesso a várias entidades ou grupos de entidades para vários recursos.

### <a name="example-1-review-access-of-all-inactive-guest-users-to-groups"></a>Exemplo 1: revisar o acesso de todos os usuários convidados inativos a grupos

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

### <a name="example-2-review-access-of-all-guest-users-to-a-directory-role"></a>Exemplo 2: revisar o acesso de todos os usuários convidados a uma função de diretório

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

## <a name="see-also"></a>Confira também

+ [Atribuir revisadores à sua definição de revisão de acesso](/graph/accessreviews-reviewers-concept)