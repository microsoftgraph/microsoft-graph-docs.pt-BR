---
title: 'Tutorial: use a API de críticas de acesso para revisar o acesso a funções privilegiadas'
description: Usar a API de críticas de acesso para revisar o acesso a funções privilegiadas
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: adc20b128a56094a0281589d38f9e99b1767b432
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337890"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-access-to-privileged-roles"></a>Tutorial: use a API de críticas de acesso para revisar o acesso a funções privilegiadas

A API de revisões de acesso no Microsoft Graph permite que as organizações auditem e atestem o acesso que as identidades (também chamadas de *entidades) são atribuídas* aos recursos na organização. Um dos recursos mais confidenciais de uma organização são funções privilegiadas. Com uma função privilegiada, uma entidade pode executar operações administrativas. Dependendo da função privilegiada, algumas operações podem ter um efeito maior na postura de segurança da organização. Usando a API de revisões de acesso, as organizações podem atestar periodicamente as entidades que têm acesso a funções privilegiadas de acordo com a política da organização.

A Contoso Limited é um provedor de serviços em crescimento que delegou vários privilégios de administrador do Azure AD a usuários, grupos e entidades de serviço na organização. A empresa precisa garantir que apenas os atribuídos certos tenham acesso a funções privilegiadas. Os auditores do sistema também devem auditar o histórico de revisão de acesso para relatar a eficácia dos controles internos da Contoso.

Neste tutorial, você usará a API de críticas de acesso para revisar periodicamente usuários e grupos com acesso a funções privilegiadas na Contoso. Esse acesso inclui funções ativas e qualificadas.

## <a name="prerequisites"></a>Pré-requisitos

Para concluir este tutorial, você precisa dos seguintes recursos e privilégios:

