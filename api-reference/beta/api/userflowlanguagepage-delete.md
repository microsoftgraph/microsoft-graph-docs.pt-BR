---
title: Excluir userFlowLanguagePage
description: Exclui os valores em um objeto userFlowLanguagePage.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ce15fce0565a7e7fdeb704d645a177342c7ad17d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444613"
---
# <a name="delete-userflowlanguagepage"></a>Excluir userFlowLanguagePage

Namespace: microsoft.graph

Exclui os valores em um [objeto userFlowLanguagePage.](../resources/userflowlanguagepage.md) Você só pode excluir os valores em um overridesPage, que é usado para personalizar os valores mostrados a um usuário durante uma jornada do usuário definida por um fluxo de usuário.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|IdentityUserFlow.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|IdentityUserFlow.ReadWrite.All|

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
DELETE /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/$value
DELETE /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/$value
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguagepage"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages/phonefactor/$value
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowlanguagepage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowlanguagepage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowlanguagepage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userflowlanguagepage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
