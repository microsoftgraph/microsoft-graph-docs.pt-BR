---
title: Atualizar indicador
description: Atualize as propriedades de um objeto bookmark.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 5eddbf0551e7acddd1af15123c927201b3aba73d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337992"
---
# <a name="update-bookmark"></a>Atualizar indicador
Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um objeto bookmark](../resources/search-bookmark.md) .

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
PATCH /search/bookmarks/{bookmarksId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto bookmark](../resources/search-bookmark.md) . Fornecer os valores para campos relevantes que devem ser atualizados. As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base em alterações em outros valores de propriedade. Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.
>**Observação:** As atualizações das propriedades da coleção atualizarão toda a coleção. Todas as atualizações de uma coleção, como palavras-chave ou categorias, substituirão totalmente a coleção.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome do indicador exibido nos resultados da pesquisa. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|descrição|String|Descrição do indicador mostrada na página de resultados da pesquisa. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|Link da URL do indicador. Quando os usuários clicarem nesse indicador nos resultados da pesquisa, eles irão para essa URL. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|categories|String collection|Categorias comumente usadas para descrever esse indicador. Por exemplo, IT e RH.|
|availabilityStartDateTime|DateTimeOffset|Carimbo de data/hora de quando o indicador começará a aparecer como um resultado de pesquisa. Definir como `null` para sempre disponível.|
|availabilityEndDateTime|DateTimeOffset|Carimbo de data/hora de quando o indicador será parar para aparecer como resultado da pesquisa. Definir como `null` para sempre disponível.|
|languageTags|Coleção de cadeias de caracteres|Lista de países ou regiões capazes de exibir esse indicador.|
|plataformas|coleção microsoft.graph.devicePlatformType|Lista de dispositivos e sistemas operacionais capazes de exibir esse indicador. Os valores possíveis são: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[coleção microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Variações de um indicador para diferentes países ou dispositivos. Use quando precisar mostrar conteúdo diferente para os usuários com base em seu dispositivo, país/região ou ambos. As configurações de data e grupo serão aplicadas a todas as variações.|
|powerAppIds|Coleção de cadeias de caracteres|Lista de Power Apps associados a esse indicador. Se os usuários adicionarem Power Apps existentes a um indicador, eles poderão concluir tarefas, como inserir o período de férias ou relatar despesas na página de resultados da pesquisa.|
|palavras-chave|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Palavras-chave que disparam esse indicador aparecem nos resultados da pesquisa.|
|state|microsoft.graph.search.answerState|Estado do indicador. Os valores possíveis são: `published`, `draft`, `excluded`ou `unknownFutureValue`.|
|groupIds|Coleção de cadeias de caracteres|Lista de grupos de segurança capazes de exibir esse indicador.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookmark"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/search/bookmarks/{bookmarksId}
Content-Type: application/json

{
  "description": "Book a fancy vacation in Tuscany or browse museums in Florence."
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookmark-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookmark-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookmark-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookmark-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-bookmark-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-bookmark-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

