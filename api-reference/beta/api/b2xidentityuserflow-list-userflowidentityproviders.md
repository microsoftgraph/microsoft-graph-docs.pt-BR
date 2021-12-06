---
title: Listar um userflowidentityproviders
description: Listar todos os identityProviders em um b2xIdentityUserFlow.
ms.localizationpriority: medium
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 0e8fc7a4c82c2f08a695d6a003a01186409e8049
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60999771"
---
# <a name="list-a-userflowidentityproviders"></a>Listar um userflowidentityproviders

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter os provedores de identidade em um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|IdentityUserFlow.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo| IdentityUserFlow.ReadWrite.All|

A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador global
* Administrador de fluxo de usuário de ID externa

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---------------|:----------|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` representação JSON dos [identityProviders](../resources/identityproviderbase.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_userflowIdentityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflow-list-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflow-list-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflow-list-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflow-list-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-b2xuserflow-list-userflowidentityproviders-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.identityProviderBase)",
    "value": [
  {
            "@odata.type": "#microsoft.graph.builtInIdentityProvider",
            "id": "AADSignup-OAUTH",
            "displayName": "Azure Active Directory Sign up",
            "identityProviderType": "AADSignup"
        },
        {
            "@odata.type": "#microsoft.graph.builtInIdentityProvider",
            "id": "MSASignup-OAUTH",
            "displayName": "Microsoft Account (Preview)",
            "identityProviderType": "MicrosoftAccount"
        },
        {
            "@odata.type": "#microsoft.graph.builtInIdentityProvider",
            "id": "EmailOtpSignup-OAUTH",
            "displayName": "Email one-time passcode (Preview)",
            "identityProviderType": "EmailOTP"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Facebook-OAUTH",
            "displayName": "Facebook",
            "identityProviderType": "Facebook",
            "clientId": "clientIdFromFacebook",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Google-OAuth",
            "type": "Google",
            "name": "Google",
            "clientId": "clientIdFromGoogle",
            "clientSecret": "*****"
        }
    ]
}

```
