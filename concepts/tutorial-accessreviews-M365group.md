---
title: 'Tutorial: use a API de críticas de acesso para revisar o acesso de convidados aos grupos Microsoft 365 seus clientes'
description: Use a API de críticas de acesso para revisar o acesso de convidados aos grupos Microsoft 365 de convidados
author: FaithOmbongi
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: e27f8d8967bd9d3148759e692f3734e5c6018e54a01897d8d4a981c11bf8eabc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54186794"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-guest-access-to-your-microsoft-365-groups"></a>Tutorial: use a API de críticas de acesso para revisar o acesso de convidados aos grupos Microsoft 365 seus clientes

Neste tutorial, você usará o Graph Explorer para criar e ler críticas de acesso que direcionam todos os Microsoft 365 grupos com usuários convidados no locatário. Para isso, você primeiro usará o Azure AD B2B para convidar e criar um usuário convidado, também conhecido como identidade externa, em seu locatário. Em seguida, você adicionará esse usuário convidado ao seu grupo Microsoft 365 antes de criar e ler a revisão de acesso.

>[!NOTE]
>Os objetos de resposta mostrados neste tutorial podem ser reduzidos para a capacidade de leitura.

## <a name="prerequisites"></a>Pré-requisitos

Para concluir este tutorial, você precisa dos seguintes recursos e privilégios:

+ Um locatário do Azure AD funcionando com uma licença Azure AD Premium P2 ou EMS E5 habilitada. 
+ Uma conta em um locatário diferente do Azure AD ou uma identidade social que você pode convidar como usuário convidado (usuário B2B).
+ Entre no Graph [Explorer](https://developer.microsoft.com/graph/graph-explorer) como usuário em uma função de administrador global. 
+ As seguintes permissões delegadas: `User.Invite.All` , `AccessReview.ReadWrite.All` , , `Group.ReadWrite.All` `User.ReadWrite.All` .

Para consentir com as permissões necessárias no Graph Explorer:
1. Selecione o ícone de configurações à direita dos detalhes da conta do usuário e escolha **Selecionar permissões**.
   
   ![Selecionar as permissões do Microsoft Graph](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
   <!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Select the Microsoft Graph permissions":::-->

2. Role a lista de permissões para essas permissões:
   + AccessReview (3), expanda e selecione **AccessReview.ReadWrite.All**.
   + Grupo (2), expanda e selecione **Group.ReadWrite.All**.
   + Usuário (8), expanda e selecione **User.Invite.All** e **User.ReadWrite.All**.
   
   Selecione **Consentimento** e, em seguida, selecione **Aceitar** para aceitar o consentimento das permissões. Você não precisa consentir em nome da organização para essas permissões.
   
   ![Consentir com as permissões Graph Microsoft](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png)
   <!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png" alt-text="Consent to the Microsoft Graph permissions":::-->

## <a name="step-1-create-a-test-user-in-your-tenant"></a>Etapa 1: Criar um usuário de teste em seu locatário

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-createUser"
}-->

```http
POST /users
Content-Type: application/json

{
    "accountEnabled": true,
    "displayName": "Aline Dupuy",
    "mailNickname": "AlineD",
    "userPrincipalName": "AlineD@contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": true,
        "password": "xWwvJ]6NMw+bWH-d"
    }
}
```

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "c9a5aff7-9298-4d71-adab-0a222e0a05e4",
    "displayName": "Aline Dupuy",
    "userPrincipalName": "AlineD@contoso.com",
    "userType": "Member"
}
```

## <a name="step-2-invite-a-guest-user-into-your-tenant"></a>Etapa 2: convidar um usuário convidado para seu locatário

Convide um usuário convidado com o endereço de email **john@tailspintoys.com** seu locatário.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-inviteguest"
}-->

```http
POST https://graph.microsoft.com/beta/invitations
Content-Type: application/json

{
    "invitedUserDisplayName": "John Doe (Tailspin Toys)",
    "invitedUserEmailAddress": "john@tailspintoys.com",
    "sendInvitationMessage": false,
    "inviteRedirectUrl": "https://myapps.microsoft.com"
}
```

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#invitations/$entity",
    "invitedUser": {
        "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    }    
}
```

## <a name="step-3-create-a-new-microsoft-365-group-and-add-the-guest-user"></a>Etapa 3: criar um novo grupo Microsoft 365 e adicionar o usuário convidado

Nesta etapa:
1. Crie um novo grupo Microsoft 365 chamado **campanha de marketing Feelgood.**
2. Atribua a si mesmo como o proprietário do grupo.
3. Adicione john@tailspintoys.com como membro do grupo. O acesso ao grupo é assunto de revisão por você, o proprietário do grupo.

### <a name="request"></a>Solicitação

