---
title: Usar a API de Pesquisa da Microsoft para refinar consultas com agregações
description: Você pode usar a agregação da API de Pesquisa da Microsoft no Microsoft Graph para refinar os resultados da pesquisa e mostrar sua distribuição no índice.
author: nmoreau
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: c2bdb3121720a880bf2f508e7c43af2e53226dec
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443358"
---
# <a name="use-the-microsoft-search-api-to-refine-queries-with-aggregations"></a>Usar a API de Pesquisa da Microsoft para refinar consultas com agregações

Você pode usar a API de Pesquisa da Microsoft no Microsoft Graph para refinar os resultados da pesquisa e mostrar sua distribuição no índice.

Para refinar os resultados, na [solicitação de pesquisa](/graph/api/resources/searchRequest), especifique [a aggregationOption](/graph/api/resources/aggregationOption). Cada **aggregationOption** especifica a propriedade na qual a agregação deve ser computada e o número de [itens searchBucket](/graph/api/resources/searchBucket) a serem retornados na resposta.

## <a name="example-1-request-aggregations-by-string-fields"></a>Exemplo 1: Solicitar agregações por campos de cadeia de caracteres

O exemplo a seguir pesquisa recursos **listItem** e agrega resultados por seu tipo de arquivo, classe de conteúdo e hora da última modificação, todos eles são valores de cadeia de caracteres.

A resposta inclui dois [objetos searchBucket](/graph/api/resources/searchbucket) para as duas agregações:
- A **propriedade** de chave especifica o valor real (por `fileType`, `contentclass`ou `lastModifiedTime`) para os objetos **listItem** correspondentes que são agregados no mesmo bucket por esse valor.
- A **propriedade** count especifica o número desses objetos agregados no mesmo bucket. Observe que esse número é uma aproximação do número de correspondências e não fornecerá um número exato de correspondências.
- Buckets de resultados agregados por tipo de arquivo são classificados por contagem em ordem decrescente. Neste exemplo, há 3 buckets para três tipos de arquivo: `docx`, `xlsx`e `pptx`.
- Buckets de resultados agregados por classe de conteúdo são classificados pelo valor da cadeia de caracteres da classe de conteúdo em ordem decrescente. Neste exemplo, há apenas um bucket com todos os objetos correspondentes que compartilham a mesma classe de conteúdo. `STS_ListItem_DocumentLibrary`
- Buckets de resultados agregados por lastModifiedTime são classificados pelo valor de cadeia de caracteres de lastModifiedTime em ordem decrescente. Este exemplo inclui três buckets: `Before 2021-09-01T09:08:19.6224752Z`, `From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z`e `2021-11-09T09:08:19.6224752Z or later`.

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
              "field": "fileType",
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
          },
          {
              "field": "lastModifiedTime",
              "size": 2,
              "bucketDefinition": {
                  "sortBy": "KeyAsString",
                  "isDescending": "true",
                  "minimumCount": 0,
                  "ranges": [
                      {
                          "to": "2021-09-01T09:08:19.6224752Z"
                      },
                      {
                          "from": "2021-09-01T09:08:19.6224752Z",
                          "to": "2021-11-09T09:08:19.6224752Z"
                      },
                      {
                          "from": "2021-11-09T09:08:19.6224752Z"
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
                    "field": "fileType",
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
                },
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "lastModifiedTime",
                    "buckets": [
                        {
                            "key": "Before 2021-09-01T09:08:19.6224752Z",
                            "count": 5,
                            "aggregationFilterToken": "range(min, 2021-09-01T09:08:19.6224752Z)"
                        },
                        {
                            "key": "From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z",
                            "count": 3,
                            "aggregationFilterToken": "range(2021-09-01T09:08:19.6224752Z, 2021-11-09T09:08:19.6224752Z)"
                        },
                        {
                            "key": "2021-11-09T09:08:19.6224752Z or later",
                            "count": 1,
                            "aggregationFilterToken": "range(2021-11-09T09:08:19.6224752Z, max, to=\"le\")"
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a>Exemplo 2: Aplicar um filtro de agregação com base em uma solicitação anterior

Este exemplo aplica um filtro de agregação baseado na **agregaçãoFilterToken** `docx` `fileType` `From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z` `lastModifiedTime` retornada como o campo e como o campo no exemplo 1.

O valor da cadeia de caracteres atribuído à propriedade **aggregationFilters** segue o formato **"{field}:\\"{aggregationFilterToken}\\"**. Se vários valores para o mesmo filtro forem necessários, o valor da cadeia de caracteres atribuído à propriedade **aggregationFilters** deverá seguir este formato: **"{field}:or(\\"{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**.

O valor da cadeia de caracteres de formatação datetime atribuído à propriedade **aggregationFilters** segue o formato **"{field}:{aggregationFilterToken}"**.


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
              "field": "fileType",
              "size": 10,
              "bucketDefinition": {
                  "sortBy": "count",
                  "isDescending": "true",
                  "minimumCount": 0
              }
          }
      ],
      "aggregationFilters": [
        "fileType:\"ǂǂ68746d6c\"",
        "lastModifiedTime:range(2021-09-01T09:08:19.6224752Z, 2021-11-09T09:08:19.6224752Z)"
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
                    "field": "fileType",
                    "buckets": [
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "html",
                            "count": 69960,
                            "aggregationFilterToken": "\"ǂǂ68746d6c\""
                        }
                    ]
                },
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "lastModifiedTime",
                    "buckets": [
                        {
                            "key": "Before 2021-09-01T09:08:19.6224752Z",
                            "count": 0,
                            "aggregationFilterToken": "range(min, 2021-09-01T09:08:19.6224752Z)"
                        },
                        {
                            "key": "From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z",
                            "count": 69960,
                            "aggregationFilterToken": "range(2021-09-01T09:08:19.6224752Z, 2021-11-09T09:08:19.6224752Z)"
                        },
                        {
                            "key": "2021-11-09T09:08:19.6224752Z or later",
                            "count": 0,
                            "aggregationFilterToken": "range(2021-11-09T09:08:19.6224752Z, max, to=\"le\")"
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="example-3-request-aggregation-by-a-numeric-field"></a>Exemplo 3: Solicitar agregação por um campo numérico

O exemplo a seguir pesquisa **recursos driveItem** e agrega resultados por seu tamanho, que é um valor numérico. A solicitação especifica a agregação por três intervalos de tamanho:
- Tamanho menor que 100
- Tamanho entre 100 e 1000
- Tamanho 1000 e superior

A resposta inclui três objetos **searchBucket** , um para cada agregação de intervalo de tamanho:
- Os 2 buckets dos intervalos de tamanho inferior não incluem nenhuma correspondente de pesquisa.
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

As agregações têm suporte apenas para itens do SharePoint ou do OneDrive. Não há suporte para mensagens **ou** **eventos**.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview)