+ Um locatário do Azure AD funcionando com uma licença Azure AD Premium P2 ou EMS E5 habilitada.
+ Entre no Graph [Explorer](https://developer.microsoft.com/graph/graph-explorer) como usuário em uma função de Administrador de Função Privilegiada.
+ Entidades com atribuições ativas ou qualificadas para uma função privilegiada. Essas atribuições serão o escopo da revisão de acesso. Para atribuir funções privilegiadas, consulte [Tutorial: Use a API Privileged Identity Management (PIM) para atribuir funções do Azure AD](/graph/tutorial-assign-azureadroles).
    + Neste tutorial, a função Administrador do Usuário é o recurso em revisão. Um grupo de segurança e um usuário individual foram atribuídos à função.
+ As seguintes permissões delegadas: `AccessReview.ReadWrite.All`.

Para consentir com as permissões necessárias no Graph Explorer:
1. Selecione o ícone de releições horizontais à direita dos detalhes da conta do usuário e escolha **Selecionar permissões**.

      :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Selecione Permissões Graph Microsoft." border="true":::

2. Role a lista de permissões para **AccessReview (3)**, expanda e selecione `AccessReview.ReadWrite.All`. Selecione **Consentimento** e, em seguida, selecione **Aceitar** para aceitar o consentimento das permissões.

      :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="Consentimento para permissões Graph Microsoft." border="true":::

>[!NOTE]
>Os objetos de resposta mostrados neste tutorial podem ser reduzidos para a capacidade de leitura.

## <a name="step-1-create-an-access-review-of-privileged-role-assignments"></a>Etapa 1: Criar uma revisão de acesso de atribuições de função privilegiadas

Neste tutorial, criamos uma revisão de acesso recorrente de atribuições  ativas  e qualificadas para a função administrador do usuário. Um **accessReviewScheduleDefinition** pode ser usado para definir a revisão de acesso de vários tipos principais (usuários e grupos ou entidades de serviço) para apenas uma função privilegiada. Para revisar o acesso a várias funções privilegiadas, crie objetos **accessReviewScheduleDefinition** separados.

A definição de agenda de revisão de acesso a seguir tem as seguintes configurações:

+ O escopo da revisão é principal (**propriedade principalScopes** ) com acesso ao recurso especificado na **propriedade resourceScopes** . Nesse caso, as entidades principais são grupos e usuários, enquanto o recurso é a função Administrador do Usuário.
+ As atribuições ativas e qualificadas para o recurso de função administrador do usuário estão em revisão.
+ Um usuário individual é selecionado como revistor. Neste exemplo, você será o revistor.
+ O aprovador deve fornecer justificativa antes de aprovar o acesso à função privilegiada.
+ A decisão padrão é `None` quando os revisadores não respondem à solicitação de revisão de acesso antes que a instância expire.
+ **autoApplyDecisionsEnabled** não está definido e o padrão é `false`. Nesse caso, após a conclusão da revisão, as decisões não são aplicadas automaticamente, portanto, você deve aplicá-las manualmente.
+ A revisão é recorrência a cada três meses em um período de três dias e não termina.

### <a name="request"></a>Solicitação

Na solicitação a seguir, substitua o `f674a1c9-4a40-439c-bfa3-4b61a9f29d85` pelo valor da ID do usuário. A funçãoDefinitionId `fe930be7-5e62-47db-91af-98c3a49a38b1` é o identificador de modelo global para a função administrador do usuário no Azure AD.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviledroles-create"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "Review access of users and groups to privileged roles",
    "descriptionForAdmins": "Review access of users and groups to privileged roles",
    "scope": {
        "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
        "principalScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/users",
                "queryType": "MicrosoftGraph"
            },
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups",
                "queryType": "MicrosoftGraph"
            }
        ],
        "resourceScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/roleManagement/directory/roleDefinitions/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
                "queryType": "MicrosoftGraph"
            }
        ]
    },
    "reviewers": [
        {
            "query": "/users/f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
            "queryType": "MicrosoftGraph"
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 3,
        "recommendationsEnabled": false,
        "recurrence": {
            "pattern": {
                "type": "absoluteMonthly",
                "interval": 3
            },
            "range": {
                "type": "noEnd",
                "startDate": "2022-03-02"
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
    "id": "57457d7c-af59-470c-ae71-aa72c657fe0f",
    "displayName": "Review access of users and groups to privileged roles",
    "createdDateTime": null,
    "lastModifiedDateTime": null,
    "status": "NotStarted",
    "descriptionForAdmins": "Review access of users and groups to privileged roles",
    "descriptionForReviewers": null,
    "instanceEnumerationScope": null,
    "createdBy": {
        "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
        "displayName": "Alex Wilber",
        "type": null,
        "userPrincipalName": "AlexW@Contoso.com"
    },
    "scope": {
        "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
        "principalScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/users",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        ],
        "resourceScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/roleManagement/directory/roleDefinitions/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        ]
    },
    "reviewers": [
        {
            "query": "/users/f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 3,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": false,
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
                "type": "noEnd",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2022-03-02",
                "endDate": null
            }
        },
        "applyActions": []
    },
    "additionalNotificationRecipients": []
}
```

## <a name="step-2-retrieve-instances-of-the-access-review"></a>Etapa 2: Recuperar instâncias da revisão de acesso

Cada instância de revisão de acesso *representa cada recorrência com cada recurso exclusivo* que está sob revisão. Na Etapa 1, apenas o recurso de função administrador do usuário foi definido no escopo. Como você definiu uma revisão de acesso recorrente, a ID da instância é diferente da ID da definição de agendamento na Etapa 1.

### <a name="request"></a>Solicitação

Na solicitação a seguir, substitua `57457d7c-af59-470c-ae71-aa72c657fe0f` pelo valor da revisão de acesso que você criou na Etapa 1.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-getinstances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances
```

### <a name="response"></a>Resposta

Nesta resposta, o objeto instance mostra a data de término como três dias após a data de início; esse período foi definido na Etapa 1 na **propriedade instanceDurationInDays** do **objeto accessReviewScheduleDefinition** . *Somente uma instância é retornada representando a primeira recorrência de apenas um recurso sob revisão.*

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('57457d7c-af59-470c-ae71-aa72c657fe0f')/instances",
    "@odata.count": 1,
    "value": [
        {
            "id": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "startDateTime": "2022-03-02T15:31:14.607Z",
            "endDateTime": "2022-03-05T15:31:14.607Z",
            "status": "InProgress",
            "scope": {
                "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
                "principalScopes": [
                    {
                        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                        "query": "/v1.0/users",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
                    },
                    {
                        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                        "query": "/v1.0/groups",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
                    }
                ],
                "resourceScopes": [
                    {
                        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                        "query": "/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
                    }
                ]
            },
            "reviewers": [
                {
                    "query": "/v1.0/users/f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": null
                }
            ],
            "fallbackReviewers": []
        }
    ]
}
```

O status dessa instância de revisão de acesso é `InProgress`. Um `InProgress` status significa que a instância de revisão está aberta para os revisadores enviarem decisões, e o período para essa instância de revisão de acesso não expirou. Você também recebeu uma notificação de email Microsoft Azure solicitando que você execute a revisão de acesso.

## <a name="step-3-retrieve-access-review-decisions-before-recording-any-decisions"></a>Etapa 3: recuperar decisões de revisão de acesso antes de registrar qualquer decisão

Antes de poder postar decisões, vamos primeiro inspecionar os itens aguardando sua decisão.

### <a name="request"></a>Solicitação

Na solicitação a seguir, substitua os seguintes valores:

+ `57457d7c-af59-470c-ae71-aa72c657fe0f` com o valor da revisão de acesso que você criou na Etapa 1.
+ `ad0dd148-5d16-4cfd-86e9-ab502f819aaf` com o valor da instância de revisão de acesso para a que você gostaria de recuperar decisões.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-getnodecisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions
```

