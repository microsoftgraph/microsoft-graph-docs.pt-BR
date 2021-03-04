---
title: Criar permissionGrantPolicy
description: Cria um objeto permissionGrantPolicy que descreve as condições sob as quais as permissões podem ser concedidas.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 0e682ed0849ac6985b651658a0e06ef2811ff149
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433863"
---
# <a name="create-permissiongrantpolicy"></a>Criar permissionGrantPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Cria uma [permissionGrantPolicy](../resources/permissiongrantpolicy.md). Uma política de concessão de permissão é usada para descrever as condições em que as permissões podem ser concedidas (por exemplo, durante o consentimento do aplicativo).

Depois de criar a política de concessão de permissão, você pode adicionar [conjuntos](permissiongrantpolicy-post-includes.md) de condições para adicionar regras correspondentes e adicionar conjuntos de condições [de](permissiongrantpolicy-post-excludes.md) exclusão para adicionar regras de exclusão.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | PermissionGrantPolicy.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | PermissionGrantPolicy.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
POST /policies/permissionGrantPolicies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:----------|
| Autorização | {token} de portador. Obrigatório.  |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de [um objeto permissionGrantPolicy.](../resources/permissiongrantpolicy.md)

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto permissionGrantPolicy](../resources/permissiongrantpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "create_permissiongrantpolicy"
}-->

```http
POST https://graph.microsoft.com/beta/policies/permissionGrantPolicies
Content-Type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```
