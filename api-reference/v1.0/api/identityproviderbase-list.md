---
title: Lista identityProviders
description: Recupere uma lista de objetos identityProviderbase.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 5a2c57f7a0d36a4f1fc865bd010f4d9ce7052925
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579782"
---
# <a name="list-identityproviders"></a>Lista identityProviders
Namespace: microsoft.graph

Recuperar uma lista de conjunto de objetos herdados  [de identityProviderBase](../resources/identityproviderbase.md).

Para um locatário do Azure AD, ele pode ser [socialIdentityProviders](../resources/socialidentityprovider.md) e/ou [objetos builtinIdentityProviders.](../resources/builtinidentityprovider.md)

Para um locatário do Azure AD B2C, ele pode ser [objetos socialIdentityProviders.](../resources/socialidentityprovider.md)

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

Para um locatário do Azure AD B2C, este método retorna um código de resposta e uma coleção de `200 OK` [objetos socialIdentityProvider](../resources/socialidentityprovider.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-list-all-identity-providers-configured-in-an-azure-ad-tenant"></a>Exemplo 1: listar todos os provedores de identidade configurados em um locatário do Azure AD

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/identityProviders
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

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
   "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/identityProviders",
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

### <a name="example-2-list-all-identityprovider-objects-configured-in-an-azure-ad-b2c-tenant"></a>Exemplo 2: Listar todos os objetos identityProvider configurados em um locatário do Azure AD B2C

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/identityProviders
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/identityProviders",
    "value": [
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "LinkedIn-OAUTH",
            "displayName": "linkedin",
            "identityProviderType": "LinkedIn",
            "clientId": "866xc0qtyy00ih",
            "clientSecret": "******"
        }
    ]
}

```
