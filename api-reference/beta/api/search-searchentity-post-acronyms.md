---
title: Criar acrônimo
description: Crie um novo objeto de acrônimo.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 4a873ed5b626424b8292473c778c1e45df7f6a18
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338070"
---
# <a name="create-acronym"></a>Criar acrônimo
Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto de acrônimo](../resources/search-acronym.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)| SearchConfiguration.Read.All, SearchConfiguration.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)| Sem suporte. |
|Aplicativo| SearchConfiguration.Read.All, SearchConfiguration.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /search/acronyms
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto acrônimo](../resources/search-acronym.md) .

A tabela a seguir mostra as propriedades que estão disponíveis quando você cria um [acrônimo](../resources/search-acronym.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|Uma breve descrição do acrônimo que fornece aos usuários mais informações sobre o acrônimo e o que ele representa. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|displayName|String|O formulário curto ou acrônimo real. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|standsFor|Coleção String|O que o acrônimo significa.|
|state|microsoft.graph.search.answerState|Estado do acrônimo. Os valores possíveis são: `published`, `draft`, `excluded`ou `unknownFutureValue`.|
|webUrl|String|A URL da página ou site onde os usuários podem ir para obter mais informações sobre o acrônimo. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `200 Ok`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_acronym_from_acronyms"
}-->
```http
POST https://graph.microsoft.com/beta/search/acronyms
Content-Type: application/json

{
  "displayName": "DNN",
  "standsFor": "Deep Neural Network",
  "description": "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.",
  "webUrl": "http://microsoft.com/deep-neural-network",
  "state": "draft"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-acronym-from-acronyms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-acronym-from-acronyms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-acronym-from-acronyms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-acronym-from-acronyms-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-acronym-from-acronyms-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-acronym-from-acronyms-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.acronym"
}-->
```http
HTTP/1.1 200 Ok
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

