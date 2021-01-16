---
title: Usar a API de Pesquisa da Microsoft no Microsoft Graph refinar consultas com agregação
description: Você pode usar a API de Pesquisa da Microsoft para recuperar agregações
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: fad049649172750cf2e362d2558cfc247467a6ed
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883190"
---
# <a name="refine-search-results-using-aggregations-preview"></a>Refinar resultados de pesquisa usando agregação (visualização)

Refine os resultados da pesquisa e mostre sua distribuição no índice.

## <a name="example-1-request-aggregations-by-string-fields"></a>Exemplo 1: Solicitar agregação por campos de cadeia de caracteres

O exemplo a seguir pesquisa **recursos listItem** e agrega resultados por seu tipo de arquivo e classe de conteúdo, ambos são valores de cadeia de caracteres.

A resposta inclui dois [objetos searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) para as duas agregação:
- A **propriedade** de chave especifica o valor real (por ou ) para os objetos `FileType` `contentclass` **listItem** correspondentes que são agregados no mesmo bucket por esse valor.
- A **propriedade** count especifica o número de tais objetos agregados no mesmo bucket. Observe que esse número é uma aproximação do número de combinações e não fornecerá um número exato de combinações.
- Buckets de resultados agregados por tipo de arquivo são organizados por contagem em ordem decrescente. Neste exemplo, há 3 buckets para 3 tipos de arquivo: `docx` `xlsx` e `pptx` .
- Buckets de resultados agregados por classe de conteúdo são organizados pelo valor da cadeia de caracteres da classe de conteúdo em ordem decrescente. Neste exemplo, há apenas um bucket com todos os objetos correspondentes compartilhando a mesma classe de `STS_ListItem_DocumentLibrary` conteúdo.

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

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a>Exemplo 2: Aplicar um filtro de agregação com base em uma solicitação anterior

Neste exemplo, aplicamos um filtro de agregação baseado no **aggregationFilterToken** retornado como o campo `docx` no exemplo `FileType` 1.

O valor da cadeia de caracteres atribuído à propriedade **aggregationFilters** segue o formato **"{field}: \\ "{aggregationFilterToken} \\ ""**. Se vários valores para o mesmo filtro são necessários, o valor de cadeia de caracteres atribuído à propriedade **aggregationFilters** deve seguir este formato: **"{field}:or( \\ "{aggregationFilterToken1} \\ ", \\ "{aggregationFilterToken2} \\ ")"**.

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

O exemplo a seguir pesquisa **recursos driveItem** e agrega resultados por seu tamanho, que é um valor numérico. A solicitação especifica a agregação por 3 intervalos de tamanho:
- Tamanho menor que 100
- Tamanho entre 100 e 1000
- Tamanho 1000 e superior

A resposta inclui três **objetos searchBucket,** um para cada agregação de intervalo de tamanho:
- Os 2 buckets dos intervalos de tamanho inferior não incluem nenhuma pesquisa coincidente.
- Todas as 9 pesquisas têm tamanhos 1.000 ou superior.

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

As agregação são suportadas apenas para itens do SharePoint ou do OneDrive. Não há suporte para mensagem **ou** **evento.**

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
