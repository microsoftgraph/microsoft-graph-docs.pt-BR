---
title: Excluir um userFlowIdentityProvider
description: Exclua um identityProvider de um b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 85fff2d0fab5d9d098aa7cae780c99faece3916f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439641"
---
# <a name="delete-a-userflowidentityprovider"></a>Excluir um userFlowIdentityProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclua um provedor de identidade de um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md) Para fluxos de usuários de autoatendados, os valores podem ser `Google-OAUTH` ou `Facebook-OAUTH` .

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)|IdentityUserFlow.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo| IdentityUserFlow.ReadWrite.All|

A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador global
* Administrador de fluxo de usuário de ID externa

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
DELETE/identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/{id}/$ref
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---------------|:----------|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`. Se não tiver êxito, `4xx` um erro será retornado com os detalhes de erro específicos.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_userflowIdentityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/{identityProvider-id}/$ref
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
