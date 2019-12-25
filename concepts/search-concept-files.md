---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar arquivos
description: Você pode usar a API de pesquisa da Microsoft para pesquisar arquivos armazenados no SharePoint ou no OneDrive.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 0b8db24a8b9ccd63ac3d3be800b209a64eb3aa9d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866914"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-files"></a><span data-ttu-id="44e03-103">Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar arquivos</span><span class="sxs-lookup"><span data-stu-id="44e03-103">Use the Microsoft Search API in Microsoft Graph to search files</span></span>

<span data-ttu-id="44e03-104">Você pode usar a API de pesquisa da Microsoft para pesquisar arquivos armazenados no SharePoint ou no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="44e03-104">You can use the Microsoft Search API to search files stored in SharePoint or OneDrive.</span></span> <span data-ttu-id="44e03-105">A API do Microsoft Search usa um modelo de relevância que utiliza sinais do Microsoft Graph sobre as relações e atividades dos usuários.</span><span class="sxs-lookup"><span data-stu-id="44e03-105">The Microsoft Search API uses a relevance model that makes use of signals from Microsoft Graph about users' relationships and activities.</span></span> <span data-ttu-id="44e03-106">Isso permite que você retorne e promova o conteúdo que os usuários se preocupam, em uma experiência de pesquisa de arquivo consistente com a guia **arquivos** que lista os resultados da pesquisa no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="44e03-106">This enables you to return and promote the content that users care about, in a file search experience that is consistent with the **Files** tab that lists search results in SharePoint.</span></span> 

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="44e03-107">A API também pode trazer arquivos externos expostos por meio do recurso [externalfile](/graph/api/resources/externalfile?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="44e03-107">The API can also surface external files exposed via the [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) resource.</span></span>

## <a name="search-sharepoint-or-onedrive-files"></a><span data-ttu-id="44e03-108">Pesquisar arquivos do SharePoint ou do OneDrive</span><span class="sxs-lookup"><span data-stu-id="44e03-108">Search SharePoint or OneDrive files</span></span>

<span data-ttu-id="44e03-109">Você pode usar o KQL em termos de pesquisa de consultas do SharePoint e do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="44e03-109">You can use KQL in search terms of queries for SharePoint and OneDrive.</span></span> <span data-ttu-id="44e03-110">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="44e03-110">For example:</span></span>

- <span data-ttu-id="44e03-111">`"query": "contoso filetype:docx OR filetype:doc"`escopo a consulta em documentos do Word.</span><span class="sxs-lookup"><span data-stu-id="44e03-111">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="44e03-112">`"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`escopo a consulta para uma determinada pasta dentro de um site.</span><span class="sxs-lookup"><span data-stu-id="44e03-112">`"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>

<span data-ttu-id="44e03-113">Para ser válido, a restrição de propriedades deve especificar um nome de propriedade gerenciada válido e consultável na condição.</span><span class="sxs-lookup"><span data-stu-id="44e03-113">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

### <a name="example"></a><span data-ttu-id="44e03-114">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44e03-114">Example</span></span>

#### <a name="request"></a><span data-ttu-id="44e03-115">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44e03-115">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="44e03-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="44e03-116">Response</span></span>

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

## <a name="search-external-files-well-known-types"></a><span data-ttu-id="44e03-117">Pesquisar arquivos externos (tipos bem conhecidos)</span><span class="sxs-lookup"><span data-stu-id="44e03-117">Search external files (well-known types)</span></span>

<span data-ttu-id="44e03-118">O [conector de compartilhamento de arquivos](/MicrosoftSearch/file-share-connector) está disponível no Microsoft Search por padrão.</span><span class="sxs-lookup"><span data-stu-id="44e03-118">The [file share connector](/MicrosoftSearch/file-share-connector) is available in Microsoft Search by default.</span></span> <span data-ttu-id="44e03-119">Você pode usá-lo para indexar arquivos disponíveis em um compartilhamento de arquivos.</span><span class="sxs-lookup"><span data-stu-id="44e03-119">You can use it to index files available on a file share.</span></span> <span data-ttu-id="44e03-120">Você pode usar a API de consulta para consultar todos os arquivos externos.</span><span class="sxs-lookup"><span data-stu-id="44e03-120">You can use the query API to query all external files.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="example"></a><span data-ttu-id="44e03-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44e03-121">Example</span></span>

<span data-ttu-id="44e03-122">O exemplo a seguir retorna todos os arquivos externos configurados para o locatário e classifica os resultados por relevância.</span><span class="sxs-lookup"><span data-stu-id="44e03-122">The following example returns all configured external files for the tenant, and sorts the results by relevance.</span></span>

#### <a name="request"></a><span data-ttu-id="44e03-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44e03-123">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.externalFile"
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

#### <a name="response"></a><span data-ttu-id="44e03-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="44e03-124">Response</span></span>

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 4,
          "moreResultsAvailable": true,
          // Hits represent the search results
          "hits": [
            {
              "_id": "FsHvoeTuRRVLnuEZLEVBfSQAAWTp",
              "_score": 1,
              "_sortField": "Relevance",
              "_source": {
                "@odata.type": "#microsoft.graph.externalFile",
                "id": "FsHvoeTuRRVLnuEZLEVBfSQAAWTp",
                "extension": "pptx",
                "name": "Contoso-Overview.pptx",
                "lastModifiedTime": "2018-05-09T04:01:14Z",
                "modifiedBy": "Baala Vedantam",
                "title": "Contoso Overview 2018",
                "url": "file://fileshare01/External Presentations/Contoso-Overview.pptx"
              }
            },
            {
              //Another searchHit
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="search-all-files-including-externalfile-instances"></a><span data-ttu-id="44e03-125">Pesquisar todos os arquivos (incluindo instâncias de arquivos externos)</span><span class="sxs-lookup"><span data-stu-id="44e03-125">Search all files (including externalFile instances)</span></span>

<span data-ttu-id="44e03-126">Você pode pesquisar todos os arquivos de um locatário, incluindo arquivos armazenados em [driveItems](/graph/api/resources/driveitem?view=graph-rest-beta) e arquivos externos, especificando dois tipos de entidade na solicitação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="44e03-126">You can search all the files in a tenant, including files stored in [driveItems](/graph/api/resources/driveitem?view=graph-rest-beta) and external files, by specifying two entity types in the search request.</span></span>

<span data-ttu-id="44e03-127">A resposta inclui as instâncias **driveItem** e **externalItem** no `_sources` campo de cada objeto [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="44e03-127">The response includes **driveItem** and **externalItem** instances in the `_sources` field of each [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta) object.</span></span>

### <a name="example"></a><span data-ttu-id="44e03-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44e03-128">Example</span></span>

<span data-ttu-id="44e03-129">O exemplo a seguir retorna todos os objetos **externalfile** e **driveItem** configurados no locatário que satisfazem os termos de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="44e03-129">The following example returns all configured **externalFile** and **driveItem** objects in the tenant that satisfy the search terms.</span></span> <span data-ttu-id="44e03-130">Ele classifica os resultados por relevância.</span><span class="sxs-lookup"><span data-stu-id="44e03-130">It sorts the results by relevance.</span></span>

### <a name="request"></a><span data-ttu-id="44e03-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44e03-131">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.driveItem",
        "microsoft.graph.externalFile"
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

## <a name="known-limitations"></a><span data-ttu-id="44e03-132">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="44e03-132">Known limitations</span></span>

<span data-ttu-id="44e03-133">Você não pode fazer o escopo de uma consulta para uma ID de conexão específica.</span><span class="sxs-lookup"><span data-stu-id="44e03-133">You cannot scope a query to a particular connection ID.</span></span>

## <a name="next-steps"></a><span data-ttu-id="44e03-134">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="44e03-134">Next steps</span></span>

- [<span data-ttu-id="44e03-135">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="44e03-135">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)