Nesta chamada, substitua:
+ `cdb555e3-b33e-4fd5-a427-17fadacbdfa7` com sua **id**. Para recuperar sua **id,** execute `GET` em `https://graph.microsoft.com/beta/me` .
+ `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` com **john@tailspintoys.com** **id** da resposta na Etapa 2.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-creategroup"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
    "description": "Feelgood Marketing Campaign with external partners and vendors.",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ],
    "mailEnabled": true,
    "mailNickname": "FeelGoodCampaign",
    "securityEnabled": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/beta/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    ]
}
```

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "59ab642a-2776-4e32-9b68-9ff7a47b7f6a",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ]
}
```

Agora você tem um grupo Microsoft 365 com um usuário convidado.

## <a name="step-4-create-an-access-review-for-all-microsoft-365-groups-with-guest-users"></a>Etapa 4: criar uma revisão de acesso para todos os grupos Microsoft 365 com usuários convidados

Ao criar uma série de revisão de acesso recorrente para todos os grupos de Microsoft 365 com usuários convidados, agende uma revisão periódica do acesso dos convidados ao grupo Microsoft 365 convidados. Faça isso para o **grupo Campanha de Marketing da Feelgood.**

A série de revisão de acesso usa as seguintes configurações:
+ É uma revisão de acesso recorrente e revisada trimestralmente.
+ Os proprietários do grupo analisam o acesso contínuo de usuários convidados.
+ O escopo de revisão está limitado a Microsoft 365 grupos com **usuários convidados** somente. Para obter mais opções para configurar o escopo, consulte a [seção Consulte também.](#see-also) 
+ Um revistor de backup. Pode ser um usuário de fallback ou um grupo que pode revisar o acesso caso o grupo não tenha proprietários atribuídos. Para obter mais opções para configurar os revisadores, consulte a [seção Consulte também.](#see-also)
+ **autoApplyDecisionsEnabled** está definido como `true` . Nesse caso, as decisões são aplicadas automaticamente quando o revistor conclui a revisão de acesso ou a duração da revisão de acesso termina. Se não estiver habilitado, um usuário deverá, após a conclusão da revisão, aplicar as decisões manualmente.
+ Aplique **a ação removeAccessApplyAction** a usuários convidados negados. Isso remove a associação no grupo do convidado negado. O usuário convidado ainda pode entrar no locatário.

### <a name="request"></a>Solicitação

Nesta chamada, substitua o seguinte:

+ `c9a5aff7-9298-4d71-adab-0a222e0a05e4` com a **id** do usuário que você está projetando como revistor de backup. Esta é a **id** da resposta na Etapa 1.
+ Valor de **startDate** com a data de hoje e o valor de **endDate** com uma data de um ano a partir da data de início. 

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "Group owners review guest across Microsoft 365 groups in the tenant (Quarterly)",
    "descriptionForAdmins": "",
    "descriptionForReviewers": "",
    "scope": {
        "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "./owners",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "backupReviewers": [
        {
            "query": "/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Approve",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "absoluteMonthly",
                "interval": 3,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-10",
                "endDate": "2022-12-21"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.removeAccessApplyAction"
            }
        ]
    }
}
```

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
    "id": "c22ae540-b89a-4d24-bac0-4ef35e6591ea",
    "displayName": "Group owners review guest across Microsoft 365 groups in the tenant (Quarterly)",
    "status": "NotStarted",
    "createdBy": {
        "id": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
    },
    "scope": {
        "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "./owners",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "backupReviewers": [
        {
            "query": "/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "settings": {
        "defaultDecisionEnabled": true,
        "defaultDecision": "Approve",
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "absoluteMonthly",
                "interval": 3,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-10",
                "endDate": "2022-12-21"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.removeAccessApplyAction"
            }
        ]
    }
}
```

## <a name="step-5-list-instances-of-the-access-review"></a>Etapa 5: Listar instâncias da revisão de acesso

A consulta a seguir lista todas as instâncias da definição de revisão de acesso. Se o locatário de teste contiver outros grupos Microsoft 365 com usuários convidados, essa solicitação retornará uma instância para cada grupo Microsoft 365 com usuários convidados no locatário.

### <a name="request"></a>Solicitação

Nesta chamada, substitua pela id da definição de revisão de `c22ae540-b89a-4d24-bac0-4ef35e6591ea` acesso retornada na Etapa 4. 

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-list_accessReviewInstance"
}-->
```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances
```

### <a name="response"></a>Resposta

