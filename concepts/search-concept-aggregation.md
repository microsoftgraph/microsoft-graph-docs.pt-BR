---
title: Usar a API Pesquisa da Microsoft no Microsoft Graph refinar consultas com agregação
description: Você pode usar a API Pesquisa da Microsoft para recuperar agregações
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: edb0618751d54ca58578d56f7ee835bd9eeb7638fd9d4a4f5602708c11d48e5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54138291"
---
# <a name="refine-search-results-using-aggregations-preview"></a>Refinar resultados de pesquisa usando agregação (visualização)

Refine os resultados da pesquisa e mostre sua distribuição no índice.

## <a name="example-1-request-aggregations-by-string-fields"></a>Exemplo 1: Solicitar agregação por campos de cadeia de caracteres

O exemplo a seguir pesquisa **recursos listItem** e agrega resultados por seu tipo de arquivo e classe de conteúdo, ambos são valores de cadeia de caracteres.

A resposta inclui dois [objetos searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) para as duas agregação:
- A **propriedade** key especifica o valor real (por ou ) para os objetos `FileType` `contentclass` **listItem** correspondentes que são agregados no mesmo bucket por esse valor.
- A **propriedade count** especifica o número de tais objetos agregados no mesmo bucket. Observe que esse número é uma aproximação do número de combinações e não fornecerá um número exato de combinações.
- Buckets de resultados agregados por tipo de arquivo são classificação por contagem em ordem decrescente. Neste exemplo, há 3 buckets para 3 tipos de arquivo: `docx` `xlsx` , e `pptx` .
- Buckets de resultados agregados por classe de conteúdo são classificação pelo valor de cadeia de caracteres da classe de conteúdo em ordem decrescente. Neste exemplo, há apenas um bucket com todos os objetos correspondentes compartilhando a mesma classe de conteúdo, `STS_ListItem_DocumentLibrary` .

### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
          "listItem"
      ],
      "query": {
          "queryString": "test"
      },
      "from": 0,
      "size": 25,
      "aggregations": [
          {
              "field": "FileType",
              "size": 20,
              "bucketDefinition": {
                  "sortBy": "count",
                  "isDescending": "true",
                  "minimumCount": 0
              }
          },
          {
              "field": "contentclass",
              "size": 15,
              "bucketDefinition": {
                  "sortBy": "keyAsString",
                  "isDescending": "true",
                  "minimumCount": 0
              }
          }
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
    "@odata.type": "#microsoft.graph.searchResponse",
    "hitsContainers": [
        {
            "@odata.type": "#microsoft.graph.searchHitsContainer",
            "hits": [
                "..."
            ],
            "total": 9,
            "moreResultsAvailable": false,
            "aggregations": [
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "FileType",
                    "buckets": [
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "docx",
                            "count": 5,
                            "aggregationFilterToken": "\"ǂǂ646f6378\""
                        },
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "xlsx",
                            "count": 3,
                            "aggregationFilterToken": "\"ǂǂ786c7378\""
                        },
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "pptx",
                            "count": 1,
                            "aggregationFilterToken": "\"ǂǂ70707478\""
                        }
                    ]
                },
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "contentclass",
                    "buckets": [
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "STS_ListItem_DocumentLibrary",
                            "count": 9,
                            "aggregationFilterToken": "\"ǂǂ5354535f4c6973744974656d5f446f63756d656e744c696272617279\""
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a>Exemplo 2: aplicar um filtro de agregação com base em uma solicitação anterior

Neste exemplo, aplicamos um filtro de agregação baseado na **agregaçãoFilterToken** retornada como o `docx` campo no exemplo `FileType` 1.

O valor da cadeia de caracteres atribuído à propriedade **aggregationFilters** segue o formato **"{field}: \\ "{aggregationFilterToken} \\ ""**. Se vários valores para o mesmo filtro são necessários, o valor de cadeia de caracteres atribuído à propriedade **aggregationFilters** deve seguir esse formato : **"{field}:or( \\ "{aggregationFilterToken1} \\ ", \\ "{aggregationFilterToken2} \\ ")"**.

### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
          "driveItem"
      ],
      "query": {
          "queryString": "test"
      },
      "from": 0,
      "size": 20,
      "aggregations": [
          {
              "field": "FileType",
              "size": 10,
              "bucketDefinition": {
                  "sortBy": "count",
                  "isDescending": "true",
                  "minimumCount": 0
              }
          }
      ],
      "aggregationFilters": [
        "FileType:\"ǂǂ68746d6c\""
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
    "@odata.type": "#microsoft.graph.searchResponse",
    "hitsContainers": [
        {
            "@odata.type": "#microsoft.graph.searchHitsContainer",
            "hits": [
                "..."
            ],
            "total": 69960,
            "moreResultsAvailable": true,
            "aggregations": [
            {
                "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                "field": "FileType",
                "buckets": [
                    {
                        "@odata.type": "#microsoft.substrateSearch.searchBucket",
                        "key": "html",
                        "count": 69960,
                        "aggregationFilterToken": "\"ǂǂ68746d6c\""
                    }
                ]
            }
        ]
        }
    ]
}
```

## <a name="example-3-request-aggregation-by-a-numeric-field"></a>Exemplo 3: Solicitar agregação por um campo numérico

O exemplo a seguir pesquisa **recursos driveItem** e agrega resultados por seu tamanho, que é um valor numérico. A solicitação especifica a agregação por intervalos de 3 tamanhos:
- Tamanho inferior a 100
- Tamanho entre 100 e 1000
- Tamanho 1000 ou superior

A resposta inclui 3 objetos **searchBucket,** um para cada agregação de intervalo de tamanho:
- Os 2 buckets dos intervalos de tamanho inferior não incluem nenhuma pesquisa.
- Todas as 9 combinações de pesquisa têm tamanhos 1000 ou superiores.

### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "driveItem"
            ],
            "query": {
                "queryString": "test"
            },
            "from": 0,
            "size": 10,
            "aggregations": [
                {
                    "field": "Size",
                    "size": 5,
                    "bucketDefinition": {
                        "sortBy": "keyAsNumber",
                        "isDescending": "true",
                        "minimumCount": 0,
                        "ranges": [
                            {
                                "to": "100"
                            },
                            {
                                "from": "100",
                                "to": "1000"
                            },
                            {
                                "from": "1000"
                            }
                        ]
                    }
                }
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
    "@odata.type": "#microsoft.graph.searchResponse",
    "hitsContainers": [
        {
            "@odata.type": "#microsoft.graph.searchHitsContainer",
            "hits": [
                "..."
                    ],
            "total": 9,
            "moreResultsAvailable": false,
            "aggregations": [
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "Size",
                    "buckets": [
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "Less than 100",
                            "count": 0,
                            "aggregationFilterToken": "range(min, 100)"
                        },
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "100 up to 1000",
                            "count": 0,
                            "aggregationFilterToken": "range(100, 1000)"
                        },
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "1000 and up",
                            "count": 9,
                            "aggregationFilterToken": "range(1000, max, to=\"le\")"
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="known-limitations"></a>Limitações conhecidas

As agregaçãos são suportadas apenas para SharePoint ou OneDrive itens. Eles não têm suporte para mensagem **ou** **evento**.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
