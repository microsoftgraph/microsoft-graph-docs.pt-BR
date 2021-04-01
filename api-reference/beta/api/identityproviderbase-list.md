---
title: Lista identityProviders
description: Recupere uma lista de objetos identityProviderbase.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: a61ccdc32cc83c5e2a520e72b30a61d1478f7cd2
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491053"
---
# <a name="list-identityproviders"></a>Lista identityProviders
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recuperar uma lista de conjunto de objetos herdados  [de identityProviderBase](../resources/identityproviderbase.md).

Para um locatário do Azure AD, ele pode ser [socialIdentityProviders](../resources/socialidentityprovider.md) e/ou [objetos builtinIdentityProviders.](../resources/builtinidentityprovider.md)

Para um locatário do Azure AD B2C, pode ser [socialIdentityProviders,](../resources/socialidentityprovider.md) [objetos openIdConnectIdentityProviders](../resources/openidconnectidentityprovider.md) e/ou [appleIdentityProvider.](../resources/appleidentityprovider.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)|IdentityProvider.Read.All, IdentityProvider.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|IdentityProvider.Read.All, IdentityProvider.ReadWrite.All|

A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador Global
* Administrador do Provedor de Identidade Externa
* Administrador de fluxo de usuário de ID externa

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---------------|:----------|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [socialIdentityProvider](../resources/socialidentityprovider.md) e/ou [builtinIdentityProvider](../resources/builtinidentityprovider.md) no corpo da resposta para um locatário do Azure AD.

Para um locatário do Azure AD B2C, este método retorna um código de resposta e uma coleção de objetos `200 OK` [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) e/ou [appleIdentityProvider](../resources/appleidentityprovider.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="example-1-list-all-identityprovider-configured-in-an-azure-ad-tenant"></a>Exemplo 1: listar **toda a identidadeProvider** configurada em um locatário do Azure AD

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase",
  "isCollection": true
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/identityProviders",
   "value":[
      {
         "@odata.type": "microsoft.graph.builtInIdentityProvider",
         "id": "MSASignup-OAUTH",
         "identityProviderType": "MicrosoftAccount",
         "displayName": "MicrosoftAccount"
      },
      {
         "@odata.type": "#microsoft.graph.socialIdentityProvider",
         "id": "Facebook-OAUTH",
         "displayName": "Facebook",
         "identityProviderType": "Facebook",
         "clientId": "test",
         "clientSecret": "******"
      }
   ]
}
```

### <a name="example-2-list-all-identityprovider-configured-in-an-azure-ad-b2c-tenant"></a>Exemplo 2: listar **toda a identidadeProvider** configurada em um locatário do Azure AD B2C

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/identityProviders",
    "value": [
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "LinkedIn-OAUTH",
            "displayName": "linkedin",
            "identityProviderType": "LinkedIn",
            "clientId": "866xc0qtyy00ih",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.openIdConnectIdentityProvider",
            "id": "OIDC-V1-rtt_AD_Test-3e393390-ed2d-4794-97f6-5c1a1ccc61f7",
            "displayName": "OIDC AD Test",
            "clientId": "fe1b3476-rdca-4bef-b321-076fde19750b",
            "clientSecret": "******",
            "scope": "openid",
            "metadataUrl": "https://login.microsoftonline.com/sashawho.onmicrosoft.com/.well-known/openid-configuration",
            "domainHint": "",
            "responseType": "code",
            "responseMode": "form_post",
            "claimsMapping": {
                "userId": "oid",
                "displayName": "name",
                "givenName": "given_name",
                "surname": "family_name",
                "email": "unique_email"
            }
        },
        {
            "@odata.type": "#microsoft.graph.appleManagedIdentityProvider",
            "id": "Apple-Managed-OIDC",
            "displayName": "Sign in with Apple",
            "developerId": "UBF8T346G9",
            "serviceId": "com.microsoft.aad.b2c.iuyt.client",
            "keyId": "99P6DD87C4",
            "certificateData": "******"
        }
    ]
}

```
