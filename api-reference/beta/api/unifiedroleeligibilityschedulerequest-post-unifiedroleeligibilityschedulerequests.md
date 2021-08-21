---
title: Criar unifiedRoleEligibilityScheduleRequest
description: Crie um novo objeto unifiedRoleEligibilityScheduleRequest.
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bf99b3df56889eb236a48f844134215e82084489
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453566"
---
# <a name="create-unifiedroleeligibilityschedulerequest"></a>Criar unifiedRoleEligibilityScheduleRequest
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md) Essa operação permite que administradores e usuários qualificados adicionem, revogam ou estendam atribuições qualificadas.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory |
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|Sem suporte|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleEligibilityScheduleRequests
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|Cadeia de caracteres|Representa o tipo da operação na atribuição de qualificação de função. Os valores possíveis são: <ul><li>`AdminAdd`: Para que os administradores atribuam qualificação de função a usuários ou grupos a funções.</li><li>`AdminExtend`: Para que os administradores estendam atribuições expiradas.</li><li>`AdminUpdate`: Para que os administradores alterem as atribuições de função existentes.</li><li>`AdminRenew`: Para que os administradores renovem atribuições expiradas.</li><li>`AdminRemove`: Para que os administradores removam usuários ou grupos de funções qualificadas.</li><li>`UserAdd`: Para que os usuários ativem suas atribuições qualificadas.</li><li>`UserExtend`: Para que os usuários solicitem estender suas atribuições qualificadas expiradas.</li><li>`UserRemove`: Para que os usuários desativem suas atribuições elegíveis ativas.</li><li>`UserRenew`: Para que os usuários solicitem a renovação de suas atribuições qualificadas expiradas.</li></ul>|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando o escopo de atribuição for específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Use `/` para escopos de aplicativos de todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas ou todos os usuários.|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo.|
|isValidationOnly|Booliano|Um booleano que determina se a chamada é uma validação ou uma chamada real. De definir essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação.|
|justification|Cadeia de caracteres|Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.|
|principalId|Cadeia de caracteres|Identificador da entidade à qual a atribuição está sendo concedida. Por exemplo, um usuário ou um grupo. Para grupos, eles devem ser atribuídos a funções, ou seja, **o isAssignableToRole** da propriedade group definida como `true` .|
|roleDefinitionId|Cadeia de caracteres|Identificador do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto schedule da solicitação de atribuição de função.|
|targetScheduleId|Cadeia de caracteres|O período de tempo para o qual a atribuição de qualificação é válida.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|O objeto ticketInfo anexado à solicitação de atribuição de função que inclui detalhes do número do tíquete e do sistema de tíquetes.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-admin-to-assign-a-role-eligibility-schedule-request"></a>Exemplo 1: Administrador para atribuir uma solicitação de agendamento de qualificação de função

Na solicitação a seguir, o administrador cria uma solicitação para atribuir a qualificação de uma função identificada por uma `fdd7a751-b60b-444a-984c-02652fe8fa1c` entidade identificada **por id** `07706ff1-46c7-4847-ae33-3003830675a1` . O escopo da qualificação é todos os objetos de diretório no locatário até 30 de junho de 2022 à meia-noite horário UTC.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_unifiedroleeligibilityschedulerequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json

{
  "action": "AdminAssign",
  "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
  "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
  "directoryScopeId": "/",
  "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
  "scheduleInfo": {
    "startDateTime": "2021-07-01T00:00:00Z",
    "expiration": {
      "endDateTime": "2022-06-30T00:00:00Z",
      "type": "AfterDateTime"
    }
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "672c03bf-226a-42ec-a8b7-3bfab96064a1",
    "status": "Provisioned",
    "createdDateTime": "2021-07-26T18:08:03.1299669Z",
    "completedDateTime": "2021-07-26T18:08:06.2081758Z",
    "approvalId": null,
    "customData": null,
    "action": "AdminAssign",
    "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "672c03bf-226a-42ec-a8b7-3bfab96064a1",
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-07-26T18:08:06.2081758Z",
        "recurrence": null,
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2022-06-30T00:00:00Z",
            "duration": null
        }
    },
    "ticketInfo": {
        "ticketNumber": null,
        "ticketSystem": null
    }
}
```

### <a name="example-2-admin-to-remove-an-existing-role-eligibility-schedule-request"></a>Exemplo 2: Administrador para remover uma solicitação de agendamento de qualificação de função existente

Na solicitação a seguir, o administrador cria uma solicitação para revogar a qualificação de uma função identificada por uma `fdd7a751-b60b-444a-984c-02652fe8fa1c` entidade identificada **por id** `07706ff1-46c7-4847-ae33-3003830675a1` .

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_unifiedroleeligibilityschedulerequests_AdminRemove"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json

{
    "action": "AdminRemove",
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
    "scheduleInfo": {
        "startDateTime": "2021-07-26T18:08:06.2081758Z",
        "expiration": {
            "endDateTime": "2022-06-30T00:00:00Z",
            "type": "AfterDateTime"
        }
    }
}
```



#### <a name="response"></a>Resposta

Este é um exemplo de resposta. A solicitação retorna um objeto de resposta que mostra o status das alterações de atribuição qualificadas anteriormente como `Revoked` . A entidade não verá mais sua função anteriormente qualificada.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "7f88a144-f9a9-4f8c-9623-39c321ae93c2",
    "status": "Revoked",
    "createdDateTime": "2021-08-06T17:59:12.4263499Z",
    "completedDateTime": null,
    "approvalId": null,
    "customData": null,
    "action": "AdminRemove",
    "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": null,
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-07-26T18:08:06.2081758Z",
        "recurrence": null,
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2022-06-30T00:00:00Z",
            "duration": null
        }
    },
    "ticketInfo": {
        "ticketNumber": null,
        "ticketSystem": null
    }
}
```