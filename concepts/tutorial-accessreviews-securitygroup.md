---
title: 'Tutorial: Usar a API de revisões de acesso para examinar o acesso aos seus grupos de segurança'
description: Saiba como usar a API de revisões de acesso para examinar o acesso a um grupo de segurança em seu locatário do Azure AD e testar chamadas à API antes de automatizá-las em scripts ou aplicativos.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 7f64afebad0057b305aa5c3dc2544753aad8d25f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443806"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-access-to-your-security-groups"></a>Tutorial: Usar a API de revisões de acesso para examinar o acesso aos seus grupos de segurança

A API de revisões de acesso no Microsoft Graph permite que as organizações auditem e atestem o acesso de que as identidades (também chamadas de entidades de segurança) são *atribuídas* aos recursos na organização. Um dos métodos mais eficientes e eficazes para gerenciar privilégios de acesso para entidades de segurança para outros recursos é por meio Azure AD de segurança. Por exemplo, centenas de usuários podem ser atribuídos a um grupo de segurança e ao grupo de segurança atribuído acesso a uma pasta. Usando a API de revisões de acesso, as organizações podem atestar periodicamente as entidades de segurança que têm acesso a esses grupos e, por extensão, a outros recursos na organização.

Suponha que você use Azure AD de segurança para atribuir acesso a identidades (também chamadas de *entidades* de segurança) aos recursos em sua organização. Periodicamente, você precisa atestar que todos os membros do grupo de segurança precisam de sua associação e, por extensão, seu acesso aos recursos atribuídos ao grupo de segurança.

Este tutorial orienta você a usar a API de revisões de acesso para examinar o acesso a um grupo de segurança em seu Azure AD locatário. Você pode usar o Explorador do Graph ou o Postman para testar suas chamadas à API de revisões de acesso antes de automatizá-las em um script ou um aplicativo. Esse ambiente de teste economiza tempo, ajudando você a definir e validar corretamente suas consultas sem recompilar repetidamente seu aplicativo.

## <a name="prerequisites"></a>Pré-requisitos

Para concluir este tutorial, você precisa dos seguintes recursos e privilégios:

+ Um locatário Azure AD trabalho com uma licença Azure AD Premium P2 ou EMS E5 habilitada.
+ Entre no [Explorador do Graph como](https://developer.microsoft.com/graph/graph-explorer) um usuário em uma função administrador global ou administrador de governança de identidade Azure AD função.
  + [Opcional] Abra uma nova **janela do navegador anônima****, anônima** ou **InPrivate**. Você entrará mais adiante neste tutorial.
+ As seguintes permissões delegadas: `AccessReview.ReadWrite.All`, `Group.ReadWrite.All`.

Para consentir com as permissões necessárias no Explorador do Graph:
1. Selecione o ícone de engrenagem de configurações à direita dos detalhes da conta de usuário e selecione **Selecionar permissões**.

    :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Selecione as permissões do Microsoft Graph." border="true":::

2. Percorra a lista de permissões para estas permissões:
   + AccessReview (3), expanda e selecione **AccessReview.ReadWrite.All**.
   + Agrupar (2), expandir e selecionar **Group.ReadWrite.All**.
  
    Selecione **Consentimento** e, na janela pop-up, escolha Consentir  em nome de sua organização e, em seguida, selecione Aceitar para aceitar o consentimento das permissões.

   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="Consentir com permissões do Microsoft Graph." border="true":::
   
>[!NOTE]
>Os objetos de resposta mostrados neste tutorial podem ser reduzidos para legibilidade.
   
## <a name="step-1-create-test-users-in-your-tenant"></a>Etapa 1: Criar usuários de teste em seu locatário

Crie três novos usuários de teste executando a solicitação abaixo de três vezes, alterando os valores das propriedades **displayName**, **mailNickname** e **userPrincipalName** a cada vez. Registre as IDs dos três novos usuários de teste.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-createUser"
}-->
```http
POST https://graph.microsoft.com/v1.0/users
Content-Type: application/json

{
    "accountEnabled": true,
    "displayName": "Adele Vance",
    "mailNickname": "AdeleV",
    "userPrincipalName": "AdeleV@Contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": true,
        "password": "xWwvJ]6NMw+bWH-d"
    }
}
```

### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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
    "id": "3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
    "displayName": "Adele Vance",
    "userPrincipalName": "AdeleV@Contoso.com"
}
```

## <a name="step-2-create-a-security-group-assign-owners-and-add-members"></a>Etapa 2: Criar um grupo de segurança, atribuir proprietários e adicionar membros

Crie um grupo de segurança chamado **Building security** que seja o destino das revisões de acesso neste tutorial. Atribua a esse grupo um proprietário de grupo e dois membros.

### <a name="request"></a>Solicitação

Na etapa anterior, você criou três usuários de teste. Um dos usuários será o proprietário do grupo, enquanto os outros dois serão membros do grupo.

Nesta chamada, substitua:
+ `d3bcdff4-4f80-4418-a65e-7bf3778c5dca` com a ID do proprietário do grupo.
+ `3b8ceebc-49e6-4e0c-9e14-c906374a7ef6` e `bf59c5ba-5304-4c9b-9192-e5a4cb8444e7` com as IDs dos dois membros do grupo.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-creategroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
    "description": "Building security",
    "displayName": "Building security",
    "groupTypes": [],
    "mailEnabled": false,
    "mailNickname": "buildingsecurity",
    "securityEnabled": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/beta/users/d3bcdff4-4f80-4418-a65e-7bf3778c5dca"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
        "https://graph.microsoft.com/beta/users/bf59c5ba-5304-4c9b-9192-e5a4cb8444e7"
    ]
}
```

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
    "description": "Building security",
    "displayName": "Building security",
    "mailNickname": "buildingsecurity",
    "securityEnabled": true
}
```

Na resposta, registre a ID do novo grupo para usá-la posteriormente neste tutorial.

## <a name="step-3-create-an-access-review-for-the-security-group"></a>Etapa 3: Criar uma revisão de acesso para o grupo de segurança

### <a name="request"></a>Solicitação

Nesta chamada, substitua os seguintes valores:
+ `eb75ccd2-59ef-48b7-8f76-cc3f33f899f4` com a ID do **grupo de segurança de** construção. O escopo especifica que a revisão é aplicada a todos os membros do **grupo de segurança building** . Para obter mais opções para configurar o escopo, consulte a [seção](#see-also) Consulte também.
+ Valor de **startDate** com a data de hoje e o valor de **endDate** com uma data de cinco dias a partir da data de início.

A revisão de acesso tem as seguintes configurações:

+ É uma auto-revisão como inferida quando você não especifica um valor para a propriedade **dos revisores** . Portanto, cada membro do grupo atestará automaticamente a necessidade de manter o acesso ao grupo.
+ O escopo da revisão são membros (diretos e indiretos) do **grupo de segurança de** criação.
+ O revistor deve fornecer uma justificativa para o motivo pelo qual ele precisa manter o acesso ao grupo.
+ A decisão padrão é `Deny` quando os revisores não respondem à solicitação de revisão de acesso antes que a instância expire. A `Deny` decisão remove os membros do grupo.
+ É uma revisão de acesso única que termina após cinco dias. Portanto, depois que o acesso for concedido, o usuário não precisará atestar novamente dentro do período de revisão de acesso.
+ As entidades de segurança definidas no escopo da revisão receberão notificações por email e lembretes solicitando que eles autotestem a necessidade de manter o acesso.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "One-time self-review for members of Building security",
    "descriptionForAdmins": "One-time self-review for members of Building security",
    "descriptionForReviewers": "One-time self-review for members of Building security",
    "scope": {
        "query": "/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
        "queryType": "MicrosoftGraph"
    },
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 5,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2022-02-11",
                "endDate": "2022-02-16"
            }
        }
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
    "id": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
    "displayName": "One-time self-review for members of Building security",
    "createdDateTime": null,
    "lastModifiedDateTime": null,
    "status": "NotStarted",
    "descriptionForAdmins": "One-time self-review for members of Building security",
    "descriptionForReviewers": "One-time self-review for members of Building security",
    "createdBy": {
        "id": "bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
        "displayName": "MOD Administrator",
        "type": null,
        "userPrincipalName": "admin@Contoso.com"
    },
    "scope": {},
    "instanceEnumerationScope": {},
    "reviewers": [],
    "fallbackReviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 5,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2022-02-11",
                "endDate": "2022-02-16"
            }
        },
        "applyActions": []
    },
    "additionalNotificationRecipients": []
}
```

