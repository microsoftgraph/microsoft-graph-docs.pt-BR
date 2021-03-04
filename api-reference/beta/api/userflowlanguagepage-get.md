---
title: Obter userFlowLanguagePage
description: Leia os valores em um objeto userFlowLanguagePage para um idioma em um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0848078f889b5d959cadb2ec5c403d1d1edf3cb9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433457"
---
# <a name="get-userflowlanguagepage"></a>Obter userFlowLanguagePage

Namespace: microsoft.graph

Leia os valores em [um objeto userFlowLanguagePage](../resources/userflowlanguagepage.md) para um idioma em um fluxo de usuário. Esses valores são mostrados a um usuário durante uma jornada do usuário definida por um fluxo de usuários.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All|

A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador global
* Administrador de Fluxo de Usuário de Identidade Externa

## <a name="http-request"></a>Solicitação HTTP

Para fazer referência ao conteúdo dentro do objeto, você deve usar `$value` . Isso retorna o conteúdo dentro do objeto e permite que você o referencia diretamente.

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages/{id}/defaultPages/{id}/$value
GET /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
GET /identity/b2xUserFlows/{id}/languages/{id}/defaultPages/{id}/$value
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userFlowLanguagePage](../resources/userflowlanguagepage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages/idpselections/$value
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguagepage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguagepage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguagepage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguagepage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguagePage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "LocalizedStrings": [
      {
        "ElementType": "ClaimsProvider",
        "ElementId": null,
        "StringId": "AmazonExchange",
        "Override": false,
        "Value": "Amazon"
      },
      {
        "ElementType": "ClaimsProvider",
        "ElementId": null,
        "StringId": "FacebookExchange",
        "Override": false,
        "Value": "Facebook"
      }
   ]
}
```
