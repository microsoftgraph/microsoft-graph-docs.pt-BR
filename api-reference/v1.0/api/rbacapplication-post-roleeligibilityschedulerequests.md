---
title: Criar roleEligibilityScheduleRequest
description: No PIM, solicite uma qualificação de função para uma entidade de segurança por meio do objeto unifiedRoleEligibilityScheduleRequest.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 787bee8a5843f432d30c46828387983018d5b78a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439848"
---
# <a name="create-roleeligibilityschedulerequest"></a>Criar roleEligibilityScheduleRequest
Namespace: microsoft.graph

No PIM, solicite uma qualificação de função para uma entidade de segurança por meio do objeto [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) . Essa operação permite que administradores e usuários qualificados adicionem, revoguem ou estendam atribuições qualificadas.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|RoleEligibilitySchedule.ReadWrite.Directory|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|RoleAssignmentSchedule.ReadWrite.Directory|

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
No corpo da solicitação, forneça uma representação JSON do objeto [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) .

Você pode especificar as propriedades a seguir ao criar **um unifiedRoleEligibilityScheduleRequest**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|unifiedRoleScheduleRequestActions|Representa o tipo de operação na solicitação de qualificação de função. Os valores possíveis são: , , , , , `selfDeactivate`, `adminExtend`, `adminRenew`, `selfExtend`, , `selfRenew`, `unknownFutureValue`. `selfActivate``adminRemove``adminUpdate``adminAssign` <br/><ul><li>`adminAssign`: para que os administradores atribuam funções qualificadas às entidades de segurança.</li><li>`adminRemove`: para que os administradores removam funções qualificadas das entidades de segurança.</li><li> `adminUpdate`: para que os administradores alterem as eligibilidades de função existentes.</li><li>`adminExtend`: para que os administradores estendam as eligibilidades de função expiradas.</li><li>`adminRenew`: para que os administradores renovem as eligibilidades expiradas.</li><li>`selfActivate`: para que os usuários ativem suas atribuições.</li><li>`selfDeactivate`: para que os usuários desativem suas atribuições ativas.</li><li>`selfExtend`: para que os usuários solicitem a extensão de suas atribuições de expiração.</li><li>`SelfRenew`: para que os usuários solicitem a renovação de suas atribuições expiradas.</li></ul>|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando a elegibilidade de função está no escopo de um aplicativo. O escopo de uma elegibilidade de função determina o conjunto de recursos para os quais a entidade de segurança está qualificada para acessar. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. **DirectoryScopeId ou** **appScopeId** é necessário.|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da elegibilidade da função. O escopo de uma elegibilidade de função determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. **DirectoryScopeId ou** **appScopeId** é necessário.|
|isValidationOnly|Booliano|Determina se a chamada é uma validação ou uma chamada real. Defina essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação. Opcional.|
|Justificação|String|Uma mensagem fornecida por usuários e administradores ao criar eles criam o objeto **unifiedRoleEligibilityScheduleRequest** . Opcional quando **a ação** é `adminRemove`. Se essa propriedade é necessária ou opcional também depende das [configurações para a Azure AD função](../api/unifiedrolemanagementpolicy-list-rules.md).|
|principalId|Cadeia de caracteres|Identificador da entidade de segurança que recebeu a qualificação de função. Obrigatório.|
|roleDefinitionId|String|Identificador do [objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) que está sendo atribuído à entidade de segurança. Obrigatório.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O período de qualificação da função. Opcional quando **a ação** é `adminRemove`. O período de qualificação depende das [configurações da Azure AD função](../api/unifiedrolemanagementpolicy-list-rules.md).|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Detalhes do tíquete vinculados à solicitação de qualificação de função, incluindo detalhes do número do tíquete e do sistema de tíquetes. Opcional|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-admin-to-assign-a-role-eligibility-schedule-request"></a>Exemplo 1: Administração para atribuir uma solicitação de agendamento de qualificação de função

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json

{
    "action": "adminAssign",
    "justification": "Assign Attribute Assignment Admin eligibility to restricted user",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "scheduleInfo": {
        "startDateTime": "2022-04-10T00:00:00Z",
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2024-04-10T00:00:00Z"
        }
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleeligibilityschedulerequest-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleeligibilityschedulerequest-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleeligibilityschedulerequest-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleeligibilityschedulerequest-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleeligibilityschedulerequest-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroleeligibilityschedulerequest-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "50877283-9d40-433c-bab8-7986dc10458a",
    "status": "Provisioned",
    "createdDateTime": "2022-04-12T09:05:39.7594064Z",
    "completedDateTime": "2022-04-12T09:05:41.8532931Z",
    "approvalId": null,
    "customData": null,
    "action": "adminAssign",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "50877283-9d40-433c-bab8-7986dc10458a",
    "justification": "Assign Attribute Assignment Admin eligibility to restricted user",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "3fbd929d-8c56-4462-851e-0eb9a7b3a2a5"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2022-04-12T09:05:41.8532931Z",
        "recurrence": null,
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2024-04-10T00:00:00Z",
            "duration": null
        }
    },
    "ticketInfo": {
        "ticketNumber": null,
        "ticketSystem": null
    }
}
```

### <a name="example-2-admin-to-remove-an-existing-role-eligibility-schedule-request"></a>Exemplo 2: Administração para remover uma solicitação de agendamento de qualificação de função existente

Na solicitação a seguir, o administrador cria uma solicitação para revogar a qualificação de uma entidade de segurança com ID `071cc716-8147-4397-a5ba-b2105951cc0b` para uma função com ID `8424c6f0-a189-499e-bbd0-26c1753c96d4`.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_unifiedroleeligibilityschedulerequests_adminRemove"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json

{
    "action": "adminRemove",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

Este é um exemplo de resposta. O objeto de resposta mostra uma qualificação de função anterior para uma entidade de segurança é `Revoked`. A entidade de segurança não verá mais sua função qualificada anteriormente.

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "f341269e-c926-41fa-a905-cef3b01b2a67",
    "status": "Revoked",
    "createdDateTime": "2022-04-12T09:12:15.6859992Z",
    "completedDateTime": null,
    "approvalId": null,
    "customData": null,
    "action": "adminRemove",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": null,
    "justification": null,
    "scheduleInfo": null,
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "3fbd929d-8c56-4462-851e-0eb9a7b3a2a5"
        }
    },
    "ticketInfo": {
        "ticketNumber": null,
        "ticketSystem": null
    }
}
```
