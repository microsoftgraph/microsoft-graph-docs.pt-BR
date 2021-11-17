---
title: Atualizar identityProvider
description: Atualizar propriedades de um identityProvider.
ms.localizationpriority: medium
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 030adb5a36c10624d205db25b48349d1e09110a9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61014939"
---
# <a name="update-identityprovider"></a>Atualizar identityProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades do provedor de identidade especificado configurado no locatário.

Entre os tipos de provedores derivados de identityProviderBase, você pode atualizar atualmente um [recurso socialIdentityProvider](../resources/socialidentityprovider.md) no Azure AD. No Azure AD B2C, essa operação pode atualizar atualmente [um recurso socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md)ou um recurso [appleManagedIdentityProvider.](../resources/applemanagedidentityprovider.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)|IdentityProvider.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo| IdentityProvider.ReadWrite.All|

A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador Global
* Administrador do Provedor de Identidade Externa

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/identityProviders/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---------------|:----------|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça um objeto JSON com uma ou mais propriedades que precisam ser atualizadas para um [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no locatário do Azure AD.

No Azure AD B2C, forneça um objeto JSON com uma ou mais propriedades que precisam ser atualizadas para [um objeto socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md)ou [um objeto appleManagedIdentityProvider.](../resources/applemanagedidentityprovider.md)

### <a name="socialidentityprovider-object"></a>Objeto socialIdentityProvider

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|O identificador do cliente para o aplicativo obtido ao registrar o aplicativo com o provedor de identidade.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido quando o aplicativo é registrado com o provedor de identidade. Isso é somente gravação. Uma operação de leitura retorna `****`.|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|

### <a name="openidconnectidentityprovider-object"></a>Objeto openIdConnectIdentityProvider

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|O identificador do cliente para o aplicativo obtido ao registrar o aplicativo com o provedor de identidade.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade. O clientSecret tem uma dependência de **responseType**. <ul><li>Quando **responseType** é `code` , um segredo é necessário para a troca de código de auth.</li><li>Quando **responseType** é `id_token` o segredo não é necessário porque não há troca de código. O id_token é retornado diretamente da resposta de autorização.</li></ul>|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|
|domainHint|String|A dica de domínio pode ser usada para pular diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa. Esse tipo complexo captura esse mapeamento.|
|metadataUrl|Cadeia de caracteres|A URL do documento de metadados do provedor de Conexão OpenID. Cada provedor Conexão de identidade OpenID descreve um documento de metadados que contém a maioria das informações necessárias para executar a login. Isso inclui informações como as URLs a ser usadas e o local das chaves de assinatura públicas do serviço. O documento Conexão de metadados do OpenID está sempre localizado em um ponto de extremidade que termina em `.well-known/openid-configuration` . Forneça a URL de metadados para o provedor Conexão de identidade openid que você adicionar.|
|responseMode|String|O modo de resposta define o método usado para enviar dados de volta do provedor de identidade personalizado para o Azure AD B2C. Valores possíveis: `form_post` , `query` .|
|responseType|Cadeia de caracteres|O tipo de resposta descreve o tipo de informação enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizado. Valores possíveis: `code` , `id_token` , `token` .|
|escopo|String|O escopo define as informações e permissões que você está procurando coletar do provedor de identidade personalizado.|

### <a name="applemanagedidentityprovider-object"></a>Objeto appleManagedIdentityProvider

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|
|developerId|Cadeia de caracteres|O Identificador de desenvolvedor da Apple.|
|serviceId|Cadeia de caracteres|O identificador de serviço da Apple.|
|keyId|Cadeia de caracteres|O identificador de chave da Apple.|
|certificateData|Cadeia de caracteres|Os dados do certificado, que são uma longa sequência de texto do certificado, podem ser nulos.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`. Caso não consiga, um `4xx` erro será retornado com detalhes específicos.

## <a name="examples"></a>Exemplos

### <a name="example-1-update-a-specific-social-identity-provider-azure-ad-or-azure-ad-b2c"></a>Exemplo 1: Atualizar um provedor de **identidade social específico** (Azure AD ou Azure AD B2C)

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_socialidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Amazon-OAUTH
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.socialIdentityProvider",
  "clientSecret": "1111111111111"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-socialidentityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-socialidentityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-socialidentityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-socialidentityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-socialidentityprovider-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a>Exemplo 2: atualizar um provedor de identidade **Conexão OpenID específico** (somente para o Azure AD B2C)

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openidconnectprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/OIDC-V1-Nam_AD_Test-3e393390-ed2d-4794-97f6-5c999ccc61f7
Content-type: application/json

{
  "responseType": "id_token"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openidconnectprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openidconnectprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openidconnectprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openidconnectprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-openidconnectprovider-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-a-specific-apple-identity-provider-only-for-azure-ad-b2c"></a>Exemplo 3: atualizar um provedor de **identidade específico da Apple** (somente para o Azure AD B2C)

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_appleidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Apple-Managed-OIDC
Content-type: application/json

{
  "displayName": "Apple"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-appleidentityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-appleidentityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-appleidentityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-appleidentityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-appleidentityprovider-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
