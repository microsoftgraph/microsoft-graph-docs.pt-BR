---
title: Criar identityProvider
description: Crie um novo objeto identityProvider.
ms.localizationpriority: medium
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 8618c8777be997ac23b06c471d70f1f2f15c9aa3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015094"
---
# <a name="create-identityprovider"></a>Criar identityProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um recurso de provedor de identidade que seja do tipo especificado no corpo da solicitação.

Entre os tipos de provedores derivados de identityProviderBase, você pode criar atualmente um [recurso socialIdentityProvider](../resources/socialidentityprovider.md) no Azure AD. No Azure AD B2C, essa operação pode atualmente criar [um recurso socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md)ou um recurso [appleManagedIdentityProvider.](../resources/applemanagedidentityprovider.md)

## <a name="permissions"></a>Permissões

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
POST /identity/identityProviders
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---------------|:----------|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no Azure AD.

No Azure AD B2C, forneça uma representação JSON [de socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md)ou [um objeto appleManagedIdentityProvider.](../resources/applemanagedidentityprovider.md)

Todas as propriedades listadas nas tabelas a seguir são necessárias.

### <a name="socialidentityprovider-object"></a>Objeto socialIdentityProvider

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|O identificador do cliente para o aplicativo obtido ao registrar o aplicativo com o provedor de identidade.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido quando o aplicativo é registrado com o provedor de identidade. Isso é somente gravação. Uma operação de leitura retorna `****`.|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|
|identityProviderType|Cadeia de caracteres|Para um cenário B2B, valores possíveis: `Google`, `Facebook`. Para um cenário B2C, valores possíveis: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.|

### <a name="openidconnectidentityprovider-object"></a>Objeto openIdConnectIdentityProvider

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|A ID do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade. O clientSecret tem uma dependência de **responseType**. <ul><li>Quando **responseType** é `code` , um segredo é necessário para a troca de código de auth.</li><li>Quando **responseType** é o segredo não é necessário porque não há troca de código, o id_token é retornado `id_token` diretamente da resposta de autorização.</li></ul>|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|
|domainHint|String|A dica de domínio pode ser usada para pular diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa. Esse tipo complexo captura esse mapeamento.|
|metadataUrl|Cadeia de caracteres|A URL do documento de metadados do provedor de Conexão OpenID. Cada provedor Conexão de identidade OpenID descreve um documento de metadados que contém a maioria das informações necessárias para executar a login. Isso inclui informações como as URLs a ser usadas e o local das chaves de assinatura públicas do serviço. O documento Conexão de metadados do OpenID está sempre localizado em um ponto de extremidade que termina em `.well-known/openid-configuration` . Forneça a URL de metadados para o provedor Conexão de identidade openid que você adicionar.|
|responseMode|String|O modo de resposta define o método usado para enviar dados de volta do provedor de identidade personalizado para o Azure AD B2C. Valores possíveis: `form_post` , `query` .|
|responseType|Cadeia de caracteres|O tipo de resposta descreve o tipo de informação enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizado. Valores possíveis: `code` , `id_token` , `token` .|
|escopo|String|O escopo define as informações e permissões que você está procurando coletar do provedor de identidade personalizado.|

### <a name="appleidentityprovider-object"></a>Objeto appleIdentityProvider

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|
|developerId|Cadeia de caracteres|O Identificador de desenvolvedor da Apple.|
|serviceId|Cadeia de caracteres|O identificador de serviço da Apple.|
|keyId|Cadeia de caracteres|O identificador de chave da Apple.|
|certificateData|Cadeia de caracteres|Os dados do certificado, que são uma longa sequência de texto do certificado, podem ser nulos.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma representação JSON de um `201 Created` [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no corpo da resposta para um locatário do Azure AD.

Para um locatário do Azure AD B2C, este método retorna um código de resposta e uma representação JSON de `201 Created` [um objeto socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md)ou [um objeto appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) no corpo da resposta.

Caso não consiga, um `4xx` erro será retornado com detalhes específicos.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-a-specific-social-identity-provider-azure-ad-and-azure-ad-b2c"></a>Exemplo 1: Criar um provedor de **identidade social específico** (Azure AD e Azure AD B2C)

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_socialidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.socialIdentityProvider",
  "displayName": "Login with Amazon",
  "identityProviderType": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-socialidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-socialidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-socialidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-socialidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-socialidentityprovider-from-identityproviderbase-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.type": "microsoft.graph.socialIdentityProvider",
    "id": "Amazon-OAUTH",
    "displayName": "Login with Amazon",
    "identityProviderType": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

### <a name="example-2-create-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a>Exemplo 2: Criar um provedor de identidade **Conexão OpenID específico** (somente para o Azure AD B2C)

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_openidconnectidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
    "displayName": "Login with the Contoso identity provider",
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

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-openidconnectidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-openidconnectidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-openidconnectidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-openidconnectidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-openidconnectidentityprovider-from-identityproviderbase-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "displayName": "Login with the Contoso identity provider",
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

### <a name="example-3-retrieves-apple-identity-provider-only-for-azure-ad-b2c"></a>Exemplo 3: recupera o provedor de identidade da Apple (somente para o Azure AD B2C)

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_applemanagedidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider",
  "displayName": "Sign in with Apple",
  "developerId": "UBF8T346G9",
  "serviceId": "com.microsoft.rts.b2c.test.client",
  "keyId": "99P6D879C4",
  "certificateData": "******"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-applemanagedidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-applemanagedidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-applemanagedidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-applemanagedidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-applemanagedidentityprovider-from-identityproviderbase-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider",
  "id": "Apple-Managed-OIDC",
  "displayName": "Sign in with Apple",
  "developerId": "UBF8T346G9",
  "serviceId": "com.microsoft.rts.b2c.test.client",
  "keyId": "99P6D879C4",
  "certificateData": "******"
}
```
