---
title: Criar identityProvider
description: Crie um novo objeto identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 5fe99410b965f6cabae171c713a7207fc2c7ea18
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508831"
---
# <a name="create-identityprovider-deprecated"></a>Criar identityProvider (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

Crie um novo [objeto identityProvider.](../resources/identityprovider.md)

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)|IdentityProvider.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|IdentityProvider.ReadWrite.All|

A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:
* Administrador Global
* Administrador do Provedor de Identidade Externa

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /identityProviders
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---------------|:----------|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do [objeto identityProvider](../resources/identityprovider.md) ou [openIdConnectProvider](../resources/openidconnectprovider.md) (somente para o Azure AD B2C). Todas as propriedades listadas na tabela a seguir são necessárias.

### <a name="identityprovider-object"></a>objeto identityProvider

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|O ID do cliente para o aplicativo. Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo. Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.|
|nome|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|
|tipo|Cadeia de caracteres|A identidade do provedor de identidade. <ul>Para o cenário B2B:<li/>Google<li/>Facebook</ul><ul>Para o cenário B2C:<li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook<li/>GitHub<li/>Twitter<li/>Weibo<li/>QQ<li/>WeChat<li/>OpenIDConnect</ul>|

### <a name="openidconnectprovider-object"></a>Objeto openIdConnectProvider

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|O ID do cliente para o aplicativo. Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo. Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.|
|nome|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|
|tipo|Cadeia de caracteres|A identidade do provedor de identidade. O valor deve ser `OpenIdConnect` .|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|As `userId` propriedades e são necessárias no objeto `displayname` claimsMapping.|
|metadataUrl|Cadeia de caracteres|A URL do documento de metadados do provedor de identidade do Open Id Connect.|
|responseMode|Cadeia de caracteres|Define o método que deve ser usado para enviar os dados de volta do provedor de identidade personalizado para o Azure AD B2C. Os seguintes modos de resposta podem ser usados: <ul><li/>`form_post` : Este modo de resposta é recomendado para melhor segurança. A resposta é transmitida por meio do método HTTP POST, com o código ou token sendo codificado no corpo usando o formato application/x-www-form-urlencoded.<li/>`query` : O código ou token é retornado como um parâmetro de consulta.</ul>|
|responseType|Cadeia de caracteres|Descreve que tipo de informação é enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizado. Os seguintes tipos de resposta podem ser usados:<ul><li/> `code` : De acordo com o fluxo de código de autorização, um código será retornado para o Azure AD B2C. O Azure AD B2C continua a chamar o token_endpoint para trocar o código pelo token.<li/> `id_token` : Um token de ID é retornado ao Azure AD B2C do provedor de identidade personalizado. <li/>`token` : Um token de acesso é retornado ao Azure AD B2C do provedor de identidade personalizado. (Esse valor não é suportado pelo Azure AD B2C no momento)</ul>|
|escopo|String|O escopo define as informações e permissões que você está procurando coletar do provedor de identidade personalizado.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e `201 Created` [um objeto identityProvider](../resources/identityprovider.md) ou [openIdConnectProvider](../resources/openidconnectprovider.md) (somente para o Azure AD B2C) no corpo da resposta. Caso não consiga, um `4xx` erro será retornado com detalhes específicos.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-a-specific-identityprovider"></a>Exemplo 1: Criar uma **identidade específicaProvider**

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.identityProvider",
  "name": "Login with Amazon",
  "type": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}
```

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "@odata.type": "microsoft.graph.identityProvider",
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

### <a name="example-2-create-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a>Exemplo 2: Criar um **openIDConnectProvider específico** (somente para o Azure AD B2C)

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "create_openidconnectprovider_from_identityproviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-openidconnectprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-openidconnectprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-openidconnectprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-openidconnectprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```http
HTTP/1.1 201 Created
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
