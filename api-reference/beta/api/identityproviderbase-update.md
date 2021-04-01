---
title: Atualizar identityProvider
description: Atualizar propriedades de um identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 985a6d4c80187decd5770eca150f501786222a1c
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491048"
---
# <a name="update-identityprovider"></a>Atualizar identityProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no Azure AD.

Para o Azure AD B2C, atualize as propriedades de [um objeto socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [appleIdentityProvider.](../resources/appleidentityprovider.md)

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

No Azure AD B2C, forneça um objeto JSON com uma ou mais propriedades que precisam ser atualizadas para [um objeto socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [um objeto appleIdentityProvider.](../resources/appleidentityprovider.md)

### <a name="socialidentityprovider-object"></a>Objeto socialIdentityProvider

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|O identificador de cliente do aplicativo obtido ao registrar o aplicativo com o provedor de identidade.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo que é obtido quando o aplicativo é registrado com o provedor de identidade. Isso é somente para gravar. Uma operação de leitura retorna " \* \* \* \* ".|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|

### <a name="openidconnectidentityprovider-object"></a>Objeto openIdConnectIdentityProvider

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|O identificador de cliente do aplicativo obtido ao registrar o aplicativo com o provedor de identidade.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade. O clientSecret tem uma dependência de **responseType**. <ul><li>Quando **responseType** é `code` , um segredo é necessário para a troca de código de auth.</li><li>Quando **responseType** é `id_token` o segredo não é necessário porque não há troca de código. O id_token é retornado diretamente da resposta de autorização.</li></ul>|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|
|domainHint|Cadeia de caracteres|A dica de domínio pode ser usada para pular diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa. Esse tipo complexo captura esse mapeamento.|
|metadataUrl|Cadeia de caracteres|A URL do documento de metadados do provedor de identidade do OpenID Connect. Cada provedor de identidade do OpenID Connect descreve um documento de metadados que contém a maioria das informações necessárias para executar a conexão. Isso inclui informações como as URLs a ser usadas e o local das chaves de assinatura públicas do serviço. O documento de metadados do OpenID Connect está sempre localizado em um ponto de extremidade que termina em `.well-known/openid-configuration` . Forneça a URL de metadados para o provedor de identidade do OpenID Connect que você adicionar.|
|responseMode|Cadeia de caracteres|O modo de resposta define o método usado para enviar dados de volta do provedor de identidade personalizado para o Azure AD B2C. Valores possíveis: `form_post` , `query` .|
|responseType|Cadeia de caracteres|O tipo de resposta descreve o tipo de informação enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizado. Valores possíveis: `code` , `id_token` , `token` .|
|escopo|String|O escopo define as informações e permissões que você está procurando coletar do provedor de identidade personalizado.|

### <a name="applemanagedidentityprovider-object"></a>Objeto appleManagedIdentityProvider

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|
|developerId|Cadeia de caracteres|O identificador do Desenvolvedor apple.|
|serviceId|Cadeia de caracteres|O identificador do Desenvolvedor apple.|
|keyId|Cadeia de caracteres|O identificador apple key.|
|certificateData|Cadeia de caracteres|Os dados do certificado, que é uma longa cadeia de caracteres de texto do certificado, podem ser nulos.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Caso não consiga, um `4xx` erro será retornado com detalhes específicos.

## <a name="examples"></a>Exemplos

### <a name="example-1-update-a-specific-social-identity-provider-azure-ad-or-azure-ad-b2c"></a>Exemplo 1: Atualizar um provedor de **identidade social específico** (Azure AD ou Azure AD B2C)

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "update_socialidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Amazon-OAUTH
Content-type: application/json
Content-length: 41

{
  "clientSecret": "1111111111111"
}
```

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

### <a name="example-2-update-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a>Exemplo 2: atualizar um provedor de identidade **do OpenID Connect** específico (somente para o Azure AD B2C)

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "update_openidconnectprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/OIDC-V1-Nam_AD_Test-3e393390-ed2d-4794-97f6-5c999ccc61f7
Content-type: application/json
Content-length: 41

{
  "responseType": "id_token"
}
```

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

<!-- {
  "blockType": "request",
  "name": "update_appleidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Apple-Managed-OIDC
Content-type: application/json
Content-length: 41

{
  "displayName": "Apple"
}
```

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
