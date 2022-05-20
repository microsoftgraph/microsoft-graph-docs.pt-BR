---
title: Criar indicador
description: Crie um novo objeto de indicador.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 84283c08a8e80427ff34a310cbcae799bd26ecef
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602746"
---
# <a name="create-bookmark"></a>Criar indicador
Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto de indicador](../resources/search-bookmark.md) .

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
}-->
```http
POST /search/bookmarks
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto de indicador](../resources/search-bookmark.md) .

A tabela a seguir mostra as propriedades que estão disponíveis quando você cria um [indicador](../resources/search-bookmark.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome do indicador exibido nos resultados da pesquisa. Herdado de [searchAnswer](../resources/search-searchAnswer.md).|
|descrição|String|Descrição do indicador mostrada na página de resultados da pesquisa. Herdado de [searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|Link da URL do indicador. Quando os usuários clicarem nesse indicador nos resultados da pesquisa, eles acessarão essa URL. Herdado de [searchAnswer](../resources/search-searchAnswer.md).|
|categories|String collection|Categorias comumente usadas para descrever esse indicador. Por exemplo, TI e RH.|
|availabilityStartDateTime|DateTimeOffset|Carimbo de data/hora de quando o indicador começará a aparecer como um resultado de pesquisa. Defina `null` como sempre disponível.|
|availabilityEndDateTime|DateTimeOffset|Carimbo de data/hora de quando o indicador será interrompido para aparecer como um resultado de pesquisa. Defina `null` como sempre disponível.|
|languageTags|Coleção de cadeias de caracteres|Lista de países ou regiões capazes de exibir esse indicador.|
|Plataformas|Coleção microsoft.graph.devicePlatformType|Lista de dispositivos e sistemas operacionais capazes de exibir esse indicador. Os valores possíveis são: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[coleção microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Variações de um indicador para diferentes países ou dispositivos. Use quando precisar mostrar conteúdo diferente para os usuários com base em seu dispositivo, país/região ou ambos. As configurações de data e grupo serão aplicadas a todas as variações.|
|powerAppIds|Conjunto de cadeias de caracteres|Lista de Power Apps associado a este indicador. Se os usuários adicionarem Power Apps existentes a um indicador, eles poderão concluir tarefas, como inserir o tempo de férias ou relatar despesas na página de resultados da pesquisa.|
|palavras-chave|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Palavras-chave que disparam esse indicador aparecem nos resultados da pesquisa.|
|state|microsoft.graph.search.answerState|Estado do indicador. Os valores possíveis são`draft`: `published`, , `excluded`ou `unknownFutureValue`.|
|groupIds|Coleção de cadeias de caracteres|Lista de grupos de segurança capazes de exibir esse indicador.|



## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `201 Created` código de resposta com a ID do indicador criado.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookmark_from_bookmarks"
}-->
```http
POST https://graph.microsoft.com/beta/search/bookmarks
Content-Type: application/json

{
  "displayName": "Contoso Install Site",
  "webUrl": "http://www.contoso.com/",
  "description": "Try or buy Contoso for Home or Business and view product information",
  "keywords":  {
    "keywords": ["Contoso", "install"],
    "reservedKeywords": ["Contoso"],
    "matchSimilarKeywords": true
  },
  "availabilityStartDateTime": null,
  "availabilityEndDateTime": null,
  "platforms": ["windows"],
  "targetedVariations": [
    {
      "languageTag": "es-es",
      "displayName": "Sitio de instalación Contoso",
      "description": "Pruebe o compre Contoso hogar o negocios y vea la información del producto"
    }
  ],
  "state": "published"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookmark-from-bookmarks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookmark-from-bookmarks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookmark-from-bookmarks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookmark-from-bookmarks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-bookmark-from-bookmarks-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-bookmark-from-bookmarks-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.bookmark"
}-->
```http
HTTP/1.1 201 CREATED
Location: /733b26d5-af76-4eea-ac69-1a0ce8716897
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

