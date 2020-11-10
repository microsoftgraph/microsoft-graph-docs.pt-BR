---
title: Obter identityProvider
description: Recupere as propriedades e os relacionamentos de um objeto identityprovider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 69615bbe83d3d93f09120a39277f8c18415ca745
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953429"
---
# <a name="get-identityprovider"></a>Obter identityProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e os relacionamentos de um [identityprovider](../resources/identityprovider.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)|IdentityProvider.Read.All, IdentityProvider.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|IdentityProvider.Read.All, IdentityProvider.ReadWrite.All|

A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:
* Administrador global
* Administrador do provedor de identidade externa

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---------------|:----------|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma representação JSON do [identityprovider](../resources/identityprovider.md) ou [openIdConnectProvider](../resources/openidconnectprovider.md) (somente para o Azure ad B2C) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-retrieve-a-specific-identityprovider"></a>Exemplo 1: recuperar um identityprovider específico

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
### <a name="example-2-retrieve-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a>Exemplo 2: recuperar um determinado openIDConnectProvider (somente para o Azure AD B2C)

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "name": "Login with the Contoso identity provider",
  "type": "OpenIDConnect",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "12345",
  "claimsMapping": {
      "userId": "myUserId",
      "givenName": "myGivenName",
      "surname": "mySurname",
      "email": "myEmail",
      "displayName": "myDisplayName"
  },
  "domainHint": "mycustomoidc",
  "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
  "responseMode": "form_post",
  "responseType": "code",
  "scope": "openid"
}
```


