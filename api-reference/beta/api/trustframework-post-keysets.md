---
title: Criar trustFrameworkKeySet
description: Crie um novo **objeto trustFrameworkKeySet.**
ms.localizationpriority: medium
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d63e2a51f2263bda959964dd22e70451cba9bab9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115306"
---
# <a name="create-trustframeworkkeyset"></a>Criar trustFrameworkKeySet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [trustFrameworkKeySet](../resources/trustframeworkkeyset.md). A ID do **trustFrameworkKeySet** é esperada na solicitação de criação; no entanto, ele pode ser modificado pelo serviço. A ID modificada estará disponível na resposta e no header de local.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | TrustFrameworkKeySet.ReadWrite.All   |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | TrustFrameworkKeySet.ReadWrite.All    |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
|Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de um [objeto trustFrameworkKeySet.](../resources/trustframeworkkeyset.md)

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta, um header de local para o objeto recém-criado e um novo `201 Created` [objeto trustFrameworkKeySet](../resources/trustframeworkkeyset.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-an-empty-keyset"></a>Exemplo 1: Criar um keyset vazio
Esta é uma das operações mais úteis. Primeiro, você cria um keyset vazio. Em seguida, no novo keyset, você pode gerar uma chave, carregar um segredo manual e carregar um certificado ou uma tecla PKCS12. 

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra a solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkkeyset_from_trustframework1"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets
Content-type: application/json

{
  "id": "keyset1"  
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-trustframeworkkeyset-from-trustframework-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-trustframeworkkeyset-from-trustframework-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-trustframeworkkeyset-from-trustframework-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-trustframeworkkeyset-from-trustframework-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-trustframeworkkeyset-from-trustframework-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-trustframeworkkeyset-from-trustframework-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Location: /trustFramework/keySets('B2C_1A_keyset1')

{
  "id": "B2C_1A_keyset1",
  "keys": []
}
```

### <a name="example-2-create-a-keyset-with-a-key"></a>Exemplo 2: Criar um keyset com uma chave

Este é um cenário avançado em que você precisa saber o formato JSON Web Key compatível com [RFC 7517](https://tools.ietf.org/html/rfc7517#section-5) da chave.

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra a solicitação.
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkkeyset_from_trustframework"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets
Content-type: application/json

{
  "id": "keyset1",
  "keys": [
    {
      "k": "k-value",
      "x5c": [
        "x5c-value"
      ],
      "x5t": "x5t-value",
      "kty": "kty-value",
      "use": "use-value",
      "exp": 99,
      "nbf": 99,
      "kid": "kid-value",
      "e": "e-value",
      "n": "n-value",
      "d": "d-value",
      "p": "p-value",
      "q": "q-value",
      "dp": "dp-value",
      "dq": "dq-value",
      "qi": "qi-value"
    }
  ]
}
```

#### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Location: /trustFramework/keySets('B2C_1A_keyset1')

{
  "id": "B2C_1A_keyset1",
  "keys": [
    {
      "k": "k-value",
      "x5c": [
        "x5c-value"
      ],
      "x5t": "x5t-value",
      "kty": "kty-value",
      "use": "use-value",
      "exp": 99,
      "nbf": 99,
      "kid": "kid-value",
      "e": "e-value",
      "n": "n-value",
      "d": "d-value",
      "p": "p-value",
      "q": "q-value",
      "dp": "dp-value",
      "dq": "dq-value",
      "qi": "qi-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


