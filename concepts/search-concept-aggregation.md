---
title: Usar a API do Microsoft Search no Microsoft Graph para refinar consultas com agregações
description: Você pode usar a API de pesquisa da Microsoft para recuperar o aggreations
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: b414c0beb26280ef90d0a6bd5c807ee9904a5a7e
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193670"
---
# <a name="refine-search-results-using-aggregations"></a>Refinar os resultados da pesquisa usando agregações

Refine os resultados da pesquisa e mostrar sua distribuição no índice. 

## <a name="example-1-request-aggregations-by-string-fields"></a>Exemplo 1: solicitar agregações por campos de cadeia de caracteres

O exemplo a seguir pesquisa os recursos **ListItems** e agregados resultados por seus tipos de arquivo e classe de conteúdo, ambos os valores de cadeia de caracteres.

A resposta inclui dois objetos [searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) para as duas agregações:
- A propriedade **Key** especifica o valor real (por `FileType` ou `contentclass` ) para aqueles objetos **ListItem** que são agregados no mesmo Bucket por esse valor.
- A propriedade **Count** especifica o número desses objetos agregados no mesmo Bucket.
- Os buckets de resultados agregados por tipo de arquivo são classificados por contagem em ordem decrescente. Neste exemplo, há 3 buckets para 3 tipos de arquivo: `docx` , `xlsx` e `pptx` .
- Os buckets de resultados agregados pela classe de conteúdo são classificados pelo valor da cadeia de caracteres da classe de conteúdo em ordem decrescente. Neste exemplo, há apenas um Bucket com todos os objetos correspondentes que compartilham a mesma classe de conteúdo `STS_ListItem_DocumentLibrary` .

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

Neste exemplo, aplicamos um filtro de agregação baseado no **aggregationFilterToken** retornado `docx` como o `FileType` campo no exemplo 1.

O valor da cadeia de caracteres atribuída à propriedade **aggregationFilters** segue o formato **"{Field}: \\ " {aggregationFilterToken} \\ ""**.

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

## <a name="example-3-request-aggregation-by-a-numeric-field"></a>Exemplo 3: solicitar a agregação por um campo numérico

O exemplo a seguir pesquisa os recursos **driveItem** e agrega os resultados pelo tamanho que é um valor numérico. A solicitação especifica a agregação em intervalos de tamanho de 3:
- Tamanho menor que 100
- Tamanho entre 100 e 1000
- Tamanho 1000 e superior

A resposta inclui 3 objetos **searchBucket** , um para cada agregação de intervalo de tamanho:
- Os 2 buckets dos intervalos de tamanho inferior não incluem nenhuma correspondência de pesquisa.
- Todas as nove correspondências de pesquisa têm tamanhos 1000 ou superior.

### <a name="request"></a>Solicitação

```HTTP
POST /search/query
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

As agregações são suportadas apenas para itens do SharePoint ou do OneDrive. Eles não têm suporte para **Message**, **Event**e **externalItem**.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
