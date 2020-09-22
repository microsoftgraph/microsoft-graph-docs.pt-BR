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
# <a name="refine-search-results-using-aggregations"></a><span data-ttu-id="6e515-103">Refinar os resultados da pesquisa usando agregações</span><span class="sxs-lookup"><span data-stu-id="6e515-103">Refine search results using aggregations</span></span>

<span data-ttu-id="6e515-104">Refine os resultados da pesquisa e mostrar sua distribuição no índice.</span><span class="sxs-lookup"><span data-stu-id="6e515-104">Refine search results and show their distribution in the index.</span></span> 

## <a name="example-1-request-aggregations-by-string-fields"></a><span data-ttu-id="6e515-105">Exemplo 1: solicitar agregações por campos de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e515-105">Example 1: Request aggregations by string fields</span></span>

<span data-ttu-id="6e515-106">O exemplo a seguir pesquisa os recursos **ListItems** e agregados resultados por seus tipos de arquivo e classe de conteúdo, ambos os valores de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="6e515-106">The following example searches **listItem** resources and aggregates results by their file type and content class, both of which are string values.</span></span>

<span data-ttu-id="6e515-107">A resposta inclui dois objetos [searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) para as duas agregações:</span><span class="sxs-lookup"><span data-stu-id="6e515-107">The response includes two [searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) objects for the two aggregations:</span></span>
- <span data-ttu-id="6e515-108">A propriedade **Key** especifica o valor real (por `FileType` ou `contentclass` ) para aqueles objetos **ListItem** que são agregados no mesmo Bucket por esse valor.</span><span class="sxs-lookup"><span data-stu-id="6e515-108">The **key** property specifies the actual value (by `FileType` or `contentclass`) for those matching **listItem** objects that are aggregated in the same bucket by that value.</span></span>
- <span data-ttu-id="6e515-109">A propriedade **Count** especifica o número desses objetos agregados no mesmo Bucket.</span><span class="sxs-lookup"><span data-stu-id="6e515-109">The **count** property specifies the number of such objects aggregated in the same bucket.</span></span>
- <span data-ttu-id="6e515-110">Os buckets de resultados agregados por tipo de arquivo são classificados por contagem em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="6e515-110">Buckets of results aggregated by file type are sorted by count in descending order.</span></span> <span data-ttu-id="6e515-111">Neste exemplo, há 3 buckets para 3 tipos de arquivo: `docx` , `xlsx` e `pptx` .</span><span class="sxs-lookup"><span data-stu-id="6e515-111">In this example, there are 3 buckets for 3 file types: `docx`, `xlsx`, and `pptx`.</span></span>
- <span data-ttu-id="6e515-112">Os buckets de resultados agregados pela classe de conteúdo são classificados pelo valor da cadeia de caracteres da classe de conteúdo em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="6e515-112">Buckets of results aggregated by content class are sorted by the string value of the content class in descending order.</span></span> <span data-ttu-id="6e515-113">Neste exemplo, há apenas um Bucket com todos os objetos correspondentes que compartilham a mesma classe de conteúdo `STS_ListItem_DocumentLibrary` .</span><span class="sxs-lookup"><span data-stu-id="6e515-113">In this example, there is only one bucket with all the matching objects sharing the same content class, `STS_ListItem_DocumentLibrary`.</span></span>

### <a name="request"></a><span data-ttu-id="6e515-114">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e515-114">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="6e515-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e515-115">Response</span></span>

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

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a><span data-ttu-id="6e515-116">Exemplo 2: aplicar um filtro de agregação com base em uma solicitação anterior</span><span class="sxs-lookup"><span data-stu-id="6e515-116">Example 2: Apply an aggregation filter based on a previous request</span></span>

<span data-ttu-id="6e515-117">Neste exemplo, aplicamos um filtro de agregação baseado no **aggregationFilterToken** retornado `docx` como o `FileType` campo no exemplo 1.</span><span class="sxs-lookup"><span data-stu-id="6e515-117">In this example, we apply an aggregation filter that is based on the **aggregationFilterToken** returned for `docx` as the `FileType` field in example 1.</span></span>

<span data-ttu-id="6e515-118">O valor da cadeia de caracteres atribuída à propriedade **aggregationFilters** segue o formato **"{Field}: \\ " {aggregationFilterToken} \\ ""**.</span><span class="sxs-lookup"><span data-stu-id="6e515-118">The string value assigned to the **aggregationFilters** property follows the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span>

### <a name="request"></a><span data-ttu-id="6e515-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e515-119">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="6e515-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e515-120">Response</span></span>

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

## <a name="example-3-request-aggregation-by-a-numeric-field"></a><span data-ttu-id="6e515-121">Exemplo 3: solicitar a agregação por um campo numérico</span><span class="sxs-lookup"><span data-stu-id="6e515-121">Example 3: Request aggregation by a numeric field</span></span>

<span data-ttu-id="6e515-122">O exemplo a seguir pesquisa os recursos **driveItem** e agrega os resultados pelo tamanho que é um valor numérico.</span><span class="sxs-lookup"><span data-stu-id="6e515-122">The following example searches **driveItem** resources and aggregates results by their size which is a numeric value.</span></span> <span data-ttu-id="6e515-123">A solicitação especifica a agregação em intervalos de tamanho de 3:</span><span class="sxs-lookup"><span data-stu-id="6e515-123">The request specifies aggregation by 3 size ranges:</span></span>
- <span data-ttu-id="6e515-124">Tamanho menor que 100</span><span class="sxs-lookup"><span data-stu-id="6e515-124">Size less than 100</span></span>
- <span data-ttu-id="6e515-125">Tamanho entre 100 e 1000</span><span class="sxs-lookup"><span data-stu-id="6e515-125">Size between 100 and 1000</span></span>
- <span data-ttu-id="6e515-126">Tamanho 1000 e superior</span><span class="sxs-lookup"><span data-stu-id="6e515-126">Size 1000 and higher</span></span>

<span data-ttu-id="6e515-127">A resposta inclui 3 objetos **searchBucket** , um para cada agregação de intervalo de tamanho:</span><span class="sxs-lookup"><span data-stu-id="6e515-127">The response includes 3 **searchBucket** objects, one for each size range aggregation:</span></span>
- <span data-ttu-id="6e515-128">Os 2 buckets dos intervalos de tamanho inferior não incluem nenhuma correspondência de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6e515-128">The 2 buckets of the lower size ranges don't include any search matches.</span></span>
- <span data-ttu-id="6e515-129">Todas as nove correspondências de pesquisa têm tamanhos 1000 ou superior.</span><span class="sxs-lookup"><span data-stu-id="6e515-129">All 9 search matches have sizes 1000 or higher.</span></span>

### <a name="request"></a><span data-ttu-id="6e515-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e515-130">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="6e515-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e515-131">Response</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="6e515-132">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="6e515-132">Known limitations</span></span>

<span data-ttu-id="6e515-133">As agregações são suportadas apenas para itens do SharePoint ou do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6e515-133">Aggregations are supported only for SharePoint or OneDrive items.</span></span> <span data-ttu-id="6e515-134">Eles não têm suporte para **Message**, **Event**e **externalItem**.</span><span class="sxs-lookup"><span data-stu-id="6e515-134">They are not supported for **message**, **event**, and **externalItem**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6e515-135">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="6e515-135">Next steps</span></span>

- [<span data-ttu-id="6e515-136">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="6e515-136">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
