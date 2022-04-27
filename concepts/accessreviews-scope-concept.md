---
title: Configurar o escopo da revisão de acesso usando o Microsoft API do Graph
description: Saiba como usar a API de revisões de acesso no Microsoft Graph para examinar o acesso aos recursos do Azure AD.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 48947751fa6ed8330fe2d4ecda5161ec8d708315
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061150"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a>Configurar o escopo da revisão de acesso usando o Microsoft API do Graph

A [API](/graph/api/resources/accessreviewsv2-overview) de revisões de acesso do Azure AD permite que você examine programaticamente o acesso que os usuários, entidades de serviço ou grupos têm aos seus recursos do Azure AD. A API pode ajudá-lo a automatizar a revisão proativa e manter o controle sobre o acesso aos recursos em sua organização.  

Os recursos a serem examinados são configurados na propriedade **de** escopo do [recurso accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition) . Essa propriedade é do tipo [accessReviewScope](/graph/api/resources/accessreviewscope), um tipo abstrato do qual os seguintes recursos de API que podem ser usados para configurar o escopo de revisão de acesso herdam.

|Recurso|Descrição|Exemplos de cenários|
|:---    |:---       |:---             |
|[accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope)|Herda de **accessReviewScope**. Melhor aplicável ao examinar o conjunto completo ou o subconjunto de entidades de segurança que têm acesso a um recurso ou grupo de recursos relacionados.|<ul><li>Associação de usuários atribuídos a um grupo, membros diretos ou membros diretos e transitivos.</li><li>Acesso de usuário convidado a um grupo.</li><li>Acesso de usuário convidado a todos os Microsoft 365 em um locatário.</li><li>Entidades de serviço atribuídas a funções privilegiadas.</li><li>Acesso de usuário e entidade de serviço aos pacotes de acesso do Gerenciamento de Direitos.</li></ul>|
|[accessReviewInactiveUsersQueryScope](/graph/api/resources/accessreviewinactiveusersqueryscope)|Herda de **accessReviewQueryScope**. Usado quando somente usuários inativos são revisados. Seu status inativo é especificado pela **propriedade inactiveDuration** . |<ul><li>Associação de grupo somente de usuários inativos.</li><ul>|
|[principalResourceMembershipsScope](/graph/api/resources/principalResourceMembershipsScope)|Herda de **accessReviewScope**. Melhor aplicável para examinar o acesso das entidades de segurança aos recursos em que você configura pools exclusivos de entidades de segurança e recursos.|<ul><li>Revisando o acesso de três entidades de segurança específicas em um Microsoft 365 e *uma* função privilegiada do Azure AD.</li><ul>|

Neste artigo, você aprenderá a definir o escopo da revisão de acesso usando esses três tipos de recursos derivados.

## <a name="use-accessreviewqueryscope-and-accessreviewinactiveusersqueryscope-to-configure-scope"></a>Usar accessReviewQueryScope e accessReviewInactiveUsersQueryScope para configurar o escopo

Para configurar o escopo usando o tipo **accessReviewQueryScope** , defina os valores de suas propriedades **query**, **queryRoot** e **queryType** . Para obter descrições dessas propriedades, consulte [o tipo de recurso accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope) .

**accessReviewInactiveUsersQueryScope** requer todas as propriedades de **accessReviewQueryScope** e inclui uma **propriedade inactiveDuration** .

### <a name="example-1-review-all-users-assigned-to-a-group"></a>Exemplo 1: Examinar todos os usuários atribuídos a um grupo

O exemplo a seguir define o escopo da revisão para membros diretos e transitivos do grupo que são usuários. Os membros transitivos são membros dos grupos aninhados.

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user",
    "queryType": "MicrosoftGraph"
}
```

**Cenário de exemplo:** Suponha que o grupo A tenha três membros diretos : usuários AU1 e AU2 e grupo G1. O grupo G1, por outro lado, tem dois membros : usuários GU1 e GU2. Os usuários GU1 e GU2 são, portanto, membros transitivos do grupo aninhado G1. Quatro objetos serão incluídos na revisão: usuários AU1, AU2, GU1 e GU2.

Para examinar *somente usuários inativos* atribuídos ao grupo:

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "inactiveDuration": "P30D",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user",
    "queryType": "MicrosoftGraph"
}
```

Este exemplo também define o escopo da revisão para membros diretos e transitivos do grupo que são usuários inativos.

### <a name="example-2-review-all-guest-users-assigned-to-a-group"></a>Exemplo 2: Examinar todos os usuários convidados atribuídos a um grupo

