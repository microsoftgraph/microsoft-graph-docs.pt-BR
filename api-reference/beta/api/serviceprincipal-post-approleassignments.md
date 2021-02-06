---
title: Conceder um appRoleAssignment a uma entidade de serviço
description: Conceder uma atribuição de função de aplicativo a uma entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 56bf801b932f1458d871df8bbe51f40340302087
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134243"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a>Conceder um appRoleAssignment a uma entidade de serviço

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atribuir uma função de aplicativo a uma entidade de serviço do cliente.

As funções do aplicativo atribuídas às entidades de serviço também são conhecidas como [permissões de aplicativo](/azure/active-directory/develop/v2-permissions-and-consent#permission-types). As permissões de aplicativo podem ser concedidas diretamente com atribuições de função de aplicativo ou por meio de uma [experiência de consentimento](/azure/active-directory/develop/application-consent-experience).

Para conceder uma atribuição de função de aplicativo a uma entidade de serviço do cliente, você precisa de três identificadores:

- `principalId`: A `id` da entidade de serviço do cliente ao qual você está atribuindo a função de aplicativo.
- `resourceId`: A `id` do recurso `servicePrincipal` (a API) que definiu a função do aplicativo (a permissão do aplicativo).
- `appRoleId`: A `id` da `appRole` (definido na entidade de serviço do recurso) para atribuir à entidade de serviço do cliente.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | AppRoleAssignment. ReadWrite.All, Directory. ReadWrite.All, Directory. AccessAsUser.All    |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> Como prática recomendada, recomendamos que você crie atribuições de função de aplicativo por meio da [`appRoleAssignedTo`relação do _recurso_ da entidade de serviço](serviceprincipal-post-approleassignedto.md), em vez da `appRoleAssignments`relação do usuário, grupo ou entidade de serviço atribuída.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:----------|
| Autorização | {token} de portador. Obrigatório.  |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de um objeto [appRoleAssignment](../resources/approleassignment.md).

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Nesse exemplo, a `{id}` e o `{principalId-value}` seriam as `id` da entidade de serviço de cliente atribuída e o `{resourceId}` seria a `id` da entidade de serviço de recurso (a API).

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. 

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 253

{
  "id": "id-value",
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalType": "principalType-value",
  "principalId": "principalId-value",
  "principalDisplayName": "principalDisplayName-value",
  "resourceId": "resourceId-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

