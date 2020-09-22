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
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors"></a><span data-ttu-id="7bc50-103">Usar a API de pesquisa da Microsoft para Pesquisar tipos personalizados importados usando conectores do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7bc50-103">Use the Microsoft Search API to search custom types imported using Microsoft Graph connectors</span></span>

<span data-ttu-id="7bc50-104">Use a API de pesquisa da Microsoft para pesquisar conteúdo ingerido e indexado pelos [conectores do Microsoft Graph](https://docs.microsoft.com/microsoftsearch/connectors-overview).</span><span class="sxs-lookup"><span data-stu-id="7bc50-104">Use the Microsoft Search API to search accross content ingested and indexed by [Microsoft Graph connectors](https://docs.microsoft.com/microsoftsearch/connectors-overview).</span></span> <span data-ttu-id="7bc50-105">O conteúdo é importado por meio de [conectores internos](https://docs.microsoft.com/microsoftsearch/connectors-gallery) fornecidos pela Microsoft ou por meio de conectores personalizados implementados usando a [API de inclusão de conectores do Microsoft Graph](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="7bc50-105">The content is imported either via [built-in connectors](https://docs.microsoft.com/microsoftsearch/connectors-gallery) provided by Microsoft, or via custom connectors implemented using the [Microsoft Graph connectors ingestion API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="7bc50-106">Após o conteúdo ter sido importado e indexado, você poderá usar a API de pesquisa para consultar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7bc50-106">Once the content has been imported and indexed, you can use the search API to query the content.</span></span>

<span data-ttu-id="7bc50-107">Para Pesquisar tipos personalizados, especifique as propriedades a seguir no corpo da solicitação do método de [consulta](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) :</span><span class="sxs-lookup"><span data-stu-id="7bc50-107">To search for custom types, specify the following properties in the request body of the [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) method:</span></span>

- <span data-ttu-id="7bc50-108">A propriedade **ContentSources** para incluir a ID de conexão atribuída durante a configuração do conector.</span><span class="sxs-lookup"><span data-stu-id="7bc50-108">The **contentSources** property to include the connection ID that is assigned during the connector setup.</span></span> <span data-ttu-id="7bc50-109">Você pode passar várias IDs de conexão para pesquisar em várias conexões.</span><span class="sxs-lookup"><span data-stu-id="7bc50-109">You can pass multiple connection IDs to search across multiple connections.</span></span> <span data-ttu-id="7bc50-110">Os resultados são retornados em uma única lista, classificados por várias conexões.</span><span class="sxs-lookup"><span data-stu-id="7bc50-110">Results are returned in a single list, ranked accross the multiple connections.</span></span>

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- <span data-ttu-id="7bc50-111">A propriedade **EntityTypes** como `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="7bc50-111">The **entityTypes** property as `externalItem`.</span></span>

- <span data-ttu-id="7bc50-112">A propriedade **Fields** para incluir os campos no item externo a serem recuperados.</span><span class="sxs-lookup"><span data-stu-id="7bc50-112">The **fields** property to include the fields in the external item to retrieve.</span></span>

## <a name="example"></a><span data-ttu-id="7bc50-113">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bc50-113">Example</span></span>

<span data-ttu-id="7bc50-114">Neste exemplo, o conteúdo do banco de dados [AdventureWorks](https://docs.microsoft.com/sql/samples/adventureworks-install-configure) foi incluído usando o conector interno do Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="7bc50-114">In this example, the content of the [AdventureWorks](https://docs.microsoft.com/sql/samples/adventureworks-install-configure) database has been ingested using the Azure SQL built-in connector.</span></span>

### <a name="request"></a><span data-ttu-id="7bc50-115">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc50-115">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="7bc50-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bc50-116">Response</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="7bc50-117">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="7bc50-117">Known limitations</span></span>

- <span data-ttu-id="7bc50-118">Você deve especificar a propriedade **Fields** para obter campos recuperáveis no esquema de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7bc50-118">You must specify the **fields** property to get retrievable fields in the search schema.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7bc50-119">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="7bc50-119">Next steps</span></span>

- [<span data-ttu-id="7bc50-120">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="7bc50-120">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
