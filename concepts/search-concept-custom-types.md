---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para Pesquisar tipos personalizados
description: Você pode usar a API de pesquisa da Microsoft para importar dados externos por meio do recurso [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) e executar consultas de pesquisa nesse conteúdo externo.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: ba08eeb2aeaf4aa13e6b5bc686143e9b4293c0d8
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49523760"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors-preview"></a><span data-ttu-id="f0f59-103">Usar a API de pesquisa da Microsoft para Pesquisar tipos personalizados importados usando os conectores do Microsoft Graph (visualização)</span><span class="sxs-lookup"><span data-stu-id="f0f59-103">Use the Microsoft Search API to search custom types imported using Microsoft Graph connectors (preview)</span></span> 

<span data-ttu-id="f0f59-104">Use a API de pesquisa da Microsoft para pesquisar conteúdo ingerido e indexado pelos [conectores do Microsoft Graph](/microsoftsearch/connectors-overview).</span><span class="sxs-lookup"><span data-stu-id="f0f59-104">Use the Microsoft Search API to search accross content ingested and indexed by [Microsoft Graph connectors](/microsoftsearch/connectors-overview).</span></span> <span data-ttu-id="f0f59-105">O conteúdo é importado por meio de [conectores internos](/microsoftsearch/connectors-gallery) fornecidos pela Microsoft ou por meio de conectores personalizados implementados usando a [API de inclusão de conectores do Microsoft Graph](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="f0f59-105">The content is imported either via [built-in connectors](/microsoftsearch/connectors-gallery) provided by Microsoft, or via custom connectors implemented using the [Microsoft Graph connectors ingestion API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="f0f59-106">Após o conteúdo ter sido importado e indexado, você poderá usar a API de pesquisa para consultar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f0f59-106">Once the content has been imported and indexed, you can use the search API to query the content.</span></span>

<span data-ttu-id="f0f59-107">Para Pesquisar tipos personalizados, especifique as propriedades a seguir no corpo da solicitação do método de [consulta](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) :</span><span class="sxs-lookup"><span data-stu-id="f0f59-107">To search for custom types, specify the following properties in the request body of the [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) method:</span></span>

- <span data-ttu-id="f0f59-108">A propriedade **ContentSources** para incluir a ID de conexão atribuída durante a configuração do conector.</span><span class="sxs-lookup"><span data-stu-id="f0f59-108">The **contentSources** property to include the connection ID that is assigned during the connector setup.</span></span> <span data-ttu-id="f0f59-109">Você pode passar várias IDs de conexão para pesquisar em várias conexões.</span><span class="sxs-lookup"><span data-stu-id="f0f59-109">You can pass multiple connection IDs to search across multiple connections.</span></span> <span data-ttu-id="f0f59-110">Os resultados são retornados em uma única lista, classificados por várias conexões.</span><span class="sxs-lookup"><span data-stu-id="f0f59-110">Results are returned in a single list, ranked accross the multiple connections.</span></span>

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- <span data-ttu-id="f0f59-111">A propriedade **EntityTypes** como `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="f0f59-111">The **entityTypes** property as `externalItem`.</span></span>

- <span data-ttu-id="f0f59-112">A propriedade **Fields** para incluir os campos no item externo a serem recuperados.</span><span class="sxs-lookup"><span data-stu-id="f0f59-112">The **fields** property to include the fields in the external item to retrieve.</span></span> <span data-ttu-id="f0f59-113">Observe que, se você não incluir nenhum **campo** na solicitação, a resposta conterá todos os campos marcados como *recuperáveis* no esquema de dados especificado para as conexões especificadas na propriedade **ContentSources** .</span><span class="sxs-lookup"><span data-stu-id="f0f59-113">Note that if you do not include any **fields** in the request, the response will contain all the fields marked as *retrievable* in the data schema specified for the specified connections in the **contentSources** property.</span></span>

<span data-ttu-id="f0f59-114">Além disso, você pode agregar resultados de pesquisa com base nas propriedades de um [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) que são numéricos ou de cadeia de caracteres, e que estão definidos como refinável no [esquema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="f0f59-114">In addition, you can aggregate search results based on properties in an [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) that are numeric or string type, and that are set to be refinable in the [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="f0f59-115">Para obter mais informações, consulte [refinar resultados de pesquisa usando agregações](search-concept-aggregation.md).</span><span class="sxs-lookup"><span data-stu-id="f0f59-115">For more information, see [Refine search results using aggregations](search-concept-aggregation.md).</span></span>

## <a name="example"></a><span data-ttu-id="f0f59-116">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0f59-116">Example</span></span>

<span data-ttu-id="f0f59-117">Neste exemplo, o conteúdo do banco de dados [AdventureWorks](/sql/samples/adventureworks-install-configure) foi incluído usando o conector interno do Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="f0f59-117">In this example, the content of the [AdventureWorks](/sql/samples/adventureworks-install-configure) database has been ingested using the Azure SQL built-in connector.</span></span>

### <a name="request"></a><span data-ttu-id="f0f59-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0f59-118">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="f0f59-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0f59-119">Response</span></span>

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

## <a name="next-steps"></a><span data-ttu-id="f0f59-120">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f0f59-120">Next steps</span></span>

- [<span data-ttu-id="f0f59-121">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="f0f59-121">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)