### <a name="response"></a>Resposta

A resposta a seguir mostra dois itens de decisão cada correspondentes a uma decisão por acesso de uma entidade ao recurso.

+ A propriedade principal mostra que duas entidades têm acesso à função administrador do usuário, um grupo chamado Ajuda **de IT (Usuário)** e um usuário chamado **Aline Dupuy**.
+ O `NotReviewed` valor da **propriedade decision** indica que os revisadores não revisaram e postaram suas decisões.
+ Nenhuma recomendação está disponível porque as recomendações não foram habilitadas no **accessReviewScheduleDefinition** na Etapa 1.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accessReviewInstanceDecisionItem)"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('57457d7c-af59-470c-ae71-aa72c657fe0f')/instances('ad0dd148-5d16-4cfd-86e9-ab502f819aaf')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "4d79fbf6-36e6-430b-ba0a-2a727a480303",
            "accessReviewId": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "NoInfoAvailable",
            "principalLink": "https://graph.microsoft.com/v1.0/users/339143ab-541e-484f-b017-e1707e962d34",
            "resourceLink": "https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
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
                "id": "fe930be7-5e62-47db-91af-98c3a49a38b1",
                "displayName": "User Administrator",
                "type": "directoryRole"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "339143ab-541e-484f-b017-e1707e962d34",
                "displayName": "Aline Dupuy",
                "type": "user",
                "userPrincipalName": "AlineD@Contoso.com",
                "lastUserSignInDateTime": ""
            }
        },
        {
            "id": "62fd1c5b-04b8-4703-9fd7-dce6232c3775",
            "accessReviewId": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "NoInfoAvailable",
            "principalLink": "https://graph.microsoft.com/v1.0/groups/b5260fca-6d64-4d5a-92df-0c482d40bc4d",
            "resourceLink": "https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
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
                "id": "fe930be7-5e62-47db-91af-98c3a49a38b1",
                "displayName": "User Administrator",
                "type": "directoryRole"
            },
            "principal": {
                "id": "b5260fca-6d64-4d5a-92df-0c482d40bc4d",
                "displayName": "IT Helpdesk (User)",
                "type": "group"
            }
        }
    ]
}
```

Como revistor, agora você pode enviar suas decisões para a instância de revisão de acesso.

## <a name="step-4-record-decisions"></a>Etapa 4: Decisões de registro

Agora você registrará decisões para a revisão de acesso.

A política da empresa exige que o acesso a funções privilegiadas seja concedido apenas a grupos e não a usuários individuais. Em conformidade com a política da empresa, você negará o acesso de Aline Dupuy ao aprovar o acesso ao grupo.

Nas solicitações a seguir, substitua os seguintes valores:

+ `57457d7c-af59-470c-ae71-aa72c657fe0f` com o valor da revisão de acesso que você criou na Etapa 1
+ `ad0dd148-5d16-4cfd-86e9-ab502f819aaf` com o valor da instância de revisão de acesso que você gostaria de recuperar decisões para
+ `4d79fbf6-36e6-430b-ba0a-2a727a480303` com o valor da instância de revisão de acesso com escopo para o acesso de Aline
+ `62fd1c5b-04b8-4703-9fd7-dce6232c3775` com o valor da instância de revisão de acesso com escopo para o acesso do grupo do Helpdesk de IT

### <a name="approve-the-security-groups-role-assignment"></a>Aprovar a atribuição de função do grupo de segurança

#### <a name="request"></a>Solicitação

Na solicitação a seguir, você aprova o acesso para o grupo de Ajuda de TI.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-decisionsforgroup"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions/62fd1c5b-04b8-4703-9fd7-dce6232c3775
Content-type: application/json

{
    "decision": "Approve",
    "justification": "The IT Helpdesk requires continued access to the User Administrator role to manage user account support requests, lifecycle, and access to resources"
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```
HTTP/1.1 204 No Content
```

### <a name="deny-the-individual-user-their-role-assignment"></a>Negar ao usuário individual sua atribuição de função

#### <a name="request"></a>Solicitação

Na solicitação a seguir, você nega acesso a Aline Dupuy.

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-decisionsforuser"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions/4d79fbf6-36e6-430b-ba0a-2a727a480303
Content-type: application/json

{
    "decision": "Deny",
    "justification": "Aline Dupuy should join an allowed group to maintain access to the User Administrator role. For more details, refer to the company policy '#132487: Privileged roles'"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```
