---
title: Pesquisar arquivos (incluindo externalFile)
description: A API de consulta permite que você pesquise entre arquivos (DriveItem ou arquivos externos).
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 95a8b99b9970ec239935ee2c35afeec581a1b35f
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703944"
---
# <a name="search-files-including-externalfile"></a><span data-ttu-id="8dd79-103">Pesquisar arquivos (incluindo externalFile)</span><span class="sxs-lookup"><span data-stu-id="8dd79-103">Search files (including externalFile)</span></span>

<span data-ttu-id="8dd79-104">A API do Microsoft Search permite pesquisar arquivos armazenados no SharePoint ou no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8dd79-104">The Microsoft Search API lets you search files stored in SharePoint or OneDrive.</span></span> <span data-ttu-id="8dd79-105">Ele usa um modelo de relevância que utiliza sinais do Microsoft Graph sobre as relações e atividades dos usuários.</span><span class="sxs-lookup"><span data-stu-id="8dd79-105">It uses a relevance model which makes use of signals from Microsoft Graph about users' relations and activities.</span></span> <span data-ttu-id="8dd79-106">Isso permite retornar e promover o conteúdo com o qual os usuários se preocupam, em uma experiência de pesquisa de arquivo consistente com a guia **arquivos** que lista os resultados da pesquisa no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8dd79-106">This allows returning and promoting content that users care about, in a file search experience that is consistent with the **Files** tab that lists search results in SharePoint.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="8dd79-107">Além disso, a API pode trazer arquivos externos expostos por meio do recurso [externalfile](/graph/api/resources/externalfile?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="8dd79-107">In addition, the API can surface external files exposed via the [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) resource.</span></span>

## <a name="search-sharepoint-or-onedrive-files"></a><span data-ttu-id="8dd79-108">Pesquisar arquivos do SharePoint ou do OneDrive</span><span class="sxs-lookup"><span data-stu-id="8dd79-108">Search SharePoint or OneDrive files</span></span>

<span data-ttu-id="8dd79-109">Você pode usar o KQL em termos de pesquisa de consultas do SharePoint e do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8dd79-109">You can use KQL in search terms of queries for SharePoint and OneDrive.</span></span> <span data-ttu-id="8dd79-110">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="8dd79-110">For example:</span></span>

- <span data-ttu-id="8dd79-111">`"query" : "contoso filetype:docx OR filetype:doc"`consultas de escopos em documentos do Word</span><span class="sxs-lookup"><span data-stu-id="8dd79-111">`"query" : "contoso filetype:docx OR filetype:doc"` scopes queries to Word documents</span></span>
- <span data-ttu-id="8dd79-112">`"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`escopo a consulta para uma determinada pasta dentro de um site.</span><span class="sxs-lookup"><span data-stu-id="8dd79-112">`"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>

<span data-ttu-id="8dd79-113">Para ser válido, a restrição de propriedades deve especificar um nome de propriedade gerenciada válido Consultád na condição.</span><span class="sxs-lookup"><span data-stu-id="8dd79-113">In order to be valid, properties restriction should specify a valid Queryable managed property name in the condition.</span></span>

### <a name="example"></a><span data-ttu-id="8dd79-114">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8dd79-114">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8dd79-115">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dd79-115">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="8dd79-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dd79-116">Response</span></span>

<span data-ttu-id="8dd79-117">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8dd79-117">Here is an example of the response.</span></span>

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

## <a name="search-external-files-well-known-types"></a><span data-ttu-id="8dd79-118">Pesquisar arquivos externos (tipos bem conhecidos)</span><span class="sxs-lookup"><span data-stu-id="8dd79-118">Search external files (well-known types)</span></span>

<span data-ttu-id="8dd79-119">O [conector de compartilhamento de arquivos](/MicrosoftSearch/file-share-connector) é um conector "pronto para uso" disponível no Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="8dd79-119">[File share connector](/MicrosoftSearch/file-share-connector) is an "out of the box" connector available in Microsoft Search.</span></span> <span data-ttu-id="8dd79-120">Permite indexar arquivos disponíveis em um compartilhamento de arquivos.</span><span class="sxs-lookup"><span data-stu-id="8dd79-120">It enables you to index files available on a file share.</span></span> <span data-ttu-id="8dd79-121">Você pode usar a API de consulta para consultar todos os arquivos externos.</span><span class="sxs-lookup"><span data-stu-id="8dd79-121">You can use the query API to query all external files.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="example"></a><span data-ttu-id="8dd79-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8dd79-122">Example</span></span>

<span data-ttu-id="8dd79-123">O exemplo a seguir retorna todos os conectores externalfile configurados para o locatário e classifica os resultados por relevância.</span><span class="sxs-lookup"><span data-stu-id="8dd79-123">The following example returns all configured externalFile connector for the tenant, and sorts the results by relevance.</span></span>

#### <a name="request"></a><span data-ttu-id="8dd79-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dd79-124">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="8dd79-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dd79-125">Response</span></span>

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

## <a name="search-all-files-including-externalfile-instances"></a><span data-ttu-id="8dd79-126">Pesquisar todos os arquivos (incluindo instâncias de arquivos externos)</span><span class="sxs-lookup"><span data-stu-id="8dd79-126">Search all files (including externalFile instances)</span></span>

<span data-ttu-id="8dd79-127">Você pode pesquisar todos os arquivos de um locatário, incluindo o [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) e todos os arquivos externos, especificando dois tipos de entidade na solicitação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8dd79-127">You can search all the files in a tenant, including [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) and all external files, by specifying two entity types in the search request.</span></span>

<span data-ttu-id="8dd79-128">A resposta fornece uma mistura de instâncias **driveItem** e externalItem no `_sources` campo de cada objeto [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="8dd79-128">The response provide a mix of **driveItem** and externalItem instances in the `_sources` field of each [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta) object.</span></span>

### <a name="example"></a><span data-ttu-id="8dd79-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8dd79-129">Example</span></span>

<span data-ttu-id="8dd79-130">O exemplo a seguir retorna todos os conectores **externos** defile e objetos **driveItem** do locatário que satisfazem os termos de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8dd79-130">The following example returns all configured **externalFile** connector and **driveItem** objects of the tenant's that satisfy the search terms.</span></span> <span data-ttu-id="8dd79-131">Ele classifica os resultados por relevância.</span><span class="sxs-lookup"><span data-stu-id="8dd79-131">It sorts the results by relevance.</span></span>

### <a name="request"></a><span data-ttu-id="8dd79-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dd79-132">Request</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="8dd79-133">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="8dd79-133">Known limitations</span></span>

<span data-ttu-id="8dd79-134">Você não pode fazer o escopo de uma consulta para uma ConnectionID específica.</span><span class="sxs-lookup"><span data-stu-id="8dd79-134">You cannot scope a query to a particular connectionId.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8dd79-135">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8dd79-135">Next steps</span></span>

<span data-ttu-id="8dd79-136">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="8dd79-136">Find out more about:</span></span>

- [<span data-ttu-id="8dd79-137">Usar a API de pesquisa</span><span class="sxs-lookup"><span data-stu-id="8dd79-137">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
