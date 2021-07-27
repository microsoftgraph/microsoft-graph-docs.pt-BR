---
title: Excluir identityProvider
description: Excluir um identityProvider existente.
localization_priority: Priority
author: namkedia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 72a59ad093fd43ebd457a8d22a9f0229a6120e15
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534569"
---
# <a name="delete-identityprovider-deprecated"></a>Excluir IdentityProvider (obsoleto)
Namespace: microsoft.graph

[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

Excluir o [identityProvider](../resources/identityprovider.md) existente.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)|IdentityProvider.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|Sem suporte.|

A conta corporativa ou de estudante deve ser um administrador global do locatário.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---------------|:----------|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

O exemplo a seguir exclui um **identityProvider**.

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "delete-identityprovider"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

