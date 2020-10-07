---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar arquivos
description: Você pode usar a API de pesquisa da Microsoft para pesquisar arquivos armazenados no OneDrive ou no SharePoint.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 3b6f8e1cbdaf686e1ab73c2b168968221d9efbcc
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373983"
---
# <a name="use-the-microsoft-search-api-to-search-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="b26f8-103">Usar a API de pesquisa da Microsoft para pesquisar conteúdo no OneDrive e no SharePoint</span><span class="sxs-lookup"><span data-stu-id="b26f8-103">Use the Microsoft Search API to search content in OneDrive and SharePoint</span></span>

<span data-ttu-id="b26f8-104">Use a API de pesquisa da Microsoft para pesquisar conteúdo armazenado no OneDrive ou no SharePoint: arquivos, pastas, listas, itens de lista ou sites.</span><span class="sxs-lookup"><span data-stu-id="b26f8-104">Use the Microsoft Search API to search content stored in OneDrive or SharePoint: files, folders, lists, list items, or sites.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="b26f8-105">A API de pesquisa permite que você escopo os tipos de conteúdo a serem recuperados no OneDrive ou no SharePoint especificando a propriedade **EntityTypes** no [searchRequest](/graph/api/resources/searchRequest?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="b26f8-105">The Search API lets you scope the types of content to retrieve in OneDrive or SharePoint by specifying the **entityTypes** property on the [searchRequest](/graph/api/resources/searchRequest?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="b26f8-106">A parte posterior deste artigo mostra alguns exemplos:</span><span class="sxs-lookup"><span data-stu-id="b26f8-106">The later part of this article shows a few examples:</span></span>

- [<span data-ttu-id="b26f8-107">Exemplo 1: Arquivos de pesquisa</span><span class="sxs-lookup"><span data-stu-id="b26f8-107">Example 1: Search files</span></span>](#example-1-search-files)
- [<span data-ttu-id="b26f8-108">Exemplo 2: itens de lista de pesquisa</span><span class="sxs-lookup"><span data-stu-id="b26f8-108">Example 2: Search list items</span></span>](#example-2-search-list-items)
- [<span data-ttu-id="b26f8-109">Exemplo 3: sites de pesquisa</span><span class="sxs-lookup"><span data-stu-id="b26f8-109">Example 3: Search sites</span></span>](#example-3-search-sites)
- [<span data-ttu-id="b26f8-110">Exemplo 4: Pesquisar todo o conteúdo no OneDrive e no SharePoint</span><span class="sxs-lookup"><span data-stu-id="b26f8-110">Example 4: Search all content in OneDrive and SharePoint</span></span>](#example-4-search-all-content-in-onedrive-and-sharepoint)

## <a name="specify-select-properties"></a><span data-ttu-id="b26f8-111">Especificar propriedades de seleção</span><span class="sxs-lookup"><span data-stu-id="b26f8-111">Specify select properties</span></span>

<span data-ttu-id="b26f8-112">Você pode especificar os campos que deseja de volta na resposta, como parte da subpropriedade **Fields** de um objeto [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta&preserve-view=true) na resposta.</span><span class="sxs-lookup"><span data-stu-id="b26f8-112">You can specify the fields you want back in the response, as part of the **fields** sub-property of a [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta&preserve-view=true) object in the response.</span></span> <span data-ttu-id="b26f8-113">Essa é uma maneira de aparar a resposta sobre o fio ou para solicitar algumas propriedades específicas que não fazem parte do esquema pronto para uso.</span><span class="sxs-lookup"><span data-stu-id="b26f8-113">This is a way to either trim down the response over the wire, or to request some specific properties that are not part of the out-of-the-box schema.</span></span>

<span data-ttu-id="b26f8-114">Observe que a seleção de propriedade só está disponível para **ListItem** , pois esta é a única entidade do SharePoint no Microsoft Graph que oferece suporte a propriedades personalizadas.</span><span class="sxs-lookup"><span data-stu-id="b26f8-114">Note that property selection is only available for **listItem** since this is the only SharePoint entity in Microsoft Graph that supports custom properties.</span></span>

<span data-ttu-id="b26f8-115">Para recuperar uma propriedade personalizada de um **driveItem**, procure **ListItem** .</span><span class="sxs-lookup"><span data-stu-id="b26f8-115">To retrieve a custom property for a **driveItem**, query **listItem** instead.</span></span>

### <a name="request"></a><span data-ttu-id="b26f8-116">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b26f8-116">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "listItem"
      ],
      "query": {
        "queryString": "contoso"
      },
      "fields": [
          "title",
          "contentclass"
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b26f8-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="b26f8-117">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "contoso.sharepoint.com,6598ee0b-0f5f-4416-a0ae-66d864efb43a,60024ce8-e74d-4d63-a939-ad00cd738670",
              "rank": 1,
              "summary": "",
              "resource": {
                "@odata.type": "#microsoft.graph.listItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                "parentReference": {
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
                },
                "fields": {
                  "contentclass": "STS_ListItem_GenericList",
                  "title": "Contoso issue "
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

## <a name="use-filters-in-search-queries"></a><span data-ttu-id="b26f8-118">Usar filtros em consultas de pesquisa</span><span class="sxs-lookup"><span data-stu-id="b26f8-118">Use filters in search queries</span></span>

<span data-ttu-id="b26f8-119">Você pode usar o KQL em termos de pesquisa de consultas do OneDrive e do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b26f8-119">You can use KQL in search terms of queries for OneDrive and SharePoint.</span></span> <span data-ttu-id="b26f8-120">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="b26f8-120">For example:</span></span>

- <span data-ttu-id="b26f8-121">`"query": "contoso filetype:docx OR filetype:doc"` escopo a consulta em documentos do Word.</span><span class="sxs-lookup"><span data-stu-id="b26f8-121">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="b26f8-122">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` escopo a consulta para uma determinada pasta dentro de um site.</span><span class="sxs-lookup"><span data-stu-id="b26f8-122">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>
- <span data-ttu-id="b26f8-123">`"query": "contoso AND isDocument=true"` escopos a consulta para retornar apenas os documentos.</span><span class="sxs-lookup"><span data-stu-id="b26f8-123">`"query": "contoso AND isDocument=true"` scopes the query to only return documents.</span></span> <span data-ttu-id="b26f8-124">Qualquer contêiner (pasta, biblioteca de documentos) não será retornado.</span><span class="sxs-lookup"><span data-stu-id="b26f8-124">Any container (folder, document library) will not be returned.</span></span>
- <span data-ttu-id="b26f8-125">`"query": "contoso contentclass:STS_List_Events"` escopos a consulta para eventos de calendário armazenados no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b26f8-125">`"query": "contoso contentclass:STS_List_Events"` scopes the query to Calendar events stored in SharePoint.</span></span>

<span data-ttu-id="b26f8-126">Para ser válido, a restrição de propriedades deve especificar um nome de propriedade gerenciada válido e consultável na condição.</span><span class="sxs-lookup"><span data-stu-id="b26f8-126">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

## <a name="example-1-search-files"></a><span data-ttu-id="b26f8-127">Exemplo 1: Arquivos de pesquisa</span><span class="sxs-lookup"><span data-stu-id="b26f8-127">Example 1: Search files</span></span>

### <a name="request"></a><span data-ttu-id="b26f8-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b26f8-128">Request</span></span>

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
        "queryString": "contoso"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b26f8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b26f8-129">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
              "rank": 1,
              "summary": "<c0>Contoso</c0> Detailed Design <ddd/>",
              "resource": {
                "@odata.type": "#microsoft.graph.driveItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                "name": "web_part_test_long Notebook",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                "createdBy": {
                 "user": {
                   "displayName": "Michaelvincent Santos;Provisioning User"
                  }
                },
                "lastModifiedBy": {
                  "user": {
                    "displayName": "Richard Mayer"
                  }
                },
                "parentReference": {
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
                }
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

## <a name="example-2-search-list-items"></a><span data-ttu-id="b26f8-130">Exemplo 2: itens de lista de pesquisa</span><span class="sxs-lookup"><span data-stu-id="b26f8-130">Example 2: Search list items</span></span>

### <a name="request"></a><span data-ttu-id="b26f8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b26f8-131">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "listItem"
      ],
      "query": {
        "queryString": "contoso"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b26f8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b26f8-132">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
              "rank": 1,
              "summary": "",
              "resource": {
                "@odata.type": "#microsoft.graph.listItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                "name": "web_part_test_long Notebook",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/Lists/Issue tracker list/DispForm.aspx?ID=1"
                "createdBy": {
                 "user": {
                   "displayName": "Michaelvincent Santos;Provisioning User"
                  }
                },
                "lastModifiedBy": {
                  "user": {
                    "displayName": "Richard Mayer"
                  }
                },
                "parentReference": {
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
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

## <a name="example-3-search-sites"></a><span data-ttu-id="b26f8-133">Exemplo 3: sites de pesquisa</span><span class="sxs-lookup"><span data-stu-id="b26f8-133">Example 3: Search sites</span></span>

### <a name="request"></a><span data-ttu-id="b26f8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b26f8-134">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "site"
      ],
      "query": {
        "queryString": "contoso"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b26f8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b26f8-135">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "contoso.sharepoint.com,6598ee0b-0f5f-4416-a0ae-66d864efb43a,60024ce8-e74d-4d63-a939-ad00cd738670",
              "rank": 1,
              "summary": "",
              "resource": {
                "@odata.type": "#microsoft.graph.site",
                "id": "contoso.sharepoint.com,6598ee0b-0f5f-4416-a0ae-66d864efb43a,60024ce8-e74d-4d63-a939-ad00cd738670",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "description": "Contoso Communication Site",
                "lastModifiedDateTime": "2020-08-30T06:41:56Z",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/"
              }
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="example-4-search-all-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="b26f8-136">Exemplo 4: Pesquisar todo o conteúdo no OneDrive e no SharePoint</span><span class="sxs-lookup"><span data-stu-id="b26f8-136">Example 4: Search all content in OneDrive and SharePoint</span></span>

<span data-ttu-id="b26f8-137">Este exemplo consulta todo o conteúdo de sites do OneDrive e do SharePoint aos quais o usuário conectado tem acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="b26f8-137">This example queries all the content in OneDrive and SharePoint sites to which the signed-in user has read access.</span></span> <span data-ttu-id="b26f8-138">A propriedade **Resource** na resposta retorna correspondências que são arquivos e pastas como objetos **driveItem** , correspondências que são contêineres (listas do SharePoint) como **lista**e todas as outras correspondências como **ListItem**.</span><span class="sxs-lookup"><span data-stu-id="b26f8-138">The **resource** property in the response returns matches that are files and folders as **driveItem** objects, matches that are containers (SharePoint lists) as **list**, and all other matches as **listItem**.</span></span>

### <a name="request"></a><span data-ttu-id="b26f8-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b26f8-139">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "driveItem", "listItem", "list"
      ],
      "query": {
        "queryString": "contoso"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b26f8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b26f8-140">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "@odata.type": "#microsoft.graph.searchHitsContainer",
              "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
              "rank": 1,
              "summary": "<c0>Contoso</c0> Detailed Design <ddd/>",
              "resource": {
                "@odata.type": "#microsoft.graph.driveItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                "name": "web_part_test_long Notebook",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                "createdBy": {
                 "user": {
                   "displayName": "Michaelvincent Santos;Provisioning User"
                  }
                },
                "lastModifiedBy": {
                  "user": {
                    "displayName": "Richard Mayer"
                  }
                },
                "parentReference": {
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
                }
                "fileSystemInfo": {
                  "createdDateTime": "2019-06-10T06:37:43Z",
                  "lastModifiedDateTime": "2019-06-10T06:37:43Z"
                }
              }
            },
            {
              "@odata.type": "#microsoft.graph.searchHit",
              "hitId": "51eef59e-5d49-4d28-96f0-864cf90765e0",
              "rank": 2,
              "summary": "",
              "resource": {
                "@odata.type": "#microsoft.graph.list",
                "displayName": "Contoso - Documents",
                "id": "51eef59e-5d49-4d28-96f0-864cf90765e0",
                "description": "",
                "lastModifiedDateTime": "2020-07-08T18:17:59+00:00",
                "name": "Shared Documents",
                "parentReference": {
                "siteId": "microsoft.sharepoint-df.com,220fd155-0ea2-477c-a816-5c08fdc45f5d,fad16ab6-0736-4fbc-a053-087296b47c99"
                },
                "webUrl": "https://microsoft.sharepoint-df.com/teams/spoppe/collab/TaskBoard/Contoso/Shared Documents/Forms/AllItems.aspx"
              }
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="known-limitations"></a><span data-ttu-id="b26f8-141">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="b26f8-141">Known limitations</span></span>

<span data-ttu-id="b26f8-142">Ao procurar **drive**, você precisa incluir no termo **QueryString** a contido no nome da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="b26f8-142">When searching for **drive**, you need to include in the **queryString** a term contained in the name of the document library.</span></span> <span data-ttu-id="b26f8-143">A consulta `*` não é suportada e não retorna todas as unidades disponíveis.</span><span class="sxs-lookup"><span data-stu-id="b26f8-143">Querying `*` is not supported and does not return all available drives.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b26f8-144">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="b26f8-144">Next steps</span></span>

- [<span data-ttu-id="b26f8-145">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="b26f8-145">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
