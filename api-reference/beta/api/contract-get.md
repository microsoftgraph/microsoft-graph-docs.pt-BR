---
title: Obter Contrato
description: Recupere as propriedades e as relações do objeto contract.
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d0feac49510b5d85af4ceae6ab647147a29fe3d0
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63668630"
---
# <a name="get-contract"></a>Obter Contrato

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e as relações do [objeto contract](../resources/contract.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e [um objeto Contract](../resources/contract.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contracts/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-contract-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-contract-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