O status da revisão de acesso acima é marcado **como NotStarted**. Você pode recuperar a revisão de acesso (GET `https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b`) para monitorar o status e, quando ele estiver marcado como **InProgress**, as instâncias foram criadas para a revisão de acesso e as decisões podem ser postadas. Você também pode recuperar a revisão de acesso para ver as configurações completas da revisão de acesso.

## <a name="step-4-list-instances-of-the-access-review"></a>Etapa 4: Listar instâncias da revisão de acesso

Depois que **o status** da revisão de acesso for marcado `InProgress`como , execute a consulta a seguir para listar todas as instâncias da definição de revisão de acesso. Como você criou uma revisão de acesso única na Etapa 3, a solicitação retorna apenas uma instância com uma ID como a ID da definição de agenda.

### <a name="request"></a>Solicitação

Nesta chamada, substitua pela `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` ID da definição de revisão de acesso retornada na Etapa 3.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_accessReviewInstance"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances
```

### <a name="response"></a>Resposta

Nessa resposta, o **status da** instância `InProgress` ocorre porque **startDateTime** é passado e **endDateTime** está no futuro. Se **startDateTime** estiver no futuro, o status será `NotStarted`. Por outro lado, se **endDateTime** estiver no passado, o status será `Completed`.

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/instances",
    "value": [
        {
            "id": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
            "startDateTime": "2022-02-11T17:35:25.24Z",
            "endDateTime": "2022-02-16T08:00:00Z",
            "status": "InProgress",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4/transitiveMembers/microsoft.graph.user",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            "reviewers": [],
            "fallbackReviewers": []
        }
    ]
}
```

## <a name="step-5-who-was-contacted-for-the-review"></a>Etapa 5: Quem foi contatado para a revisão?

Você pode confirmar que todos os membros do  grupo de segurança do Edifício foram contatados para postar suas decisões de revisão para esta instância da revisão de acesso.

### <a name="request"></a>Solicitação

Nesta chamada, substitua pela `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` ID da definição da agenda de revisão de acesso.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_contactedReviewers"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/contactedReviewers
```

### <a name="response"></a>Resposta

A resposta a seguir mostra que os dois membros **do grupo de** segurança building foram notificados sobre sua revisão pendente.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewReviewer",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/instances('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/contactedReviewers",
    "@odata.count": 2,
    "value": [
        {
            "id": "3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
            "displayName": "Adele Vance",
            "userPrincipalName": "AdeleV@Contoso.com",
            "createdDateTime": "2022-02-11T17:35:34.4092545Z"
        },
        {
            "id": "bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
            "displayName": "Alex Wilber",
            "userPrincipalName": "AlexW@Contoso.com",
            "createdDateTime": "2022-02-11T17:35:34.4092545Z"
        }
    ]
}
```

## <a name="step-6-get-decisions"></a>Etapa 6: Obter decisões

Você está interessado nas decisões tomadas para a instância da revisão de acesso.

### <a name="request"></a>Solicitação

Nessa chamada, substitua pela `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` ID da definição da agenda de revisão de acesso e pela instância.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_accessReviewInstanceDecisionItem"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions
```

### <a name="response"></a>Resposta

A resposta a seguir mostra as decisões tomadas na instância da revisão. Como **o Building Security** tem dois membros, dois itens de decisão são esperados.

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/instances('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "4db68765-472d-4aa2-847a-433ea94bcfaf",
            "accessReviewId": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
            "resourceLink": "https://graph.microsoft.com/v1.0/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "resource": {
                "id": "eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
                "displayName": "Building security",
                "type": "group"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
                "displayName": "Alex Wilber",
                "type": "user",
                "userPrincipalName": "AlexW@Contoso.com",
                "lastUserSignInDateTime": "2/11/2022 5:31:37 PM +00:00"
            }
        },
        {
            "id": "c7de8fba-4d6a-4fab-a659-62ff0c02643d",
            "accessReviewId": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
            "resourceLink": "https://graph.microsoft.com/v1.0/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "resource": {
                "id": "eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
                "displayName": "Building security",
                "type": "group"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
                "displayName": "Adele Vance",
                "type": "user",
                "userPrincipalName": "AdeleV@Contoso.com",
                "lastUserSignInDateTime": "2/11/2022 4:58:13 PM +00:00"
            }
        }
    ]
}
```

