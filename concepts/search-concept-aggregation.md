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
# <a name="refine-search-results-using-aggregations-preview"></a><span data-ttu-id="53e9f-103">Refinar resultados de pesquisa usando agregação (visualização)</span><span class="sxs-lookup"><span data-stu-id="53e9f-103">Refine search results using aggregations (preview)</span></span>

<span data-ttu-id="53e9f-104">Refine os resultados da pesquisa e mostre sua distribuição no índice.</span><span class="sxs-lookup"><span data-stu-id="53e9f-104">Refine search results and show their distribution in the index.</span></span>

## <a name="example-1-request-aggregations-by-string-fields"></a><span data-ttu-id="53e9f-105">Exemplo 1: Solicitar agregação por campos de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53e9f-105">Example 1: Request aggregations by string fields</span></span>

<span data-ttu-id="53e9f-106">O exemplo a seguir pesquisa **recursos listItem** e agrega resultados por seu tipo de arquivo e classe de conteúdo, ambos são valores de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="53e9f-106">The following example searches **listItem** resources and aggregates results by their file type and content class, both of which are string values.</span></span>

<span data-ttu-id="53e9f-107">A resposta inclui dois [objetos searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) para as duas agregação:</span><span class="sxs-lookup"><span data-stu-id="53e9f-107">The response includes two [searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) objects for the two aggregations:</span></span>
- <span data-ttu-id="53e9f-108">A **propriedade** de chave especifica o valor real (por ou ) para os objetos `FileType` `contentclass` **listItem** correspondentes que são agregados no mesmo bucket por esse valor.</span><span class="sxs-lookup"><span data-stu-id="53e9f-108">The **key** property specifies the actual value (by `FileType` or `contentclass`) for those matching **listItem** objects that are aggregated in the same bucket by that value.</span></span>
- <span data-ttu-id="53e9f-109">A **propriedade** count especifica o número de tais objetos agregados no mesmo bucket.</span><span class="sxs-lookup"><span data-stu-id="53e9f-109">The **count** property specifies the number of such objects aggregated in the same bucket.</span></span> <span data-ttu-id="53e9f-110">Observe que esse número é uma aproximação do número de combinações e não fornecerá um número exato de combinações.</span><span class="sxs-lookup"><span data-stu-id="53e9f-110">Note that this number is an approximation of the number of matches and will not provide an exact number of matches.</span></span>
- <span data-ttu-id="53e9f-111">Buckets de resultados agregados por tipo de arquivo são organizados por contagem em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="53e9f-111">Buckets of results aggregated by file type are sorted by count in descending order.</span></span> <span data-ttu-id="53e9f-112">Neste exemplo, há 3 buckets para 3 tipos de arquivo: `docx` `xlsx` e `pptx` .</span><span class="sxs-lookup"><span data-stu-id="53e9f-112">In this example, there are 3 buckets for 3 file types: `docx`, `xlsx`, and `pptx`.</span></span>
- <span data-ttu-id="53e9f-113">Buckets de resultados agregados por classe de conteúdo são organizados pelo valor da cadeia de caracteres da classe de conteúdo em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="53e9f-113">Buckets of results aggregated by content class are sorted by the string value of the content class in descending order.</span></span> <span data-ttu-id="53e9f-114">Neste exemplo, há apenas um bucket com todos os objetos correspondentes compartilhando a mesma classe de `STS_ListItem_DocumentLibrary` conteúdo.</span><span class="sxs-lookup"><span data-stu-id="53e9f-114">In this example, there is only one bucket with all the matching objects sharing the same content class, `STS_ListItem_DocumentLibrary`.</span></span>

### <a name="request"></a><span data-ttu-id="53e9f-115">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53e9f-115">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="53e9f-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="53e9f-116">Response</span></span>

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

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a><span data-ttu-id="53e9f-117">Exemplo 2: Aplicar um filtro de agregação com base em uma solicitação anterior</span><span class="sxs-lookup"><span data-stu-id="53e9f-117">Example 2: Apply an aggregation filter based on a previous request</span></span>

<span data-ttu-id="53e9f-118">Neste exemplo, aplicamos um filtro de agregação baseado no **aggregationFilterToken** retornado como o campo `docx` no exemplo `FileType` 1.</span><span class="sxs-lookup"><span data-stu-id="53e9f-118">In this example, we apply an aggregation filter that is based on the **aggregationFilterToken** returned for `docx` as the `FileType` field in example 1.</span></span>

