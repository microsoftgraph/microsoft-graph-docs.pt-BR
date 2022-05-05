---
title: Listar roleAssignmentScheduleRequests
description: No PIM, recupere as solicitações de atribuições de função ativas para entidades de segurança feitas por meio do objeto unifiedRoleAssignmentScheduleRequest.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 167fa54bcca28c3d9b362e3a44b6834aecab864d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207228"
---
# <a name="list-roleassignmentschedulerequests"></a>Listar roleAssignmentScheduleRequests
Namespace: microsoft.graph

No PIM, recupere as solicitações de atribuições de função ativas para entidades de segurança. As atribuições ativas incluem aquelas feitas por meio de [atribuições e solicitações](rbacapplication-post-roleassignmentschedulerequests.md) de ativação e diretamente por meio da [API de atribuições de função](../resources/unifiedroleassignment.md). As atribuições de função podem ser permanentemente ativas com ou sem uma data de expiração ou temporariamente ativas após a ativação do usuário de atribuições qualificadas.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory |
| Delegado (conta pessoal da Microsoft) | Sem suporte                               |
| Aplicativo                            | RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory               |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleRequests
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte aos `$select`parâmetros de consulta , `$filter`e `$expand` OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método `200 OK` retorna um código de resposta e uma coleção de [objetos unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-retrieve-role-assignment-requests"></a>Exemplo 1: Recuperar solicitações de atribuição de função

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentschedulerequest"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleassignmentschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleassignmentschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleassignmentschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleassignmentschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedroleassignmentschedulerequest-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests",
    "value": [
        {
            "id": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
            "status": "Provisioned",
            "createdDateTime": "2022-04-11T11:50:05.95Z",
            "completedDateTime": "2022-04-11T11:50:06Z",
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
    ]
}
```


### <a name="example-2-retrieve-specified-properties-of-role-assignment-requests-and-expand-the-relationships"></a>Exemplo 2: recuperar propriedades especificadas de solicitações de atribuição de função e expandir as relações

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentschedulerequest_expand_relationships"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests?$select=principalId,action,roleDefinitionId&$expand=roleDefinition,activatedUsing,principal,targetSchedule
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleassignmentschedulerequest-expand-relationships-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleassignmentschedulerequest-expand-relationships-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleassignmentschedulerequest-expand-relationships-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleassignmentschedulerequest-expand-relationships-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedroleassignmentschedulerequest-expand-relationships-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests(principalId,action,roleDefinitionId,roleDefinition(),activatedUsing(),principal(),targetSchedule())",
    "value": [
        {
            "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
            "action": "adminAssign",
            "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
            "roleDefinition": {
                "id": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
                "description": "",
                "displayName": "Groups Administrator",
                "isBuiltIn": true,
                "isEnabled": true,
                "templateId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
                "version": null,
                "resourceScopes": [],
                "rolePermissions": []
            },
            "activatedUsing": null,
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "071cc716-8147-4397-a5ba-b2105951cc0b",
                "displayName": "Conf Room Adams",
                "userPrincipalName": "Adams@Contoso.com",
                "mail": "Adams@Contoso.com",
                "businessPhones": [],
                "givenName": null,
                "jobTitle": null,
                "mobilePhone": null,
                "officeLocation": null,
                "preferredLanguage": null,
                "surname": null
            },
            "targetSchedule": {
                "id": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
                "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
                "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
                "directoryScopeId": "/",
                "appScopeId": null,
                "createdUsing": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
                "createdDateTime": "2022-04-11T11:50:05.95Z",
                "modifiedDateTime": "2022-04-11T11:50:05.95Z",
                "status": "Provisioned",
                "assignmentType": "Assigned",
                "memberType": "Direct",
                "scheduleInfo": {
                    "startDateTime": "2022-04-11T11:50:05.9999343Z",
                    "recurrence": null,
                    "expiration": {
                        "type": "noExpiration",
                        "endDateTime": null,
                        "duration": null
                    }
                }
            }
        }
    ]
}
```
