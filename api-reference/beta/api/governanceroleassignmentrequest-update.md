---
title: Atualizar governanceRoleAssignmentRequests
description: Permitem que administradores atualizar suas decisões (`AdminApproved` ou `AdminDenied`) em governanceRoleAssignmentRequests que estão no status de `PendingAdminDecision`.
localization_priority: Normal
ms.openlocfilehash: 3d68e06688922177e2a1a183a9fe4bfc6be6a91d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874932"
---
# <a name="update-governanceroleassignmentrequests"></a>Atualizar governanceRoleAssignmentRequests

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Permitem que administradores atualizar suas decisões (`AdminApproved` ou `AdminDenied`) em [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que estão no status de `PendingAdminDecision`.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Observação:** Essa API também requer que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) em relação ao qual pertence o [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) recurso. 

|Tipo de permissão      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureResources  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome           | Descrição|
|:---------------|:----------|
| Autorização  | Portador {código}|
| Content-type  | application/json|

## <a name="request-body"></a>Corpo da solicitação

|Parâmetros      |Tipo                   |Obrigatório |Descrição|
|:-------------|:----------------------|:--------|:----------|
|motivo        |Cadeia de caracteres                 |✓        |O motivo fornecido pelo administrador para a sua decisão.|
|decisão        |Cadeia de caracteres                 |✓        |A decisão de administrador da solicitação de atribuição de função. O valor deve ser atualizado como `AdminApproved` ou `AdminDenied`.|
|agenda      |[governanceSchedule](../resources/governanceschedule.md)|        | O agendamento da solicitação de atribuição de função. Status da `AdminApproved`, é necessário.|
|assignmentState      |Cadeia de caracteres|         | O estado da atribuição e os valores pode ser `Eligible` ou `Active`. Decisão de `AdminApproved`, é necessário. |
### <a name="response"></a>Resposta
Esse método só pode ser aplicado a solicitações que estejam no status de `PendingAdminDecision`.

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
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
<!-- {
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
