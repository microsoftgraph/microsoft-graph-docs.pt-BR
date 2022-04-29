---
title: Criar unifiedRoleAssignmentScheduleRequest
description: No PIM, solicite uma atribuição de função ativa e persistente por meio do objeto unifiedRoleAssignmentScheduleRequest. Use essa API para ativar funções qualificadas.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e8295babb10821b9949231bb27ebb20b8570662d
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133854"
---
# <a name="create-unifiedroleassignmentschedulerequest"></a>Criar unifiedRoleAssignmentScheduleRequest
Namespace: microsoft.graph

No PIM, execute as seguintes operações por meio do [objeto unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) :
+ Solicite atribuições de função ativas e persistentes para uma entidade de segurança, com ou sem datas de expiração.
+ Ativar, desativar, estender ou renovar uma atribuição de função qualificada para uma entidade de segurança.

Para chamar essa API para atualizar, renovar e estender as atribuições por conta própria, você deve ter a MFA (autenticação multifator) imposta e executar a consulta em uma sessão na qual elas foram desafiadas para MFA. Consulte [Habilitar a autenticação Azure AD multifator para proteger eventos de entrada](/azure/active-directory/authentication/howto-mfa-userstates).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|RoleAssignmentSchedule.ReadWrite.Directory|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|RoleAssignmentSchedule.ReadWrite.Directory|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleAssignmentScheduleRequests
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) .

Você pode especificar as propriedades a seguir ao criar **um unifiedRoleAssignmentScheduleRequest**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|unifiedRoleScheduleRequestActions|Representa o tipo da operação na solicitação de atribuição de função. Os valores possíveis são `adminAssign`, `adminUpdate`, `adminRemove`, `selfActivate`, `selfDeactivate`, `adminExtend`, `adminRenew`, `selfExtend`, `selfRenew`, `unknownFutureValue`. <br/><ul><li>`adminAssign`: para administradores atribuirem funções a usuários ou grupos.</li><li>`adminRemove`: para administradores removerem usuários ou grupos de funções.</li><li> `adminUpdate`: para que os administradores alterem as atribuições de função existentes.</li><li>`adminExtend`: para que os administradores estendam as atribuições de expiração.</li><li>`adminRenew`: para que os administradores renovem atribuições expiradas.</li><li>`selfActivate`: para que os usuários ativem suas atribuições.</li><li>`selfDeactivate`: para que os usuários desativem suas atribuições ativas.</li><li>`selfExtend`: para que os usuários solicitem a extensão de suas atribuições de expiração.</li><li>`selfRenew`: para que os usuários solicitem a renovação de suas atribuições expiradas.</li></ul>|
|Customdata|Cadeia de caracteres|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Opcional.|
|principalId|Cadeia de caracteres|Identificador da entidade de segurança que recebeu a atribuição. Obrigatório.|
|roleDefinitionId|Cadeia de caracteres|Identificador do [objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) que está sendo atribuído. Obrigatório.|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. **DirectoryScopeId ou** **appScopeId** é necessário.|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando a atribuição está no escopo de um aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. **DirectoryScopeId ou** **appScopeId** é necessário.|
|Justificação|Cadeia de caracteres|Uma mensagem fornecida por usuários e administradores ao criar eles criam o objeto **unifiedRoleAssignmentScheduleRequest** . Opcional.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O período da solicitação de atribuição de função. No momento, não há suporte para agendamentos recorrentes. Obrigatório.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Detalhes do tíquete vinculados à solicitação de atribuição de função, incluindo detalhes do número do tíquete e do sistema de tíquetes. Opcional.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-admin-assigning-a-directory-role-to-a-principal"></a>Exemplo 1: Administrador atribuindo uma função de diretório a uma entidade de segurança

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentschedulerequest_from_"
}
-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests
Content-Type: application/json

{
    "action": "adminAssign",
    "justification": "Assign Groups Admin to IT Helpdesk group",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "scheduleInfo": {
        "startDateTime": "2022-04-10T00:00:00Z",
        "expiration": {
            "type": "NoExpiration"
        }
    }
}
```


#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
    "id": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
    "status": "Provisioned",
    "createdDateTime": "2022-04-11T11:50:03.9014347Z",
    "completedDateTime": "2022-04-11T11:50:05.9999343Z",
    "approvalId": null,
    "customData": null,
    "action": "adminAssign",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
    "justification": "Assign Groups Admin to IT Helpdesk group",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "3fbd929d-8c56-4462-851e-0eb9a7b3a2a5"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2022-04-11T11:50:05.9999343Z",
        "recurrence": null,
        "expiration": {
            "type": "noExpiration",
            "endDateTime": null,
            "duration": null
        }
    },
    "ticketInfo": {
        "ticketNumber": null,
        "ticketSystem": null
    }
}
```

### <a name="example-2-user-activating-their-eligible-role"></a>Exemplo 2: Usuário ativando sua função qualificada

#### <a name="request"></a>Solicitação

Na solicitação a seguir, um usuário identificado por **principalId** `071cc716-8147-4397-a5ba-b2105951cc0b` ativa sua própria  função qualificada para uma Azure AD função identificada pela ID`8424c6f0-a189-499e-bbd0-26c1753c96d4`. O escopo de sua função é todos os objetos de diretório no locatário e a atribuição é de cinco horas. Para executar essa solicitação, o usuário de chamada deve ter a MFA (autenticação multifator) imposta e executar a consulta em uma sessão na qual foi desafiado para MFA.

Para recuperar os detalhes de suas solicitações de qualificação e identificar a qualificação a ser ativada, o usuário chamará [a API unifiedRoleEligibilitySchedule: filterByCurrentUser](unifiedroleeligibilityschedule-filterbycurrentuser.md) .

<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentschedulerequest_from_unifiedroleassignmentschedulerequests_selfActivate"
}
-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests/
Content-Type: application/json

{
    "action": "selfActivate",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "justification": "I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs",
    "scheduleInfo": {
        "startDateTime": "2022-04-14T00:00:00.000Z",
        "expiration": {
            "type": "AfterDuration",
            "duration": "PT5H"
        }
    },
    "ticketInfo": {
        "ticketNumber": "CONTOSO:Normal-67890",
        "ticketSystem": "MS Project"
    }
}
```



#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
    "id": "911bab8a-6912-4de2-9dc0-2648ede7dd6d",
    "status": "Granted",
    "createdDateTime": "2022-04-13T08:52:32.6485851Z",
    "completedDateTime": "2022-04-14T00:00:00Z",
    "approvalId": null,
    "customData": null,
    "action": "selfActivate",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "911bab8a-6912-4de2-9dc0-2648ede7dd6d",
    "justification": "I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "071cc716-8147-4397-a5ba-b2105951cc0b"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2022-04-14T00:00:00Z",
        "recurrence": null,
        "expiration": {
            "type": "afterDuration",
            "endDateTime": null,
            "duration": "PT5H"
        }
    },
    "ticketInfo": {
        "ticketNumber": "CONTOSO:Normal-67890",
        "ticketSystem": "MS Project"
    }
}
```