HTTP/1.1 204 No Content
```

Quando você recupera as decisões de revisão de acesso (repita a Etapa 3), elas têm as seguintes configurações:
+ A decisão de revisão de acesso para o grupo do Helpdesk de IT é `Approve` enquanto para Aline é `Deny`.
+ O objeto reviewedBy contém seus detalhes como revisores.
+ ApplyResult significa `New` que as decisões não foram aplicadas.

Embora você tenha gravado todas as decisões pendentes para esta instância, as decisões não foram aplicadas aos objetos de recurso e principais. Por exemplo, Aline ainda tem acesso à função privilegiada. Você pode verificar essa atribuição executando a seguinte consulta `https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'`. Esse comportamento é porque **o autoApplyDecisionsEnabled** `false`foi definido como , você não interrompeu a revisão e o período de instância não terminou.

Neste tutorial, você não interromperá a instância manualmente, mas a deixará terminar automaticamente e aplicará as decisões.

> [!TIP]
>
> 1. Até que **o status** da instância de revisão de acesso seja marcado como `Completed`, você ainda pode alterar as decisões. Reprise a etapa 4 para aplicar decisões diferentes para as entidades de entidades.
> 2. Você também pode interromper manualmente a instância de revisão de acesso para que possa acelerar seu progresso para a Etapa 5.

## <a name="step-5-apply-access-review-decisions"></a>Etapa 5: aplicar decisões de revisão de acesso

Como administrador, depois **que o status** da instância de revisão de acesso for definido como `Completed`, você pode aplicar as decisões.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-applydecisions"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/applyDecisions
```

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```
HTTP/1.1 204 No Content
```

Aline agora perdeu o acesso à função de Administrador do Usuário enquanto o grupo de Ajuda de IT mantém seu acesso. Você pode verificar esse estado de atribuição de função executando a seguinte consulta `https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'`.

Depois que as decisões foram aplicadas, **o status** da instância de revisão de acesso será `Applied`. Além disso, como criamos uma revisão de acesso recorrente na Etapa 1, uma nova instância será iniciada. Sua data de início será de três meses a partir do momento em que o período de revisão atual for marcado como tendo terminado.

## <a name="step-6-retrieve-access-review-decisions"></a>Etapa 6: Recuperar decisões de revisão de acesso

