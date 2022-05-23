---
title: Obter connectionQuota
description: Recupere as propriedades e as relações de uma connectionQuota.
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a1d5720de230a4ab21c79dc24b4ab6b480ae88ab
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629271"
---
# <a name="get-connectionquota"></a>Obter connectionQuota

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e as relações de um [objeto connectionQuota](../resources/externalconnectors-connectionquota.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte. |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | ExternalConnection.ReadWrite.OwnedBy |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/quota
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte a [todos os parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e um [objeto externalConnection](../resources/externalconnectors-externalconnection.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/quota
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-connection-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-connection-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Resposta
<!-- markdownlint-enable MD024 -->

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.connectionQuota"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "itemsRemaining": 7000
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-12-02 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connectionQuota",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