<span data-ttu-id="53e9f-119">O valor da cadeia de caracteres atribuído à propriedade **aggregationFilters** segue o formato **"{field}: \\ "{aggregationFilterToken} \\ ""**.</span><span class="sxs-lookup"><span data-stu-id="53e9f-119">The string value assigned to the **aggregationFilters** property follows the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <span data-ttu-id="53e9f-120">Se vários valores para o mesmo filtro são necessários, o valor de cadeia de caracteres atribuído à propriedade **aggregationFilters** deve seguir este formato: **"{field}:or( \\ "{aggregationFilterToken1} \\ ", \\ "{aggregationFilterToken2} \\ ")"**.</span><span class="sxs-lookup"><span data-stu-id="53e9f-120">If multiple values for the same filter are required, the string value assigned to the **aggregationFilters** property should follow this format : **"{field}:or(\\"{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**.</span></span>

### <a name="request"></a><span data-ttu-id="53e9f-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53e9f-121">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="53e9f-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="53e9f-122">Response</span></span>

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

## <a name="example-3-request-aggregation-by-a-numeric-field"></a><span data-ttu-id="53e9f-123">Exemplo 3: Solicitar agregação por um campo numérico</span><span class="sxs-lookup"><span data-stu-id="53e9f-123">Example 3: Request aggregation by a numeric field</span></span>

<span data-ttu-id="53e9f-124">O exemplo a seguir pesquisa **recursos driveItem** e agrega resultados por seu tamanho, que é um valor numérico.</span><span class="sxs-lookup"><span data-stu-id="53e9f-124">The following example searches **driveItem** resources and aggregates results by their size which is a numeric value.</span></span> <span data-ttu-id="53e9f-125">A solicitação especifica a agregação por 3 intervalos de tamanho:</span><span class="sxs-lookup"><span data-stu-id="53e9f-125">The request specifies aggregation by 3 size ranges:</span></span>
- <span data-ttu-id="53e9f-126">Tamanho menor que 100</span><span class="sxs-lookup"><span data-stu-id="53e9f-126">Size less than 100</span></span>
- <span data-ttu-id="53e9f-127">Tamanho entre 100 e 1000</span><span class="sxs-lookup"><span data-stu-id="53e9f-127">Size between 100 and 1000</span></span>
- <span data-ttu-id="53e9f-128">Tamanho 1000 e superior</span><span class="sxs-lookup"><span data-stu-id="53e9f-128">Size 1000 and higher</span></span>

<span data-ttu-id="53e9f-129">A resposta inclui três **objetos searchBucket,** um para cada agregação de intervalo de tamanho:</span><span class="sxs-lookup"><span data-stu-id="53e9f-129">The response includes 3 **searchBucket** objects, one for each size range aggregation:</span></span>
- <span data-ttu-id="53e9f-130">Os 2 buckets dos intervalos de tamanho inferior não incluem nenhuma pesquisa coincidente.</span><span class="sxs-lookup"><span data-stu-id="53e9f-130">The 2 buckets of the lower size ranges don't include any search matches.</span></span>
- <span data-ttu-id="53e9f-131">Todas as 9 pesquisas têm tamanhos 1.000 ou superior.</span><span class="sxs-lookup"><span data-stu-id="53e9f-131">All 9 search matches have sizes 1000 or higher.</span></span>

### <a name="request"></a><span data-ttu-id="53e9f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53e9f-132">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="53e9f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="53e9f-133">Response</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="53e9f-134">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="53e9f-134">Known limitations</span></span>

<span data-ttu-id="53e9f-135">As agregação são suportadas apenas para itens do SharePoint ou do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="53e9f-135">Aggregations are supported only for SharePoint or OneDrive items.</span></span> <span data-ttu-id="53e9f-136">Não há suporte para mensagem **ou** **evento.**</span><span class="sxs-lookup"><span data-stu-id="53e9f-136">They are not supported for **message** or **event**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="53e9f-137">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="53e9f-137">Next steps</span></span>

- [<span data-ttu-id="53e9f-138">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="53e9f-138">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
