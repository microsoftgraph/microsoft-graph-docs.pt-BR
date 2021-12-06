---
title: Atualizar b2cAuthenticationMethodsPolicy
description: Atualize as propriedades de um objeto b2cAuthenticationMethodsPolicy.
ms.localizationpriority: high
author: namkedia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1b31c64e4648b212fb98d0f9751c7fb0606be7cb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994933"
---
# <a name="update-b2cauthenticationmethodspolicy"></a>Atualizar b2cAuthenticationMethodsPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um objeto [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões|
|:---------------------------------------|:---------------|
| Delegada (conta corporativa ou de estudante)     | Policy.ReadWrite.AuthenticationMethod|
| Delegada (conta Microsoft pessoal) | Policy.ReadWrite.AuthenticationMethod|
| Aplicativo                            | Policy.ReadWrite.AuthenticationMethod|

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do objeto [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).

A tabela a seguir mostra as propriedades obrigatórias ao atualizar [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|isEmailPasswordAuthenticationEnabled|Booliano|O administrador de locatário pode configurar contas locais usando o email se o método de autenticação de email e senha estiver habilitado.|
|isUserNameAuthenticationEnabled|Booliano|O administrador de locatários pode configurar contas locais usando o nome de usuário se o método de autenticação do nome de usuário e senha estiver habilitado.|
|isPhoneOneTimePasswordAuthenticationEnabled|Boolean|O administrador de locatários poderá configurar contas locais usando o número de telefone se o número de telefone e o método de autenticação de senha única estiver habilitado.|

## <a name="response"></a>Resposta

Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy

{
    "isEmailPasswordAuthenticationEnabled": false,
    "isUserNameAuthenticationEnabled": true,
    "isPhoneOneTimePasswordAuthenticationEnabled": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-b2cauthenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/patch-b2cauthenticationmethodspolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update b2cauthenticationmethodspolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
