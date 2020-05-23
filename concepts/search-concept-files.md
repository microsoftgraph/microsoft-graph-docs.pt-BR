---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar arquivos
description: Você pode usar a API de pesquisa da Microsoft para pesquisar arquivos armazenados no SharePoint ou no OneDrive.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 7a7e5c92f3ffe9399732d6454d3e06d2013f8768
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345839"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-files"></a><span data-ttu-id="9a2e6-103">Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar arquivos</span><span class="sxs-lookup"><span data-stu-id="9a2e6-103">Use the Microsoft Search API in Microsoft Graph to search files</span></span>

<span data-ttu-id="9a2e6-104">Você pode usar a API de pesquisa da Microsoft para pesquisar arquivos armazenados no SharePoint ou no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9a2e6-104">You can use the Microsoft Search API to search files stored in SharePoint or OneDrive.</span></span> <span data-ttu-id="9a2e6-105">A API do Microsoft Search usa um modelo de relevância que utiliza sinais do Microsoft Graph sobre as relações e atividades dos usuários.</span><span class="sxs-lookup"><span data-stu-id="9a2e6-105">The Microsoft Search API uses a relevance model that makes use of signals from Microsoft Graph about users' relationships and activities.</span></span> <span data-ttu-id="9a2e6-106">Isso permite que você retorne e promova o conteúdo que os usuários se preocupam, em uma experiência de pesquisa de arquivo consistente com a guia **arquivos** que lista os resultados da pesquisa no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9a2e6-106">This enables you to return and promote the content that users care about, in a file search experience that is consistent with the **Files** tab that lists search results in SharePoint.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="search-sharepoint-or-onedrive-files"></a><span data-ttu-id="9a2e6-107">Pesquisar arquivos do SharePoint ou do OneDrive</span><span class="sxs-lookup"><span data-stu-id="9a2e6-107">Search SharePoint or OneDrive files</span></span>

<span data-ttu-id="9a2e6-108">Você pode usar o KQL em termos de pesquisa de consultas do SharePoint e do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9a2e6-108">You can use KQL in search terms of queries for SharePoint and OneDrive.</span></span> <span data-ttu-id="9a2e6-109">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="9a2e6-109">For example:</span></span>

- <span data-ttu-id="9a2e6-110">`"query": "contoso filetype:docx OR filetype:doc"`escopo a consulta em documentos do Word.</span><span class="sxs-lookup"><span data-stu-id="9a2e6-110">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="9a2e6-111">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`escopo a consulta para uma determinada pasta dentro de um site.</span><span class="sxs-lookup"><span data-stu-id="9a2e6-111">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>

<span data-ttu-id="9a2e6-112">Para ser válido, a restrição de propriedades deve especificar um nome de propriedade gerenciada válido e consultável na condição.</span><span class="sxs-lookup"><span data-stu-id="9a2e6-112">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

### <a name="example"></a><span data-ttu-id="9a2e6-113">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a2e6-113">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9a2e6-114">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a2e6-114">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.driveItem"
      ],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="9a2e6-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a2e6-115">Response</span></span>

<!---TODO nmoreau team Include one example of externalItem response.-->
```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "test"
      ],
      "hitsContainers": [
        {
          "total": 350,
          "moreResultsAvailable": true,
          "hits": [
            {
              "_id": "FlULeN/ui/1GjLx1rUfio5UAAEl",
              "_score": 1,
              "_sortField": "Relevance",
              "_summary": "<c0>Contoso</c0> Detailed Design <ddd/>",
              "_source": {
                "@odata.type": "#microsoft.graph.driveItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                "name": "web_part_test_long Notebook",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                "lastModifiedBy": {
                  "user": {
                    "displayName": "Richard Mayer"
                  }
                },
                "fileSystemInfo": {
                  "createdDateTime": "2019-06-10T06:37:43Z",
                  "lastModifiedDateTime": "2019-06-10T06:37:43Z"
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

## <a name="next-steps"></a><span data-ttu-id="9a2e6-116">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9a2e6-116">Next steps</span></span>

- [<span data-ttu-id="9a2e6-117">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="9a2e6-117">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
