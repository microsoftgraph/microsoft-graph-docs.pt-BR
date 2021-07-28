---
title: Criar identityProvider
description: Crie um novo objeto identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: ecc3882e4c5ea8106209e32e75a8589d05d2a4cc
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535432"
---
# <a name="create-identityprovider"></a>Criar identityProvider
Namespace: microsoft.graph

Crie um novo [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no Azure AD.

No Azure AD B2C, crie um novo [objeto socialIdentityProvider.](../resources/socialidentityprovider.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)|IdentityProvider.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|IdentityProvider.ReadWrite.All|

A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador global
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

No corpo da solicitação, forneça uma representação JSON de um [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no Azure AD.

No Azure AD B2C, forneça uma representação JSON do [objeto socialIdentityProvider.](../resources/socialidentityprovider.md)

Todas as propriedades listadas na tabela a seguir são necessárias.

### <a name="socialidentityprovider-object"></a>Objeto socialIdentityProvider

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|clientId|Cadeia de caracteres|O identificador do cliente para o aplicativo obtido ao registrar o aplicativo com o provedor de identidade.|
|clientSecret|Cadeia de caracteres|O segredo do cliente para o aplicativo obtido quando o aplicativo é registrado com o provedor de identidade. Isso é somente gravação. Uma operação de leitura retorna `****` .|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade.|
|identityProviderType|Cadeia de caracteres|Para um cenário B2B, valores possíveis: `Google`, `Facebook`. Para um cenário B2C, valores possíveis: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.|
|escopo|String|O escopo define as informações e permissões que você está procurando coletar do provedor de identidade personalizado.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma representação JSON de um objeto `201 Created` [socialIdentityProvider](../resources/socialidentityprovider.md) no corpo da resposta para locatários do Azure AD e do Azure AD B2C.

Caso não consiga, um `4xx` erro será retornado com detalhes específicos.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-a-specific-social-identity-provider-azure-ad-and-azure-ad-b2c"></a>Exemplo 1: Criar um provedor de identidade social específico (Azure AD e Azure AD B2C)

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "create_socialidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.socialIdentityProvider",
  "displayName": "Login with Amazon",
  "identityProviderType": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}
```

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
