---
title: 'searchEntity: consulta'
description: Executa a consulta especificada no corpo da solicitação. Os resultados da pesquisa são fornecidos na resposta.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c699dab1c97d5b7650f42d4282e36d35b2769a31
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401796"
---
# <a name="searchentity-query"></a>searchEntity: consulta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Executa a consulta especificada no corpo da solicitação. Os resultados da pesquisa são fornecidos na resposta.

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference). 

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Mail. Read, mail. ReadWrite, Calendars. Read, Calendars. ReadWrite, files. Read. All, files. ReadWrite. All, sites. Read. All, sites. ReadWrite. All, ExternalItem. Read. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

```HTTP
POST /search/query
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Quest|coleção [searchRequest](../resources/searchrequest.md)|Uma coleção de uma ou mais solicitações de pesquisa cada formatadas em um blob JSON. Cada blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de paginação, os campos solicitados e a consulta de pesquisa real. <br> Esteja ciente das [limitações conhecidas](../resources/search-api-overview.md#known-limitations) de pesquisa de combinações específicas de tipos de entidade e da classificação ou agregação de resultados de pesquisa. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o `HTTP 200 OK` código de resposta e um objeto da coleção [searchResponse](../resources/searchresponse.md) no corpo da resposta.
 

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "search_query"
}-->

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "externalItem"
      ],
      "contentSources": [
        "/external/connections/connectionfriendlyname"
      ],
      "query": {
        "queryString": "contoso product"
      },
      "from": 0,
      "size": 25,
      "fields": [
        "title",
        "description"
      ]
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.searchResponse",
  "isCollection": true
} -->

```HTTP
HTTP/1.1 200 OK
Content-type: application/json
```

```json
{
  "value": [
    {
      "searchTerms": [
        "searchTerms-value"
      ],
      "hitsContainers": [
        {
          "hits": [
            {
              "hitId": "1",
              "rank": 1,
              "summary": "_summary-value",
              "resource": "The source field will contain the underlying graph entity part of the response"
            }
          ],
          "total": 47,
          "moreResultsAvailable": true
        }
      ]
    }
  ]
}
```

## <a name="see-also"></a>Confira também
- [Mensagens de email](/graph/search-concept-messages) de pesquisa
- [Eventos de calendário](/graph/search-concept-events) de pesquisa
- Pesquisar conteúdo no SharePoint e no OneDrive ([arquivos, listas e sites](/graph/search-concept-files))
- Dados [de tipos personalizados de pesquisa (conectores do gráfico)](/graph/search-concept-custom-types)
- [Classificar](/graph/search-concept-sort) resultados de pesquisa
- Usar [agregações](/graph/search-concept-aggregations) para refinar os resultados da pesquisa


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


