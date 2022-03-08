---
title: Atualizar qna
description: Atualize as propriedades de um objeto qna.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: da045a3ed91bdc6ad5441fe9a854d225c144208d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338149"
---
# <a name="update-qna"></a>Atualizar qna
Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto qna](../resources/search-qna.md) .

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
PATCH /search/qna/{qnaId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto qna](../resources/search-qna.md) . Fornecer os valores para campos relevantes que devem ser atualizados. As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base em alterações em outros valores de propriedade. Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.
>**Observação:** As atualizações das propriedades da coleção atualizarão toda a coleção. Todas as atualizações de uma coleção, como palavras-chave ou categorias, substituirão totalmente a coleção.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Pergunta exibida nos resultados da pesquisa. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|descrição|String|Resposta exibida nos resultados da pesquisa. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|Link de URL de Qna. Quando os usuários clicarem nesse qna nos resultados da pesquisa, eles irão para essa URL. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|availabilityStartDateTime|DateTimeOffset|Timestamp de quando a qna começará a aparecer como um resultado de pesquisa. Definir como `null` para sempre disponível.|
|availabilityEndDateTime|DateTimeOffset|Timestamp de quando a qna será parada para aparecer como um resultado de pesquisa. Definir como `null` para sempre disponível.|
|languageTags|String collection|Lista de países ou regiões capazes de exibir esse qna.|
|plataformas|coleção microsoft.graph.devicePlatformType|Lista de dispositivos e sistemas operacionais capazes de exibir esse qna. Os valores possíveis são: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[coleção microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Variações de uma qna para diferentes países ou dispositivos. Use quando precisar mostrar conteúdo diferente para os usuários com base em seu dispositivo, país/região ou ambos. As configurações de data e grupo serão aplicadas a todas as variações.|
|palavras-chave|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Palavras-chave que disparam esse qna aparecem nos resultados da pesquisa.|
|state|microsoft.graph.search.answerState|Estado da qna. Os valores possíveis são: `published`, `draft`, `excluded`ou `unknownFutureValue`.|
|groupIds|Coleção de cadeias de caracteres|Lista de grupos de segurança capazes de exibir esse qna.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_qna"
}-->
``` http
PATCH https://graph.microsoft.com/beta/search/qna/{qnaId}
Content-Type: application/json

{
    "description": "The dates that Contoso offices will be closed to observe holidays. These dates may differ from the actual date of the holiday in cases where the holiday falls on a weekend."
}
```


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}-->
``` http
HTTP/1.1 204 No Content
```

