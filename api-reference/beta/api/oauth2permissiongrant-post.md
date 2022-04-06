---
title: Criar oAuth2PermissionGrant (uma concessão de permissão delegada)
description: Crie um objeto oAuth2PermissionGrant, representando uma concessão de permissão delegada.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 631bc0ce35a597c44af163cf82d12bc3eb029298
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63670835"
---
# <a name="create-oauth2permissiongrant-a-delegated-permission-grant"></a>Criar oAuth2PermissionGrant (uma concessão de permissão delegada)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie uma concessão de permissão delegada, representada por um [objeto oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .

Uma concessão de permissão delegada autoriza uma entidade de serviço de cliente (representando um aplicativo cliente) a acessar uma entidade de serviço de recursos (representando uma API), em nome de um usuário assinado, para o nível de acesso limitado pelas permissões delegadas que foram concedidas.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /oauth2PermissionGrants
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição |
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de [um objeto oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [oauth2PermissionGrant](../resources/oauth2permissiongrant.md).

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| clientId | Cadeia de caracteres | A **id da** entidade de [](../resources/serviceprincipal.md) serviço do cliente para o aplicativo que está autorizado a agir em nome de um usuário interno ao acessar uma API. Obrigatório.  |
| consentType | String | Indica se a autorização é concedida para que o aplicativo cliente represente todos os usuários ou apenas um usuário específico. *AllPrincipals* indica autorização para representar todos os usuários. *A* entidade indica autorização para representar um usuário específico. O consentimento em nome de todos os usuários pode ser concedido por um administrador. Os usuários que não são administradores podem ser autorizados a consentir em nome de si mesmos em alguns casos, para algumas permissões delegadas. Obrigatório.  |
| principalId | String | A **id** do [usuário em](../resources/user.md) nome do qual o cliente está autorizado a acessar o recurso, quando **consentType** for *Principal*. Se **consentType** for *AllPrincipals* , esse valor será nulo. Obrigatório quando **consentType** for *Principal*. |
| resourceId | Cadeia de caracteres | A **id da** entidade de [serviço de recursos](../resources/serviceprincipal.md) à qual o acesso está autorizado. Isso identifica a API que o cliente está autorizado a tentar chamar em nome de um usuário in-locar. |
| escopo | String | Uma lista separada por espaço dos valores de declaração para permissões delegadas que devem ser incluídos em tokens de acesso para o aplicativo de recurso (a API). Por exemplo, `openid User.Read GroupMember.Read.All`. Cada valor de declaração deve corresponder  ao campo de valor de uma das permissões delegadas definidas pela API, listadas na propriedade **publishedPermissionScopes** da entidade de [serviço de recursos](../resources/serviceprincipal.md). |
| startTime | DateTimeOffset | Atualmente, o valor de hora de início é ignorado, mas um valor é necessário. Obrigatório. |
| expiryTime | DateTimeOffset | Atualmente, o valor de hora de término é ignorado, mas um valor é necessário. Obrigatório. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta de 200 séries e um novo [objeto oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_oAuth2PermissionGrant"
}-->

```http
POST https://graph.microsoft.com/beta/oauth2PermissionGrants
Content-Type: application/json

{
    "clientId": "ef969797-201d-4f6b-960c-e9ed5f31dab5",
    "consentType": "AllPrincipals",
    "resourceId": "943603e4-e787-4fe9-93d1-e30f749aae39",
    "scope": "DelegatedPermissionGrant.ReadWrite.All",
    "startTime": "2022-03-17T00:00:00Z",
    "expiryTime": "2023-03-17T00:00:00Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/post-oauth2permissiongrant-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/post-oauth2permissiongrant-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#oauth2PermissionGrants/$entity",
    "clientId": "ef969797-201d-4f6b-960c-e9ed5f31dab5",
    "consentType": "AllPrincipals",
    "expiryTime": "2023-03-17T00:00:00Z",
    "id": "l5eW7x0ga0-WDOntXzHateQDNpSH5-lPk9HjD3Sarjk",
    "principalId": null,
    "resourceId": "943603e4-e787-4fe9-93d1-e30f749aae39",
    "scope": "DelegatedPermissionGrant.ReadWrite.All",
    "startTime": "2022-03-17T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


