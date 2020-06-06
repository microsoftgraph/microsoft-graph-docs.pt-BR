---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para Pesquisar tipos personalizados
description: Você pode usar a API de pesquisa da Microsoft para importar dados externos por meio do recurso [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) e executar consultas de pesquisa nesse conteúdo externo.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: e4dbdb7f324edc882a8bb9514a5f406bceee6ad6
ms.sourcegitcommit: 093d89c7583bb6880c8395e9498a1f33cdd938b4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44568766"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-custom-types"></a><span data-ttu-id="1b9f8-103">Usar a API de pesquisa da Microsoft no Microsoft Graph para Pesquisar tipos personalizados</span><span class="sxs-lookup"><span data-stu-id="1b9f8-103">Use the Microsoft Search API in Microsoft Graph to search custom types</span></span>

<span data-ttu-id="1b9f8-104">Você pode usar a API de pesquisa da Microsoft para importar dados externos por meio do recurso [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) e executar consultas de pesquisa nesse conteúdo externo.</span><span class="sxs-lookup"><span data-stu-id="1b9f8-104">You can use the Microsoft Search API to import external data via the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) resource, and run search queries on this external content.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="1b9f8-105">Para Pesquisar tipos personalizados, especifique o seguinte no corpo da solicitação do método de [consulta](/graph/api/search-query?view=graph-rest-beta) :</span><span class="sxs-lookup"><span data-stu-id="1b9f8-105">To search for custom types, specify the following in the [query](/graph/api/search-query?view=graph-rest-beta) method request body:</span></span>

- <span data-ttu-id="1b9f8-106">A propriedade **ContentSources** para incluir a ID de conexão atribuída durante a configuração do conector</span><span class="sxs-lookup"><span data-stu-id="1b9f8-106">The **contentSources** property to include the connection ID that is assigned during the connector setup</span></span>

- <span data-ttu-id="1b9f8-107">A propriedade **EntityTypes** como`externalItem`</span><span class="sxs-lookup"><span data-stu-id="1b9f8-107">The **entityTypes** property as `externalItem`</span></span>

- <span data-ttu-id="1b9f8-108">A propriedade **stored_fields** para incluir os campos no item externo que você deseja recuperar</span><span class="sxs-lookup"><span data-stu-id="1b9f8-108">The **stored_fields** property to include the fields in the external item you want to retrieve</span></span>

## <a name="example"></a><span data-ttu-id="1b9f8-109">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b9f8-109">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b9f8-110">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b9f8-110">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "externalItem"
      ],
      "contentSources": [
        "/external/connections/servicenow-connector-contoso"
      ],
      "query": {
        "query_string": {
          "query": "contoso tickets"
        }
      },
      "from": 0,
      "size": 25,
      "stored_fields": [
        "title",
        "priority",
        "description"
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1b9f8-111">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b9f8-111">Response</span></span>

```json
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

## <a name="known-limitations"></a><span data-ttu-id="1b9f8-112">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="1b9f8-112">Known limitations</span></span>

- <span data-ttu-id="1b9f8-113">Tipos personalizados não dão suporte à pesquisa em várias fontes (especificado em **ContentSources**).</span><span class="sxs-lookup"><span data-stu-id="1b9f8-113">Custom types don’t support searching across multiple sources (specified in **contentSources**).</span></span> <span data-ttu-id="1b9f8-114">Você pode pesquisar apenas uma conexão por vez.</span><span class="sxs-lookup"><span data-stu-id="1b9f8-114">You can search only one connection at a time.</span></span>

- <span data-ttu-id="1b9f8-115">Você deve especificar a propriedade **stored_fields** ; caso contrário, os resultados da pesquisa não serão retornados.</span><span class="sxs-lookup"><span data-stu-id="1b9f8-115">You must specify the **stored_fields** property; otherwise, search results are not returned.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1b9f8-116">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="1b9f8-116">Next steps</span></span>

- [<span data-ttu-id="1b9f8-117">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="1b9f8-117">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
