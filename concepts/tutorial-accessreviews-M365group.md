---
title: 'Tutorial: use a API de críticas de acesso para revisar o acesso de convidados aos grupos Microsoft 365 seus clientes'
description: Use a API de críticas de acesso para revisar o acesso de convidados aos grupos Microsoft 365 seus clientes
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: f2c9210b4173850c6fbccaad352c88b894965e29
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334916"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-guest-access-to-your-microsoft-365-groups"></a>Tutorial: use a API de críticas de acesso para revisar o acesso de convidados aos grupos Microsoft 365 seus clientes

A API de revisões de acesso no Microsoft Graph permite que as organizações auditem e atestem o acesso que as identidades (também chamadas de *entidades) são atribuídas* aos recursos na organização. Na colaboração entre locatários, os usuários externos podem ter recursos de acesso, como arquivos, anotações, calendários e até mesmo Teams conversas. Esse acesso pode ser gerenciado com eficiência por meio Microsoft 365 grupos. Usando a API de revisões de acesso, as organizações podem, portanto, atestar periodicamente as entidades que têm acesso a esses grupos e, por extensão, outros recursos na organização.

Vamos supor que você concedeu acesso a usuários externos (também chamados de usuários *convidados) aos* recursos em sua organização por meio Microsoft 365 grupos. Este tutorial orientará você a revisar o acesso deles aos grupos Microsoft 365 em seu locatário.

>[!NOTE]
>Os objetos de resposta mostrados neste tutorial podem ser reduzidos para a capacidade de leitura.

## <a name="prerequisites"></a>Pré-requisitos

Para concluir este tutorial, você precisa dos seguintes recursos e privilégios:

+ Um locatário do Azure AD funcionando com uma licença Azure AD Premium P2 ou EMS E5 habilitada. 
+ Uma conta em um locatário diferente do Azure AD ou uma identidade social que você pode convidar como usuário convidado (usuário B2B).
+ Entre no Graph [Explorer](https://developer.microsoft.com/graph/graph-explorer) como usuário em uma função de administrador global. 
+ As seguintes permissões delegadas: `User.Invite.All`, , `AccessReview.ReadWrite.All`, `Group.ReadWrite.All``User.ReadWrite.All`.

Para consentir com as permissões necessárias no Graph Explorer:
1. Selecione o ícone de configurações à direita dos detalhes da conta do usuário e escolha **Selecionar permissões**.
   
   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Selecione Permissões Graph Microsoft." border="true":::

2. Role a lista de permissões para essas permissões:
   + AccessReview (3), expanda e selecione **AccessReview.ReadWrite.All**.
   + Grupo (2), expanda e selecione **Group.ReadWrite.All**.
   + Usuário (8), expanda e selecione **User.Invite.All** e **User.ReadWrite.All**.
   
   Selecione **Consentimento** e, em seguida, selecione **Aceitar** para aceitar o consentimento das permissões. Você não precisa consentir em nome da sua organização para essas permissões.
   
   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="Consentimento para permissões Graph Microsoft." border="true":::

## <a name="step-1-create-a-test-user-in-your-tenant"></a>Etapa 1: Criar um usuário de teste em seu locatário

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-createUser"
}-->

```http
POST https://graph.microsoft.com/v1.0/users
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
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
POST https://graph.microsoft.com/v1.0/invitations
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#invitations/$entity",
    "invitedUser": {
        "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    }    
}
```

## <a name="step-3-create-a-new-microsoft-365-group-and-add-the-guest-user"></a>Etapa 3: criar um novo grupo Microsoft 365 e adicionar o usuário convidado

Nesta etapa:
1. Crie um novo grupo Microsoft 365 chamado **Boa campanha de marketing**.
2. Atribua a si mesmo como o proprietário do grupo.
3. Adicione john@tailspintoys.com como membro do grupo. O acesso ao grupo é assunto de revisão por você, o proprietário do grupo.

### <a name="request"></a>Solicitação