Os auditores da Contoso estão revendo todas as decisões para conceder ou negar acesso a funções privilegiadas na organização. Você recuperará logs de decisão de revisão de acesso para todas as avaliações de acesso com escopo para funções privilegiadas. Neste exemplo, você recuperará logs de decisão para **o accessReviewScheduleDefinition** criado na Etapa 1.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-getdecisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions
```

### <a name="response"></a>Resposta

O seguinte objeto de resposta é diferente do objeto de resposta recebido na Etapa 3 com as seguintes configurações:
+ A decisão de revisão **de** acesso para o Helpdesk de IT é `Approve` enquanto para Aline é `Deny`.
+ O **objeto reviewedBy** contém seus detalhes básicos como revisores.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accessReviewInstanceDecisionItem)"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('57457d7c-af59-470c-ae71-aa72c657fe0f')/instances('ad0dd148-5d16-4cfd-86e9-ab502f819aaf')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "4d79fbf6-36e6-430b-ba0a-2a727a480303",
            "accessReviewId": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "reviewedDateTime": "2022-03-02T16:50:21.227Z",
            "decision": "Deny",
            "justification": "Aline Dupuy should join an allowed group to maintain access to the User Administrator role. For more details, refer to the company policy '#132487: Privileged roles'",
            "appliedDateTime": "2022-03-02T17:21:05.363Z",
            "applyResult": "AppliedSuccessfully",
            "recommendation": "NoInfoAvailable",
            "principalLink": "https://graph.microsoft.com/v1.0/users/339143ab-541e-484f-b017-e1707e962d34",
            "resourceLink": "https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
            "reviewedBy": {
                "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
                "displayName": "Alex Wilber",
                "type": null,
                "userPrincipalName": "AlexW@Contoso.com"
            },
            "appliedBy": {
                "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
                "displayName": "Alex Wilber",
                "type": null,
                "userPrincipalName": "AlexW@Contoso.com"
            },
            "resource": {
                "id": "fe930be7-5e62-47db-91af-98c3a49a38b1",
                "displayName": "User Administrator",
                "type": "directoryRole"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "339143ab-541e-484f-b017-e1707e962d34",
                "displayName": "Aline Dupuy",
                "type": "user",
                "userPrincipalName": "AlineD@Contoso.com",
                "lastUserSignInDateTime": ""
            }
        },
        {
            "id": "62fd1c5b-04b8-4703-9fd7-dce6232c3775",
            "accessReviewId": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "reviewedDateTime": "2022-03-02T16:31:04.357Z",
            "decision": "Approve",
            "justification": "The IT Helpdesk requires continued access to the User Administrator role to manage user account support requests, lifecycle, and access to resources.",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "NoInfoAvailable",
            "principalLink": "https://graph.microsoft.com/v1.0/groups/b5260fca-6d64-4d5a-92df-0c482d40bc4d",
            "resourceLink": "https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
            "reviewedBy": {
                "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
                "displayName": "Alex Wilber",
                "type": null,
                "userPrincipalName": "AlexW@Contoso.com"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "resource": {
                "id": "fe930be7-5e62-47db-91af-98c3a49a38b1",
                "displayName": "User Administrator",
                "type": "directoryRole"
            },
            "principal": {
                "id": "b5260fca-6d64-4d5a-92df-0c482d40bc4d",
                "displayName": "IT Helpdesk (User)",
                "type": "group"
            }
        }
    ]
}
```

<!-- comment this out until a bug is fixed

## Step 7: Retrieve access review history definitions

Contoso's auditors also want to review the access review history for the last quarter. In this example, you'll generate an access review history report for all **accessReviewScheduleDefinition** objects scoped to directory role assignments (roleAssignmentScheduleInstances). In this query, the **decisions** property is empty and therefore defaults to include all decisions in the history report.

First, you'll define the scope of the history report. Then, you generate a download URI that the auditors will use to download the report. The download URI is active for only 24 hours. So, after expiry, you can regenerate another download URI from the previously defined history report.

### Define the scope of the access review history data

In the following request, an empty **decisions** object means all decisions related to the scope of the access review will be included in the history report.

#### Request

```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions

{
    "displayName": "Last quarter's access reviews for privileged roles - User Administrator",
    "decisions": [],
    "reviewHistoryPeriodStartDateTime": "2022-03-01T00:00:00Z",
    "reviewHistoryPeriodEndDateTime": "9999-12-31T00:00:00Z",
    "scopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "queryType": "MicrosoftGraph",
            "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')"
        }
    ]
}
```

