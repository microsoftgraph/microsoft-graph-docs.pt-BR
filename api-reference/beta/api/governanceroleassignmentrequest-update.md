---
title: Atualizar governançaRoleAssignmentRequests
description: Permitir que os administradores atualizem suas decisões ( ou ) sobre `AdminApproved` `AdminDenied` governançaRoleAssignmentRequests que estão em status de `PendingAdminDecision` .
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 59080cf19cf96d82f029d3ba9513cd16a042157a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435851"
---
# <a name="update-governanceroleassignmentrequests"></a>Atualizar governançaRoleAssignmentRequests

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Permitir que os administradores atualizem suas decisões ( ou ) sobre `AdminApproved` `AdminDenied` [governançaRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que estão em status de `PendingAdminDecision` .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).

>**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função de administrador ( ou ) no recurso ao qual a `Active` `owner` `user access administrator` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pertence. 

### <a name="azure-resources"></a>Recursos do Azure

| Tipo de permissão | Permissões |
|:--------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureResources |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

### <a name="azure-ad"></a>Azure Active Directory

| Tipo de permissão | Permissões |
|:--------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureAD |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

### <a name="groups"></a>Grupos

|Tipo de permissão | Permissões |
|:-------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureADGroups |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome           | Descrição|
|:---------------|:----------|
| Authorization  | Portador {código}|
| Content-type  | application/json|

## <a name="request-body"></a>Corpo da solicitação

|Parâmetros      |Tipo                   |Obrigatório |Descrição|
|:-------------|:----------------------|:--------|:----------|
|motivo        |String                 |✓        |O motivo fornecido pelo administrador para sua decisão.|
|decision        |String                 |✓        |A decisão do administrador da solicitação de atribuição de função. O valor deve ser atualizado como `AdminApproved` ou `AdminDenied` .|
|Cronograma      |[governanceSchedule](../resources/governanceschedule.md)|        | O cronograma da solicitação de atribuição de função. Para o status `AdminApproved` de , é necessário.|
|assignmentState      |String|         | O estado da atribuição e os valores podem `Eligible` ser ou `Active` . Para a decisão `AdminApproved` de , é necessário. |
### <a name="response"></a>Resposta
Esse método só pode ser aplicado a solicitações que estão em status de `PendingAdminDecision` .

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updaterequest-governanceroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a>Corpo da solicitação
```json
{
  "reason":"approve the request to extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-02-20T07:31:13.451Z",
    "stopDateTime":"2018-05-21T07:31:13.451Z",
    },
  "decision":"AdminApproved",
  "assignmentState": "Eligible"
}
```

##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