Nesta chamada, substitua:
+ `cdb555e3-b33e-4fd5-a427-17fadacbdfa7` com sua ID. Para recuperar sua ID, execute `GET` em `https://graph.microsoft.com/v1.0/me`.
+ `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` com **john@tailspintoys.com** ID da resposta na Etapa 2.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-creategroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
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
        "https://graph.microsoft.com/v1.0/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/v1.0/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "59ab642a-2776-4e32-9b68-9ff7a47b7f6a",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ]
}
```

Agora você tem um grupo Microsoft 365 com um usuário convidado.

## <a name="step-4-create-an-access-review-for-all-microsoft-365-groups-with-guest-users"></a>Etapa 4: criar uma revisão de acesso para todos os grupos Microsoft 365 com usuários convidados

Ao criar uma série de revisão de acesso recorrente para todos os grupos Microsoft 365 com usuários convidados, agende uma revisão periódica do acesso dos convidados ao grupo Microsoft 365 convidados. Nesse caso, o grupo **Campanha de Marketing se sente** bem.

A série de revisão de acesso usa as seguintes configurações:
+ É uma revisão de acesso recorrente e revisada trimestralmente.
+ Os proprietários do grupo decidem se os usuários convidados devem manter seu acesso.
+ O escopo de revisão é limitado apenas Microsoft 365 grupos com **usuários convidados**.
+ Um revistor de backup. Eles podem ser um usuário de fallback ou um grupo que pode revisar o acesso caso o grupo não tenha proprietários atribuídos.
+ **autoApplyDecisionsEnabled** está definido como `true`. Nesse caso, as decisões são aplicadas automaticamente quando o revistor conclui a revisão de acesso ou a duração da revisão de acesso termina. Se não estiver habilitado, um usuário deverá aplicar as decisões manualmente após a conclusão da revisão.
+ Aplique a **ação removeAccessApplyAction** aos usuários convidados negados para removê-los do grupo. O usuário convidado ainda pode entrar no locatário, mas não acessará o grupo.

### <a name="request"></a>Solicitação

Nesta chamada, substitua os seguintes valores:

+ `c9a5aff7-9298-4d71-adab-0a222e0a05e4` com a ID de Aline que você está projetando como revistor de backup.
+ Valor de **startDate** com a data de hoje e o valor de **endDate** com uma data de um ano a partir da data de início. 

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions
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
    "fallbackReviewers": [
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions/$entity",
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
    "fallbackReviewers": [
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

A consulta a seguir lista todas as instâncias da definição de revisão de acesso. Se houver mais de um grupo Microsoft 365 com usuários convidados em seu locatário, essa solicitação retornará uma instância para cada grupo Microsoft 365 *com usuários convidados*.

### <a name="request"></a>Solicitação

Nesta chamada, substitua pela `c22ae540-b89a-4d24-bac0-4ef35e6591ea` ID da definição de revisão de acesso retornada na Etapa 4.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-list_accessReviewInstance"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances
```

### <a name="response"></a>Resposta

Nesta resposta, o escopo `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` inclui um grupo identificado por (o grupo de campanhas de **marketing** Sentir-se bem criado na Etapa 3) porque ele tem um usuário convidado.

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances",
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
Nesta resposta, a instância de revisão de acesso atualmente é `InProgress`. Como é uma revisão trimestral, uma nova instância de revisão é criada automaticamente a cada três meses e os revisadores podem aplicar novas decisões.

## <a name="step-6-get-decisions"></a>Etapa 6: Obter decisões

Obter as decisões tomadas para a instância de uma revisão de acesso.

### <a name="request"></a>Solicitação

Nesta chamada:
+ Substitua `c22ae540-b89a-4d24-bac0-4ef35e6591ea` pela ID da definição de revisão de acesso retornada na Etapa 4.
+ Substitua `6392b1a7-9c25-4844-83e5-34e23c88e16a` pela ID da sua instância de revisão de acesso retornada na Etapa 5.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-list_accessReviewInstanceDecisionItem"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances/6392b1a7-9c25-4844-83e5-34e23c88e16a/decisions
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances('6392b1a7-9c25-4844-83e5-34e23c88e16a')/decisions",
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

Em uma revisão trimestral como esta e desde que a revisão de acesso ainda esteja ativa:
+ A cada três meses, uma nova instância de revisão será criada.
+ Os revisadores serão obrigados a aplicar novas decisões para novas instâncias.


## <a name="step-7-clean-up-resources"></a>Etapa 7: Limpar recursos

Exclua os recursos que você criou para este tutorial— Sinta-se bem em grupo de campanha de **marketing** , a definição do agendamento de revisão de acesso, o usuário convidado e o usuário de teste.

### <a name="delete-the-microsoft-365-group"></a>Excluir o Microsoft 365 grupo

#### <a name="request"></a>Solicitação

Nesta chamada, substitua pela `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` ID da sua campanha de **marketing** De boa Microsoft 365 grupo.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a
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

Nesta chamada, substitua pela `c22ae540-b89a-4d24-bac0-4ef35e6591ea` ID da sua definição de revisão de acesso. Como a definição do cronograma de revisão de acesso é o modelo para a revisão de acesso, excluir a definição removerá as configurações, instâncias e decisões relacionadas.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea
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

Nesta chamada, substitua `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` pela ID do usuário convidado, john@tailspintoys.com.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20
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
Nesta chamada, substitua `c9a5aff7-9298-4d71-adab-0a222e0a05e4` pela ID do usuário de teste.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_guestuser"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4
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

Parabéns! Você criou uma revisão de acesso para usuários convidados Microsoft 365 grupos em seu locatário e agendou-a trimestralmente. Os proprietários do grupo revisarão o acesso durante esses ciclos, escolhendo aprovar ou negar o acesso.

## <a name="see-also"></a>Confira também


+ [API de avaliações do Access](/graph/api/resources/accessreviewsv2-overview)
+ [O que são avaliações de acesso do Azure AD?](/azure/active-directory/governance/access-reviews-overview)
+ [Revisar o acesso a grupos e aplicativos em avaliações de acesso do Azure AD](/azure/active-directory/governance/perform-access-review)