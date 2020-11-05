---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para Pesquisar tipos personalizados
description: Você pode usar a API de pesquisa da Microsoft para importar dados externos por meio do recurso [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) e executar consultas de pesquisa nesse conteúdo externo.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 671f8feb37203d9fea652a203dfe4d094e5a8024
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921743"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors"></a>Usar a API de pesquisa da Microsoft para Pesquisar tipos personalizados importados usando conectores do Microsoft Graph

Use a API de pesquisa da Microsoft para pesquisar conteúdo ingerido e indexado pelos [conectores do Microsoft Graph](/microsoftsearch/connectors-overview). O conteúdo é importado por meio de [conectores internos](/microsoftsearch/connectors-gallery) fornecidos pela Microsoft ou por meio de conectores personalizados implementados usando a [API de inclusão de conectores do Microsoft Graph](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

Após o conteúdo ter sido importado e indexado, você poderá usar a API de pesquisa para consultar o conteúdo.

Para Pesquisar tipos personalizados, especifique as propriedades a seguir no corpo da solicitação do método de [consulta](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) :

- A propriedade **ContentSources** para incluir a ID de conexão atribuída durante a configuração do conector. Você pode passar várias IDs de conexão para pesquisar em várias conexões. Os resultados são retornados em uma única lista, classificados por várias conexões.

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- A propriedade **EntityTypes** como `externalItem` .

- A propriedade **Fields** para incluir os campos no item externo a serem recuperados. Observe que, se você não incluir nenhum **campo** na solicitação, a resposta conterá todos os campos marcados como *recuperáveis* no esquema de dados especificado para as conexões especificadas na propriedade **ContentSources** .

Além disso, você pode agregar resultados de pesquisa com base nas propriedades de um [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) que são numéricos ou de cadeia de caracteres, e que estão definidos como refinável no [esquema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true). Para obter mais informações, consulte [refinar resultados de pesquisa usando agregações](search-concept-aggregation.md).

## <a name="example"></a>Exemplo

Neste exemplo, o conteúdo do banco de dados [AdventureWorks](/sql/samples/adventureworks-install-configure) foi incluído usando o conector interno do Azure SQL.

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

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)