Nesta resposta, o escopo inclui um grupo com **id** (o grupo de campanhas de marketing Feelgood criado na Etapa 3) porque tem `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` um usuário convidado. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances",
    "value": [
        {
            "id": "6392b1a7-9c25-4844-83e5-34e23c88e16a",
            "startDateTime": "2021-02-10T17:00:36.96Z",
            "endDateTime": "2021-02-10T17:00:36.96Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```
Nesta resposta, a instância de revisão de acesso atualmente é `InProgress` . Como essa é uma revisão trimestral, a cada três meses, uma nova instância de revisão é criada automaticamente e você, o revistor, pode aplicar novas decisões.

## <a name="step-6-get-decisions"></a>Etapa 6: Obter decisões

Obter as decisões tomadas para a instância de uma revisão de acesso.

### <a name="request"></a>Solicitação

Nesta chamada:
+ Substitua `c22ae540-b89a-4d24-bac0-4ef35e6591ea` pela **id da definição** de revisão de acesso retornada na Etapa 4.
+ Substitua pela id da sua instância de revisão `6392b1a7-9c25-4844-83e5-34e23c88e16a` de acesso retornada na Etapa 5. 

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-list_accessReviewInstanceDecisionItem"
}-->
```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances/6392b1a7-9c25-4844-83e5-34e23c88e16a/decisions
```

### <a name="response"></a>Resposta

A resposta a seguir mostra a decisão tomada para a instância da revisão.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances('6392b1a7-9c25-4844-83e5-34e23c88e16a')/decisions",
    "@odata.count": 1,
    "value": [
        {
            "id": "0e76ee07-b4c6-469e-bc9d-e73fc9a8d660",
            "accessReviewId": "6392b1a7-9c25-4844-83e5-34e23c88e16a",
            "reviewedDateTime": "2021-02-10T17:06:26.147Z",
            "decision": "Approve",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "AAD Access Reviews",
                "userPrincipalName": "AAD Access Reviews"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20",
                "userDisplayName": "John Doe (Tailspin Toys)",
                "userPrincipalName": "john@tailspintoys.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20",
                "displayName": "John Doe (Tailspin Toys)",
                "userPrincipalName": "john@tailspintoys.com"
            }
        }
    ]
}
```

Como esta é uma revisão trimestral e enquanto a definição ainda estiver ativa, ou seja, a recorrência **endDate** não é uma data passada, a cada três meses, quando uma nova instância de revisão é criada, você como o revistor pode aplicar novas decisões.

## <a name="step-7-clean-up-resources"></a>Etapa 7: Limpar recursos

Exclua os recursos criados para este tutorial: grupo de campanhas de **marketing feelgood,** definição de agenda de revisão de acesso, usuário convidado e usuário de teste.

### <a name="delete-the-microsoft-365-group"></a>Excluir o Microsoft 365 grupo

#### <a name="request"></a>Solicitação

Nesta chamada, substitua pela id da sua campanha de `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` **marketing do Feelgood**  Microsoft 365 grupo.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-access-review-definition"></a>Excluir a definição de revisão de acesso

Nesta chamada, substitua pela id da `c22ae540-b89a-4d24-bac0-4ef35e6591ea` **sua definição** de revisão de acesso. Como a definição de agenda de revisão de acesso é o modelo para a revisão de acesso, excluir a definição removerá as configurações, instâncias e decisões associadas à revisão de acesso.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="remove-the-guest-user"></a>Remover o usuário convidado

Nesta chamada, substitua `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` pela **id** do usuário convidado, john@tailspintoys.com.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-test-user"></a>Excluir o usuário de teste
Nesta chamada, substitua `c9a5aff7-9298-4d71-adab-0a222e0a05e4` pela **id do** usuário de teste.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_guestuser"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

Parabéns! Você criou uma revisão de acesso para todos os usuários convidados Microsoft 365 grupos em seu locatário e agendou trimestralmente para a avaliação e atestado do acesso dos usuários convidados. Os proprietários do grupo revisarão o acesso durante esses ciclos, escolhendo aprovar ou negar o acesso.

## <a name="see-also"></a>Confira também

+ [Referência da API de avaliações do Access](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)
+ [Configurar o escopo de sua definição de revisão de acesso usando a API Graph Microsoft](/graph/accessreviews-scope-concept)
+ [Atribuir revisadores à sua definição de revisão de acesso usando a API Graph Microsoft](/graph/accessreviews-reviewers-concept)
+ [Visão geral de avaliações do Access e requisitos de licença](/azure/active-directory/governance/access-reviews-overview)
+ [Criar uma revisão de acesso de grupos & aplicativos](/azure/active-directory/governance/create-access-review)
+ [Convidar/adicionar usuários convidados à sua organização](/graph/api/resources/invitation?view=graph-rest-beta&preserve-view=true)
+ [Referência da API de Avaliações do Access](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)
+ [Criar accessReviewScheduleDefinition](/graph/api/accessreviewscheduledefinition-create?view=graph-rest-beta&preserve-view=true)
+ [Listar accessReviewInstance](/graph/api/accessreviewinstance-list?view=graph-rest-beta&preserve-view=true)
+ [Listar accessReviewInstanceDecisionItem](/graph/api/accessreviewinstancedecisionitem-list?view=graph-rest-beta&preserve-view=true)
