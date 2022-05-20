---
title: Criar qna
description: Crie um novo objeto qna.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d3b2266238a74b052aba433c75e5b91d08669386
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602718"
---
# <a name="create-qna"></a>Criar qna
Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto qna](../resources/search-qna.md) .

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
POST /search/qnas
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto qna](../resources/search-qna.md) .

A tabela a seguir mostra as propriedades que estão disponíveis quando você cria um [qna](../resources/search-qna.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Pergunta exibida nos resultados da pesquisa. Herdado de [searchAnswer](../resources/search-searchAnswer.md).|
|descrição|Cadeia de caracteres|Resposta exibida nos resultados da pesquisa. Herdado de [searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|Link da URL do Qna. Quando os usuários clicarem nesse qna nos resultados da pesquisa, eles acessarão essa URL. Herdado de [searchAnswer](../resources/search-searchAnswer.md).|
|availabilityStartDateTime|DateTimeOffset|Carimbo de data/hora de quando o qna começará a aparecer como um resultado de pesquisa. Defina `null` como sempre disponível.|
|availabilityEndDateTime|DateTimeOffset|Carimbo de data/hora de quando o qna será interrompido para aparecer como um resultado de pesquisa. Defina `null` como sempre disponível.|
|languageTags|Coleção de cadeias de caracteres|Lista de países ou regiões capazes de exibir este qna.|
|Plataformas|Coleção microsoft.graph.devicePlatformType|Lista de dispositivos e sistemas operacionais capazes de exibir esse qna. Os valores possíveis são: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[coleção microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Variações de um qna para diferentes países ou dispositivos. Use quando precisar mostrar conteúdo diferente para os usuários com base em seu dispositivo, país/região ou ambos. As configurações de data e grupo serão aplicadas a todas as variações.|
|palavras-chave|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Palavras-chave que disparam esse qna para aparecer nos resultados da pesquisa.|
|state|microsoft.graph.search.answerState|Estado do qna. Os valores possíveis são`draft`: `published`, , `excluded`ou `unknownFutureValue`.|
|groupIds|Coleção de cadeias de caracteres|Lista de grupos de segurança capazes de exibir este qna.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta com a ID da pergunta e resposta criadas.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_qna_from_qnas"
}-->
```http
POST https://graph.microsoft.com/beta/search/qnas
Content-Type: application/json

{
  "displayName": "Global Country Holidays",
  "webUrl": "http://www.contoso.com/",
  "description": "The dates that Contoso offices will be closed to observe holidays. These dates may differ from the actual date of the holiday in cases where the holiday falls on a weekend.    <table>    <thead>    <tr>    <td><strong>2021 Dates</strong></td>    <td><strong>Holiday</strong></td>    </tr>    </thead>    <tbody>    <tr>        <td>January 1, 2021</td>        <td>New Year's Day</td>    </tr>        <tr>        <td>January 18, 2021</td>        <td>Martin Luther King Day</td>    </tr>        <tr>        <td>February 15, 2021</td>        <td>Presidents Day</td>    </tr>        <tr>        <td>May 31, 2021</td>        <td>Memorial Day</td>    </tr>        <tr>        <td>July 5, 2021</td>        <td>Independence Day</td>    </tr>        <tr>        <td>September 6, 2021</td>        <td>Labor Day</td>    </tr>        <tr>        <td>November 25, 2021 - November 26, 2021</td>        <td>Thanksgiving Day and Day after Thanksgiving</td>    </tr>    <tr>        <td>December 23, 2021 - December 24, 2021</td>        <td>Christmas Eve and Christmas Day</td>    </tr>    </tbody>    </table>",
  "keywords":  {
    "keywords": ["new years day", "martin luther king day", "presidents day", "memorial day", "independence day", "labor day", "thanksgiving", "christmas"],
    "reservedKeywords": ["holidays", "paid days off"],
    "matchSimilarKeywords": true
  },
  "availabilityStartDateTime": "2020-09-21T20:01:37Z",
  "availabilityEndDateTime": "2021-12-31T20:01:37Z",
  "languageTags": ["en-us"],
  "platforms": ["ios"],
  "state": "published"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-qna-from-qnas-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-qna-from-qnas-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-qna-from-qnas-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-qna-from-qnas-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-qna-from-qnas-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-qna-from-qnas-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.qna"
}-->
```http
HTTP/1.1 201 CREATED
Location: /733b26d5-af76-4eea-ac69-1a0ce8716897
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

