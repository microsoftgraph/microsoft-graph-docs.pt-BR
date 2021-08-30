---
title: Conceder um appRoleAssignment a uma entidade de serviço
description: Conceder uma atribuição de função de aplicativo a uma entidade de serviço.
ms.localizationpriority: high
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 45031635f8483385ab9d844c34d9f12a7cfeebf3
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695312"
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
  "name": "serviceprincipal_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignments
Content-Type: application/json

{
  "principalId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "resourceId": "8fce32da-1246-437b-99cd-76d1d4677bd5",
  "appRoleId": "498476ce-e0fe-48b0-b801-37ba7e2685c6"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Neste exemplo, observe que o valor usado como a principal **id** do serviço no URL do solicitado (`9028d19c-26a9-4809-8e3f-20ff73e2d75e`) é o mesmo que a propriedade **principalId** no corpo. O valor **resourceId** é a **id** principal do serviço de recursos (a API)

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments/$entity",
  "id": "2jLOj0YSe0OZzXbR1Gd71fDqFUrPM1xIgUfvWBHJ9n0",
  "creationTimestamp": "2021-02-15T16:39:38.2975029Z",
  "appRoleId": "498476ce-e0fe-48b0-b801-37ba7e2685c6",
  "principalDisplayName": "Fabrikam App",
  "principalId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "principalType": "ServicePrincipal",
  "resourceDisplayName": "Microsoft Graph",
  "resourceId": "8fce32da-1246-437b-99cd-76d1d4677bd5"
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