Na chamada, a **propriedade de** decisão tem `NotReviewed` o valor de porque os membros do grupo não concluiram o autoteste. Siga a Etapa 7 para saber como cada membro pode atestar automaticamente sua necessidade de revisão de acesso.

## <a name="step-7-self-review-a-pending-access-decision"></a>Etapa 7: revisar automaticamente uma decisão de acesso pendente

Na Etapa 3, você configurou a revisão de acesso como auto-revisão. Essa configuração exige que ambos os membros do grupo de **segurança de construção** autotestem sua necessidade de manter o acesso ao grupo.

>[!NOTE]
>Conclua esta etapa como um dos dois membros do **grupo de segurança De** construção.

Nesta etapa, você lista as revisões de acesso pendentes e, em seguida, conclui o processo de autoteste. Você pode concluir essa etapa de uma das duas maneiras, usando a API ou o [portal Meus Acessos](https://myaccess.microsoft.com/). O outro revisador não concluirá esse processo e, em vez disso, você permitirá que as decisões padrão sejam aplicadas à revisão de acesso.

Inicie uma nova **sessão** de navegador de navegação **anônima, anônima** ou **InPrivate** e entre como um dos dois membros do **grupo de segurança De** construção. Ao fazer isso, você não interromperá sua sessão de administrador atual. Entraremos como Adele Vance. Como alternativa, você pode interromper a sessão de administrador atual fazendo logon no Explorador do Graph e fazendo logon novamente como um dos dois membros do grupo.

### <a name="method-1-use-the-access-reviews-api-to-self-review-pending-access"></a>Método 1: Usar a API de revisões de acesso para auto-examinar o acesso pendente

#### <a name="list-your-access-reviews-decision-items"></a>Listar seus itens de decisão de revisões de acesso

Nesta chamada, substitua pela `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` ID da definição da agenda de revisão de acesso.

##### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/v1.0/identitygovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions/filterByCurrentUser(on='reviewer')
```

##### <a name="response"></a>Resposta
Na resposta abaixo, você (Adele Vance) tem uma revisão de **acesso pendente (**`NotReviewed`a decisão é) para atestar automaticamente. As **propriedades de** **entidade de** segurança e recurso indicam a entidade de segurança à qual a decisão se aplica e o recurso ao qual o acesso está sob revisão. Nesse caso, Adele Vance e o **grupo de segurança do** Edifício, respectivamente.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(accessReviewInstanceDecisionItem)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
            "id": "c7de8fba-4d6a-4fab-a659-62ff0c02643d",
            "accessReviewId": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
            "resourceLink": "https://graph.microsoft.com/v1.0/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "resource": {
                "id": "eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
                "displayName": "Building security",
                "type": "group"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
                "displayName": "Adele Vance",
                "type": "user",
                "userPrincipalName": "AdeleV@Contoso.com",
                "lastUserSignInDateTime": "2/15/2022 9:35:23 AM +00:00"
            }
        }
    ]
}
```

#### <a name="record-a-decision"></a>Registrar uma decisão

Para concluir a revisão de acesso, Adele Vance confirmará a necessidade de manter o acesso ao **grupo de segurança building** .

##### <a name="request"></a>Solicitação

Nesta chamada, substitua pela `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` ID `c7de8fba-4d6a-4fab-a659-62ff0c02643d` da definição da agenda de revisão de acesso e pela ID do item de decisão pendente retornado na etapa anterior.

```http
PATCH https://graph.microsoft.com/v1.0/identitygovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions/c7de8fba-4d6a-4fab-a659-62ff0c02643d

{
    "decision": "Approve",
    "justification": "As the assistant security manager, I still need access to the building security group."
}
```

##### <a name="response"></a>Resposta

```http
HTTP/1.1 204 No Content
```


#### <a name="verify-the-decisions"></a>Verificar as decisões

Para verificar as decisões que você registrou para sua revisão de acesso, [liste os itens de decisão de revisão de acesso](#list-your-access-reviews-decision-items). Embora o período de revisão de acesso não tenha expirado nem as decisões se apliquem, **o applyResult** `New` será marcado como e você terá permissão para alterar a decisão.

Agora você pode sair e sair da sessão anônima do navegador.

### <a name="method-2-use-the-my-access-portal"></a>Método 2: Usar o portal Meus Acessos

Os revisores também podem visitar o [portal Meus Acessos](https://myaccess.microsoft.com/) para verificar suas instâncias de revisão de acesso pendentes.

+ Liste as revisões de acesso pendentes. O usuário pode seguir uma das duas maneiras de chegar lá:
  + Opção 1: selecione **o botão Revisar acesso** na notificação por email recebida na caixa de entrada de email. A notificação por email é semelhante à captura de tela a seguir. Selecionar esse botão direciona-os para a revisão de acesso pendente.

  :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/emailnotification.png" alt-text="Notificação por email para examinar seu acesso." border="true":::

  + Opção 2: acesse o [portal Meus Acessos](https://myaccess.microsoft.com/) . Selecione o menu **revisões do Access** e selecione a **guia Grupos e** Aplicativos.

+ Na lista de revisões de acesso, selecione a revisão de acesso para a qual você deseja postar a decisão. Selecione **Sim** para postar a decisão de que você ainda precisa de acesso ao **Building Security**. Insira um motivo e selecione **Enviar**.

  :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/selfattest.png" alt-text="Autoteste a necessidade de manter o acesso a um recurso.":::


Agora você pode sair e sair da sessão anônima do navegador.

## <a name="step-8-confirm-the-decisions-and-the-status-of-the-access-review"></a>Etapa 8: Confirmar as decisões e o status da revisão de acesso

De volta à sessão principal do navegador em que você ainda está conectado como administrador global, repita a Etapa 4 para ver se a propriedade de  decisão de Adele Vance está agora`Approve`. Quando a revisão de acesso terminar ou expirar, a decisão padrão `Deny` será registrada para Alex Wilber. As decisões serão aplicadas automaticamente porque **o autoApplyDecisionsEnabled** `true` foi definido como e o período da instância de revisão de acesso terá terminado. Adele manterá o acesso ao grupo de **segurança** building e Alex será removido automaticamente do grupo.

Parabéns! Você criou uma revisão de acesso e autotestou sua necessidade de manter o acesso. Você só autotestou `Deny` uma vez e manterá o acesso até que ele seja removido por meio de uma decisão de outra instância de revisão de acesso ou por meio de outro processo interno.

## <a name="step-9-clean-up-resources"></a>Etapa 9: Limpar recursos

Exclua os recursos que você criou para este tutorial **– o grupo** de segurança de criação, a definição do agendamento de revisão de acesso e os três usuários de teste.

### <a name="delete-the-security-group"></a>Excluir o grupo de segurança

#### <a name="request"></a>Solicitação

Nesta chamada, substitua pela `eb75ccd2-59ef-48b7-8f76-cc3f33f899f4` **ID de** Segurança **de construção**.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="delete-the-access-review-definition"></a>Excluir a definição de revisão de acesso

Nesta chamada, substitua pela `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` ID da definição de revisão de acesso. Como a definição do agendamento de revisão de acesso é o blueprint para a revisão de acesso, a exclusão da definição removerá as configurações, instâncias e decisões.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="delete-the-three-test-users"></a>Excluir os três usuários de teste
Nessa chamada, substitua pela `3b8ceebc-49e6-4e0c-9e14-c906374a7ef6` ID de um de seus usuários de teste. Repita essa etapa duas vezes com as IDs dos outros dois usuários para excluí-las.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="conclusion"></a>Conclusão

Você criou uma revisão de acesso na qual as entidades de segurança autotestam a necessidade de manter o acesso a um recurso, nesse caso, o grupo **de** segurança building.

Este tutorial demonstrou um dos cenários pela API de Azure AD de acesso. A API de revisões de acesso dá suporte a diferentes cenários por meio de uma combinação de recursos, entidades de segurança e revisores para atender às suas necessidades de atestado de acesso. Para obter mais informações, consulte a [API de revisões de acesso](/graph/api/resources/accessreviewsv2-overview).

## <a name="see-also"></a>Confira também

+ [O que são Azure AD revisões de acesso?](/azure/active-directory/governance/access-reviews-overview)
+ [Examine o acesso para você mesmo a grupos ou aplicativos Azure AD revisões de acesso](/azure/active-directory/governance/review-your-access)