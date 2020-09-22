---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para Pesquisar tipos personalizados
description: Você pode usar a API de pesquisa da Microsoft para importar dados externos por meio do recurso [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) e executar consultas de pesquisa nesse conteúdo externo.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: b125b8f923e941ad73d5c578e99a67fdd9ea9eea
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192599"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors"></a>Usar a API de pesquisa da Microsoft para Pesquisar tipos personalizados importados usando conectores do Microsoft Graph

Use a API de pesquisa da Microsoft para pesquisar conteúdo ingerido e indexado pelos [conectores do Microsoft Graph](https://docs.microsoft.com/microsoftsearch/connectors-overview). O conteúdo é importado por meio de [conectores internos](https://docs.microsoft.com/microsoftsearch/connectors-gallery) fornecidos pela Microsoft ou por meio de conectores personalizados implementados usando a [API de inclusão de conectores do Microsoft Graph](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

Após o conteúdo ter sido importado e indexado, você poderá usar a API de pesquisa para consultar o conteúdo.

Para Pesquisar tipos personalizados, especifique as propriedades a seguir no corpo da solicitação do método de [consulta](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) :

- A propriedade **ContentSources** para incluir a ID de conexão atribuída durante a configuração do conector. Você pode passar várias IDs de conexão para pesquisar em várias conexões. Os resultados são retornados em uma única lista, classificados por várias conexões.

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- A propriedade **EntityTypes** como `externalItem` .

- A propriedade **Fields** para incluir os campos no item externo a serem recuperados.

## <a name="example"></a>Exemplo

Neste exemplo, o conteúdo do banco de dados [AdventureWorks](https://docs.microsoft.com/sql/samples/adventureworks-install-configure) foi incluído usando o conector interno do Azure SQL.

### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "externalItem"
      ],
      "contentSources": [
          "/external/connections/azuresqlconnector",
          "/external/connections/azuresqlconnector2"
      ],
      "query": {
        "queryString": "yang"
      },
      "from": 0,
      "size": 25,
      "fields": [
        "BusinessEntityID",
        "firstName",
        "lastName"
      ]
    }
  ]
}
```

### <a name="response"></a>Resposta

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
  "value": [
    {
      "searchTerms": ["ya"],
      "hitsContainers": [
        {
          "total": 2,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "AAMkADc0NDNlNTE0",
              "rank": 1,
              "summary": "<ddd/>",
              "contentSource": "/external/connections/azuresqlconnector",
              "resource": {
                "@odata.type": "#microsoft.graph.externalItem",
                "properties": {
                  "businessEntityID": 20704,
                  "firstName": "Amy",
                  "lastName": "Yang"
                }
              }
            },
           {
              "hitId": "AQMkADg3M2I3YWMyLTEwZ",
              "rank": 2,
              "summary": "<ddd/>",
              "contentSource": "/external/connections/azuresqlconnector2",
              "resource": {
                "@odata.type": "#microsoft.graph.externalItem",
                "properties": {
                  "businessEntityID": 20704,
                  "shortdescription": "Contoso maintenance guidelines",
                  "firstName": "Amy",
                  "lastName": "Yang"
                }
              }
            },
          ]
        }
      ]
    }
  ]
}
```

## <a name="known-limitations"></a>Limitações conhecidas

- Você deve especificar a propriedade **Fields** para obter campos recuperáveis no esquema de pesquisa.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
