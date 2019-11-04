---
title: Tipos personalizados de pesquisa
description: A API de consulta permite pesquisar entre tipos personalizados ingeridos por meio da API de indexação.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: d4381529d66eaae19d9866eeb594201cec115735
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939562"
---
# <a name="search-custom-types-externalitem"></a><span data-ttu-id="3d1ae-103">Tipos personalizados de pesquisa (externalItem)</span><span class="sxs-lookup"><span data-stu-id="3d1ae-103">Search custom types (externalItem)</span></span>

<span data-ttu-id="3d1ae-104">A API do Microsoft Search permite que você importe dados externos por meio do recurso [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) e execute consultas de pesquisa nesse conteúdo externo.</span><span class="sxs-lookup"><span data-stu-id="3d1ae-104">The Microsoft Search API lets you import external data via the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) resource, and run search queries on this external content.</span></span>

<span data-ttu-id="3d1ae-105">Para Pesquisar tipos personalizados, especifique o seguinte no corpo da solicitação do método de [consulta](/graph/api/search-query?view=graph-rest-beta) :</span><span class="sxs-lookup"><span data-stu-id="3d1ae-105">To search for custom types, specify the following in the [query](/graph/api/search-query?view=graph-rest-beta) method request body:</span></span>

- <span data-ttu-id="3d1ae-106">A propriedade **ContentSources** para incluir a ID de conexão atribuída durante a configuração do conector</span><span class="sxs-lookup"><span data-stu-id="3d1ae-106">The **contentSources** property to include the connection ID which is assigned during the connector setup</span></span>

- <span data-ttu-id="3d1ae-107">A propriedade **EntityType** como`externalItem`</span><span class="sxs-lookup"><span data-stu-id="3d1ae-107">The **entityType** property as `externalItem`</span></span>

- <span data-ttu-id="3d1ae-108">A propriedade **stored_fields** para incluir os campos no item externo que você deseja recuperar</span><span class="sxs-lookup"><span data-stu-id="3d1ae-108">The **stored_fields** property to include the fields in the external item you want to retrieve</span></span>

## <a name="example"></a><span data-ttu-id="3d1ae-109">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d1ae-109">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d1ae-110">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d1ae-110">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.externalItem"],
       "contentSources": ["/external/connections/servicenow-connector-contoso"],
       "query": {
        "query_string": {
          "query": "contoso tickets"
        }
      },
      "from": 0,
      "size": 25,
    "stored_fields": [
        "title",
        "priority",
        "description"
       ]
    }
  ]
}
```
### <a name="response"></a><span data-ttu-id="3d1ae-111">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d1ae-111">Response</span></span>

<span data-ttu-id="3d1ae-112">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d1ae-112">Response</span></span>

```Json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "hitsContainers": [
                {
                    "total": 2,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "_id": "AAMkADc0NDNlNTE0",
                            "_score": 1,
                            "_sortField": "Relevance",
                            "_source": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "properties": {
                                    "number": "KB0010025",
                                    "shortdescription": "Contoso maintenance guidelines",
                                    "syscreatedon": "2019-10-14T22:45:02Z",
                                    "accessurl": "https://contoso.service-now.com/kb_view.do?sys_kb_id=6b5465781ba000104793877ddc4bcb81",
                                    "previewContent": "Contoso maintenance guidelines"
                                }
                            }
                        },
                        {
                            "_id": "MG+1glPAAAAAAl3AAA=",
                            "_score": 2,
                            "_sortField": "Relevance",
                            "_source": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "properties": {
                                    "number": "KB0054396",
                                    "shortdescription": "Contoso : Setting Office for the first time.",
                                    "syscreatedon": "2019-08-09T01:53:26Z",
                                    "accessurl": "https://contoso.service-now.com/kb_view.do?sys_kb_id=004d8d931b0733004793877ddc4bcb29",
                                    "previewContent": "Description:  Setting Office for the first time.  Resolution:    To setup any Office app for the first time, tap any Office app like Word to launch it.    Tap Sign in if you already have a Microsoft Account or an Office 365 work or school account."
                                }
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```


## <a name="known-limitations"></a><span data-ttu-id="3d1ae-113">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="3d1ae-113">Known limitations</span></span>

- <span data-ttu-id="3d1ae-114">Tipos personalizados não dão suporte à pesquisa em várias fontes (especificado em **ContentSources**).</span><span class="sxs-lookup"><span data-stu-id="3d1ae-114">Custom types don’t support searching across multiple sources (specified in **contentSources**).</span></span> <span data-ttu-id="3d1ae-115">Você pode pesquisar apenas uma conexão por vez.</span><span class="sxs-lookup"><span data-stu-id="3d1ae-115">You can search only one connection at a time.</span></span>

- <span data-ttu-id="3d1ae-116">Você deve especificar a propriedade **stored_fields** , caso contrário os resultados da pesquisa não serão retornados.</span><span class="sxs-lookup"><span data-stu-id="3d1ae-116">You must specify the **stored_fields** property, otherwise search results are not returned.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3d1ae-117">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="3d1ae-117">Next steps</span></span>

<span data-ttu-id="3d1ae-118">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="3d1ae-118">Find out more about:</span></span>

- [<span data-ttu-id="3d1ae-119">Usar a API de pesquisa</span><span class="sxs-lookup"><span data-stu-id="3d1ae-119">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)