O exemplo a seguir define o escopo da revisão para membros diretos e transitivos do grupo que são usuários convidados. Os membros transitivos são membros dos grupos aninhados.

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-3-review-all-users-and-groups-assigned-to-a-group"></a>Exemplo 3: Examinar todos os usuários e grupos atribuídos a um grupo

O exemplo a seguir tem como escopo a revisão apenas para membros diretos do grupo que são usuários ou outros grupos. Neste escopo:
+ Os usuários diretos são incluídos na revisão.
+ Os grupos diretos estão incluídos na revisão.
+ Os membros transitivos dos grupos, ou seja, membros de grupos aninhados, não estão incluídos na revisão.

```http
"scope": {
        "query": "/groups/{group id}/members",
        "queryType": "MicrosoftGraph"
}
```

**Cenário de exemplo:** Suponha que o grupo A tenha três membros diretos : usuários AU1 e AU2 e grupo G1. O grupo G1, por outro lado, tem dois membros : usuários GU1 e GU2. Os usuários GU1 e GU2 são, portanto, membros transitivos do grupo aninhado G1. Somente três objetos são direcionados na revisão acima, usuários AU1 e AU2 e grupo G1.

### <a name="example-4-review-all-users-assigned-to-all-microsoft-365-groups"></a>Exemplo 4: Examinar todos os usuários atribuídos a todos os Microsoft 365 grupos

O exemplo a seguir cria uma revisão de cada grupo Microsoft 365 que contém usuários convidados. Para a instância de revisão em cada grupo, a revisão tem como escopo apenas membros diretos do grupo que são usuários convidados.

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified'))",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "./members/microsoft.graph.user",
    "queryType": "MicrosoftGraph"
}
```

Além disso, como essa revisão é aplicada em todos os grupos Microsoft 365, configure **o instanceEnumerationScope** para especificar os grupos Microsoft 365 a serem examinados. Grupos dinâmicos e grupos atribuíveis a funções não estão incluídos nesta revisão.

### <a name="example-5-review-all-guest-users-assigned-to-all-microsoft-365-groups"></a>Exemplo 5: Examinar todos os usuários convidados atribuídos a todos os Microsoft 365 grupos

O exemplo a seguir tem como escopo a revisão para membros diretos Microsoft 365 grupos que são usuários convidados.

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

Além disso, como essa revisão é aplicada em todos os grupos Microsoft 365, configure **o instanceEnumerationScope** para especificar os grupos Microsoft 365 a serem examinados. Grupos dinâmicos e grupos atribuíveis a funções não estão incluídos nesta revisão.

#### <a name="review-all-inactive-guest-users-assigned-to-all-microsoft-365-groups"></a>Examinar todos os usuários convidados inativos atribuídos a todos os Microsoft 365 grupos

O exemplo a seguir tem como escopo a revisão para membros diretos de Microsoft 365 que são usuários convidados inativos.

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified'))",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

Além disso, como essa revisão é aplicada a usuários inativos, use o recurso **accessReviewInactiveUsersQueryScope** e especifique **a propriedade @odata.type com** `#microsoft.graph.accessReviewInactiveUsersQueryScope`o valor . Grupos dinâmicos e grupos atribuíveis a funções não estão incluídos nesta revisão.

### <a name="example-6-review-all-guest-users-assigned-to-all-teams"></a>Exemplo 6: Examinar todos os usuários convidados atribuídos a todas as equipes

O exemplo a seguir tem como escopo a revisão para membros diretos de todas as equipes que são usuários convidados.

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
    
Além disso, como essa revisão é aplicada a todos os grupos de Teams habilitados para Microsoft 365, configure **o instanceEnumeration Teams Scope** para especificar os grupos de Microsoft 365 habilitados para Microsoft 365 para revisão. Grupos dinâmicos e grupos atribuíveis a funções não estão incluídos nesta revisão.