#### Response

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/historyDefinitions/$entity",
    "id": "983db508-b77b-427d-ab90-a4041efa658d",
    "displayName": "Last quarter's access reviews for privileged roles - User Administrator",
    "reviewHistoryPeriodStartDateTime": "2022-03-01T00:00:00Z",
    "reviewHistoryPeriodEndDateTime": "9999-12-31T00:00:00Z",
    "decisions": [
        "approve",
        "deny",
        "dontKnow",
        "notReviewed",
        "notNotified"
    ],
    "status": "requested",
    "createdDateTime": "2022-03-02T18:08:51.9032457Z",
    "fulfilledDateTime": null,
    "downloadUri": null,
    "createdBy": {
        "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
        "displayName": "Alex Wilber",
        "type": null,
        "userPrincipalName": "AlexW@Contoso.com"
    },
    "scopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ]
}
```

### Retrieve the instances of the access review history

#### Request

```msgraph-interactive
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/983db508-b77b-427d-ab90-a4041efa658d/instances
```

#### Response

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/historyDefinitions('983db508-b77b-427d-ab90-a4041efa658d')/instances",
    "value": [
        {
            "id": "983db508-b77b-427d-ab90-a4041efa658d",
            "reviewHistoryPeriodStartDateTime": "2022-03-01T00:00:00Z",
            "reviewHistoryPeriodEndDateTime": "9999-12-31T00:00:00Z",
            "status": "done",
            "runDateTime": "2022-03-02T18:08:51.9032457Z",
            "fulfilledDateTime": "2022-03-02T18:08:55.8336038Z",
            "downloadUri": null
        }
    ]
}
```

### Generate a link to download the history report from the instance of the access review history

#### Request

```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/983db508-b77b-427d-ab90-a4041efa658d/instances/983db508-b77b-427d-ab90-a4041efa658d/generateDownloadUri()
```

#### Response

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessReviewHistoryInstance",
    "@odata.type": "#microsoft.graph.accessReviewHistoryInstance",
    "id": "a222f18d-5cf5-4210-874c-14d0a7d930b3",
    "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
    "reviewHistoryPeriodEndDateTime": "9999-12-31T00:00:00Z",
    "status": "done",
    "runDateTime": "2022-02-22T10:08:08.2057428Z",
    "fulfilledDateTime": "2022-02-22T10:09:28.5862766Z",
    "downloadUri": "https://ermconsolreportweu.blob.core.windows.net/erm-reports/Last quarter's group reviews April 2021-a222f18d-5cf5-4210-874c-14d0a7d930b3.csv?skoid=4ad0868b-7b78-4869-abb7-8f29151d8428&sktid=33e01921-4d64-4f8c-a055-5bdaffd5e33d&skt=2022-02-22T10:11:22Z&ske=2022-02-22T10:13:22Z&sks=b&skv=2020-04-08&sv=2020-04-08&st=2022-02-22T10:11:22Z&se=2022-02-23T10:11:22Z&sr=b&sp=r&sig=5eX5BfVLS58QqF7oguRH8TeSQdXDHZlapY3y1U%2FGz%2BM%3D"
}
```

The downloadUri property contains a link to download the history report in an Excel file format. This link is active for only 24 hours.

-->
## <a name="step-7-clean-up-resources"></a>Etapa 7: Limpar recursos

**Exclua o objeto accessReviewScheduleDefinition** criado para este tutorial. Como a definição de agenda de revisão de acesso é o plano para a revisão de acesso, excluir a definição removerá as configurações, instâncias, decisões.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-deleteaccessreview"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea
```

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="conclusion"></a>Conclusão

Você aprendeu a revisar o acesso a funções privilegiadas no Azure AD. Sua organização pode usar a API de críticas de acesso para reger continuamente o acesso privilegiado a seus recursos, incluindo funções do Azure AD e funções de recurso do Azure. Além de usuários e grupos, você também pode revisar o acesso de aplicativos e entidades de serviço a funções privilegiadas.

## <a name="see-also"></a>Confira também

+ [Referência da API de avaliações do Access](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)
+ [Configurar o escopo da definição de revisão de acesso usando a API do Microsoft Graph](/graph/accessreviews-scope-concept)
+ [Saiba mais sobre o gerenciamento de acesso privilegiado](/microsoft-365/compliance/privileged-access-management-overviewe)