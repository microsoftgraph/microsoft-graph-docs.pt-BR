---
title: Use a API de Pesquisa da Microsoft no Microsoft Graph pesquisar tipos personalizados
description: Você pode usar a API de Pesquisa da Microsoft para importar dados externos por meio do [recurso externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) e executar consultas de pesquisa nesse conteúdo externo.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: cc75530533ef8613f416e7fabc03904b2f7940ec
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703598"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors-preview"></a><span data-ttu-id="57e5a-103">Use a API de Pesquisa da Microsoft para pesquisar tipos personalizados importados usando conectores Graph Microsoft (visualização)</span><span class="sxs-lookup"><span data-stu-id="57e5a-103">Use the Microsoft Search API to search custom types imported using Microsoft Graph connectors (preview)</span></span> 

<span data-ttu-id="57e5a-104">Use a API de Pesquisa da Microsoft para pesquisar o conteúdo ingerido e indexado pelos conectores [Graph Microsoft.](/microsoftsearch/connectors-overview)</span><span class="sxs-lookup"><span data-stu-id="57e5a-104">Use the Microsoft Search API to search accross content ingested and indexed by [Microsoft Graph connectors](/microsoftsearch/connectors-overview).</span></span> <span data-ttu-id="57e5a-105">O conteúdo é importado por meio de conectores [integrados fornecidos](/microsoftsearch/connectors-gallery) pela Microsoft ou por meio de conectores personalizados implementados usando a API de ingestão de conectores do [Microsoft Graph](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="57e5a-105">The content is imported either via [built-in connectors](/microsoftsearch/connectors-gallery) provided by Microsoft, or via custom connectors implemented using the [Microsoft Graph connectors ingestion API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="57e5a-106">Depois que o conteúdo tiver sido importado e indexado, você poderá usar a API de pesquisa para consultar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="57e5a-106">Once the content has been imported and indexed, you can use the search API to query the content.</span></span>

<span data-ttu-id="57e5a-107">Para pesquisar tipos personalizados, especifique as seguintes propriedades no corpo da solicitação do [método de](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) consulta:</span><span class="sxs-lookup"><span data-stu-id="57e5a-107">To search for custom types, specify the following properties in the request body of the [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) method:</span></span>

- <span data-ttu-id="57e5a-108">A **propriedade contentSources** para incluir a ID de conexão atribuída durante a instalação do conector.</span><span class="sxs-lookup"><span data-stu-id="57e5a-108">The **contentSources** property to include the connection ID that is assigned during the connector setup.</span></span> <span data-ttu-id="57e5a-109">Você pode passar várias IDs de conexão para pesquisar em várias conexões.</span><span class="sxs-lookup"><span data-stu-id="57e5a-109">You can pass multiple connection IDs to search across multiple connections.</span></span> <span data-ttu-id="57e5a-110">Os resultados são retornados em uma única lista, classificada entre as várias conexões.</span><span class="sxs-lookup"><span data-stu-id="57e5a-110">Results are returned in a single list, ranked accross the multiple connections.</span></span>

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- <span data-ttu-id="57e5a-111">A **propriedade entityTypes** como `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="57e5a-111">The **entityTypes** property as `externalItem`.</span></span>

- <span data-ttu-id="57e5a-112">A **propriedade fields** para incluir os campos no item externo a ser recuperado.</span><span class="sxs-lookup"><span data-stu-id="57e5a-112">The **fields** property to include the fields in the external item to retrieve.</span></span> <span data-ttu-id="57e5a-113">Observe que, se você  não incluir nenhum campo na solicitação, a resposta conterá todos os campos marcados como *recuperáveis* no esquema de dados especificado para as conexões especificadas na propriedade **contentSources.**</span><span class="sxs-lookup"><span data-stu-id="57e5a-113">Note that if you do not include any **fields** in the request, the response will contain all the fields marked as *retrievable* in the data schema specified for the specified connections in the **contentSources** property.</span></span>

<span data-ttu-id="57e5a-114">Além disso, você pode agregar resultados de pesquisa com base em propriedades em [um externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) que são numéricos ou tipo de cadeia de caracteres e que são definidos como refináveis no [esquema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="57e5a-114">In addition, you can aggregate search results based on properties in an [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) that are numeric or string type, and that are set to be refinable in the [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="57e5a-115">Para obter mais informações, [consulte Refinar resultados de pesquisa usando agregação .](search-concept-aggregation.md)</span><span class="sxs-lookup"><span data-stu-id="57e5a-115">For more information, see [Refine search results using aggregations](search-concept-aggregation.md).</span></span>

## <a name="example-1-retrieve-items-using-azure-sql-built-in-connector"></a><span data-ttu-id="57e5a-116">Exemplo 1: Recuperar itens usando o Azure SQL conector integrado</span><span class="sxs-lookup"><span data-stu-id="57e5a-116">Example 1: Retrieve items using Azure SQL built-in connector</span></span>

<span data-ttu-id="57e5a-117">Neste exemplo, o conteúdo do banco de dados [AdventureWorks](/sql/samples/adventureworks-install-configure) foi ingerido usando o conector SQL Azure integrado.</span><span class="sxs-lookup"><span data-stu-id="57e5a-117">In this example, the content of the [AdventureWorks](/sql/samples/adventureworks-install-configure) database has been ingested using the Azure SQL built-in connector.</span></span>

### <a name="request"></a><span data-ttu-id="57e5a-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57e5a-118">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="57e5a-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="57e5a-119">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
  "value": [
    {
      "searchTerms": ["yang"],
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
                  "shortDescription": "Contoso maintenance guidelines",
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

## <a name="example-2-retrieve-items-using-semantic-labels"></a><span data-ttu-id="57e5a-120">Exemplo 2: Recuperar itens usando rótulos semânticos</span><span class="sxs-lookup"><span data-stu-id="57e5a-120">Example 2: Retrieve items using semantic labels</span></span>

### <a name="request"></a><span data-ttu-id="57e5a-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57e5a-121">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
      {
        "entityTypes": [
          "microsoft.graph.externalItem"
        ],
        "contentSources": [
          "/external/connections/FileAsUdt"
        ],
        "query": {
          "query_string": {
            "query": "test"
          }
        },
        "stored_fields": [
          "label_Title",
          "label_URL",
          "label_LastModifiedBy",
          "label_LastModifiedDateTime"
        ],
        "from": 0,
        "size": 25
      }
    ]
}
```

### <a name="response"></a><span data-ttu-id="57e5a-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="57e5a-122">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
"value": [
      {
        "searchTerms": [
          "test"
        ],
        "hitsContainers": [
          {
            "hits": [
              {
                "_id": "AQMkAGRjZWJjZTFkLTkzYWItNDhlOC1iODA2LTgwMTNjNjEzYzI2YwBGAAADOx0/YV2JckefuDmJtUO7mwcAHNjGq33S50uXSFeU/U9mogAAAgEWAAAAHNjGq33S50uXSFeU/U9mogAAAgleAAAA",
                "_contentSource": "FileAsUdt",
                "_score": 1,
                "_summary": "<c0>Test</c0> component to move data files and messages between the gateway and internal <ddd/>",
                "_source": {
                  "@odata.type": "#microsoft.graph.externalItem",
                  "properties": {
                    "label_Title": "SONIC Operations support and test Guide for the month of March",
                    "label_URL": "D:\\\\ConnectorsEcho\\\\New\\\\MSW06SecondSet\\\\teams\\\\Enterprise_Platforms\\\\CCO\\\\Projects\\\\BTSi Modernization\\\\SONIC Retirement\\\\SONIC_Operations_Support_Guide.docx",
                    "label_LastModifiedBy": [
                      "Bob",
                      "Scott"
                    ],
                    "label_LastModifiedDateTime": "2020-01-30T12:44:19Z"
                  }
                }
              },
              {
                "_id": "AQMkAGRjZWJjZTFkLTkzYWItNDhlOC1iODA2LTgwMTNjNjEzYzI2YwBGAAADOx0/YV2JckefuDmJtUO7mwcAHNjGq33S50uXSFeU/U9mogAAAgEWAAAAHNjGq33S50uXSFeU/U9mogAAAgldAAAA",
                "_contentSource": "FileAsUdt",
                "_score": 2,
                "_summary": "File Transfer Workbench A <c0>test</c0> File transfer Management Solution File Transfer the number <ddd/>",
                "_source": {
                  "@odata.type": "#microsoft.graph.externalItem",
                  "properties": {
                    "label_Title": "Test File Transfer Workbench for the month of January",
                    "label_URL": "D:\\\\ConnectorsEcho\\\\New\\\\MSW06SecondSet\\\\teams\\\\IssueLog\\\\FCAGA Organisation\\\\NSN CO CCA Infra YBCFTPAR entry\\\\File Transfer Workbench.ppt",
                    "label_LastModifiedBy": [
                      "Alice",
                      "Scott"
                    ],
                    "label_LastModifiedDateTime": "2020-01-31T11:44:19Z"
                  }
                }
              },
              {
                "_id": "AQMkAGRjZWJjZTFkLTkzYWItNDhlOC1iODA2LTgwMTNjNjEzYzI2YwBGAAADOx0/YV2JckefuDmJtUO7mwcAHNjGq33S50uXSFeU/U9mogAAAgEWAAAAHNjGq33S50uXSFeU/U9mogAAAglgAAAA",
                "_contentSource": "FileAsUdt",
                "_score": 3,
                "_summary": "document and the associated <c0>test</c0> software are the sole property of Express Logic.<ddd/>",
                "_source": {
                  "@odata.type": "#microsoft.graph.externalItem",
                  "properties": {
                    "label_Title": "System User Guide Express Logic 858.613.6640",
                    "label_URL": "D:\\\\ConnectorsEcho\\\\New\\\\MSW06FirstSet\\\\teams\\\\AzureIoTMarketing\\\\Shared Documents\\\\Whitepapers\\\\RTOS Whitepapers\\\\User Guides\\\\Azure_RTOS_FileX_User_Guide.pdf",
                    "label_LastModifiedBy": [
                      "Alice",
                      "Bob"
                    ],
                    "label_LastModifiedDateTime": "2020-05-25T10:20:19Z"
                  }
                }
              }
            ],
            "total": 3,
            "moreResultsAvailable": false
          }
        ]
      }
    ]
}
```

<span data-ttu-id="57e5a-123">Para obter mais detalhes, consulte [Atribuir rótulos de propriedade](/microsoftsearch/configure-connector#step-5-assign-property-labels).</span><span class="sxs-lookup"><span data-stu-id="57e5a-123">For more details, see [Assign property labels](/microsoftsearch/configure-connector#step-5-assign-property-labels).</span></span>

## <a name="next-steps"></a><span data-ttu-id="57e5a-124">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="57e5a-124">Next steps</span></span>

- [<span data-ttu-id="57e5a-125">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="57e5a-125">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