Essa revisão não incluirá usuários de conexão direta B2B em equipes com canais compartilhados. Para incluir usuários de conexão direta B2B em equipes com canais compartilhados, consulte o Exemplo 11: Examinar todos os usuários atribuídos a uma equipe, incluindo usuários do [B2B Direct Connect](#example-13-review-all-users-assigned-to-a-team-including-b2b-direct-connect-users-in-a-team-with-shared-channels) em uma equipe com canais compartilhados.

#### <a name="review-all-inactive-guest-users-assigned-to-all-teams"></a>Examinar todos os usuários convidados inativos atribuídos a todos os Teams

O exemplo a seguir tem como escopo a revisão para membros diretos de todas as equipes que são usuários convidados inativos.

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

Além disso, como essa revisão é aplicada em todas as equipes, configure a **propriedade instanceEnumerationScope** para especificar todas as equipes. Grupos dinâmicos e grupos atribuíveis a funções não estão incluídos nesta revisão.

Essa revisão não incluirá usuários de conexão direta B2B em equipes com canais compartilhados. Para incluir usuários de conexão direta B2B em equipes com canais compartilhados, consulte o Exemplo 11: Examinar todos os usuários atribuídos a uma equipe, incluindo usuários do [B2B Direct Connect](#example-11-review-all-users-assigned-to-a-team-including-b2b-direct-connect-users-in-a-team-with-shared-channels) em uma equipe com canais compartilhados.


---

### <a name="example-7-review-all-assignment-to-entitlement-management-access-packages"></a>Exemplo 7: Examinar todas as atribuições para pacotes de acesso do Gerenciamento de Direitos

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

---

### <a name="example-8-review-all-service-principals-assigned-to-a-privileged-role"></a>Exemplo 8: Examinar todas as entidades de serviço atribuídas a uma função com privilégios

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```
    
### <a name="example-9-review-all-users-assigned-to-a-privileged-role"></a>Exemplo 9: Examinar todos os usuários atribuídos a uma função privilegiada 

#### <a name="review-all-users-assigned-to-a-privileged-role-all-active-and-eligible-assignments-included"></a>Examinar todos os usuários atribuídos a uma função privilegiada (todas as atribuições ativas e qualificadas incluídas)

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleDefinitions/{role ID}",
    "queryType": "MicrosoftGraph"
}
```
    
#### <a name="review-all-users-with-eligible-assignment-to-a-privileged-role"></a>Examinar todos os usuários com atribuição qualificada para uma função privilegiada

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleEligibilityScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.user') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```
    
#### <a name="review-all-users-with-active-assignment-to-a-privileged-role"></a>Examinar todos os usuários com atribuição ativa a uma função privilegiada

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(assignmentType eq 'Assigned' and isof(principal,'microsoft.graph.user') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

---

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a>Usar principalResourceMembershipsScope para configurar o escopo

O **principalResourceMembershipsScope** expõe as propriedades **principalScopes** e **resourceScopes** para dar suporte a opções de configuração mais personalizadas para o escopo do objeto **accessReviewScheduleDefinition** . Os recursos incluem examinar o acesso de várias entidades de segurança ou grupos de entidades de segurança a vários recursos.

### <a name="example-10-review-all-inactive-guest-users-assigned-to-all-groups"></a>Exemplo 10: Examinar todos os usuários convidados inativos atribuídos a todos os grupos

O exemplo a seguir tem como escopo a revisão para membros diretos de todos os grupos que são usuários convidados inativos. Os usuários convidados são considerados usuários inativos quando o período de inatividade é de 30 dias a partir da data de início da instância de revisão de acesso.

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

### <a name="example-11-review-all-users-assigned-to-a-team-including-b2b-direct-connect-users-in-a-team-with-shared-channels"></a>Exemplo 11: Examinar todos os usuários atribuídos a uma equipe, incluindo usuários do B2B Direct Connect em uma equipe com canais compartilhados

Neste exemplo, o escopo de revisão de acesso é todos os usuários que são membros de uma equipe ou atribuídos a um canal compartilhado dentro da equipe. Esses membros incluem usuários internos, usuários diretos e transitivos, usuários de colaboração B2B e usuários do Direct Connect B2B.

```http
"scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/users",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "resourceScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/groups/{groupId}/transitiveMembers/microsoft.graph.user",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        },
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/teams/{groupId}/channels?$filter=(membershipType eq 'shared')",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ]
}
```

Para examinar usuários e equipes do B2B Direct Connect em canais compartilhados, `/teams/{groupId}/channels?$filter=(membershipType eq 'shared')` você deve especificar o padrão de consulta no **objeto resourceScopes**. Uma *revisão de todas* as equipes, como o [Exemplo 7](#example-7-review-all-inactive-guest-users-assigned-to-all-teams-direct-members-only), não incluirá usuários do B2B Direct Connect e equipes em canais compartilhados.

> [!NOTE]
> A revisão de acesso de usuários e equipes do B2B Direct Connect só tem suporte em revisões de acesso de estágio único e não em revisões de acesso de vários estágios.

### <a name="example-12-review-all-guest-users-assigned-to-a-directory-role"></a>Exemplo 12: Examinar todos os usuários convidados atribuídos a uma função de diretório

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

+ [Atribuir revisores à sua definição de revisão de acesso](/graph/accessreviews-reviewers-concept)
+ [Experimente tutoriais para](/graph/accessreviews-overview) saber como usar a API de revisões de acesso para examinar o acesso aos recursos do Azure AD
+ [Criar uma revisão de acesso](/azure/active-directory/governance/create-access-review)
