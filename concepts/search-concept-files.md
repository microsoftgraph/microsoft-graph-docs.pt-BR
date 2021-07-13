---
title: Usar a API Pesquisa da Microsoft no Microsoft Graph para pesquisar arquivos
description: Você pode usar a API Pesquisa da Microsoft para pesquisar arquivos armazenados OneDrive ou SharePoint.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 93dca7b4c431140646ee22ae6772448e0554e35a
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401334"
---
# <a name="use-the-microsoft-search-api-to-search-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="8ead7-103">Use a API Pesquisa da Microsoft para pesquisar conteúdo em OneDrive e SharePoint</span><span class="sxs-lookup"><span data-stu-id="8ead7-103">Use the Microsoft Search API to search content in OneDrive and SharePoint</span></span>

<span data-ttu-id="8ead7-104">Use a API Pesquisa da Microsoft para pesquisar conteúdo armazenado em OneDrive ou SharePoint: arquivos, pastas, listas, itens de lista ou sites.</span><span class="sxs-lookup"><span data-stu-id="8ead7-104">Use the Microsoft Search API to search content stored in OneDrive or SharePoint: files, folders, lists, list items, or sites.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="8ead7-105">A API de Pesquisa permite que você escopo os tipos de conteúdo a ser recuperado em OneDrive ou SharePoint especificando a propriedade **entityTypes** no [searchRequest](/graph/api/resources/searchRequest).</span><span class="sxs-lookup"><span data-stu-id="8ead7-105">The Search API lets you scope the types of content to retrieve in OneDrive or SharePoint by specifying the **entityTypes** property on the [searchRequest](/graph/api/resources/searchRequest).</span></span> <span data-ttu-id="8ead7-106">Este artigo descreve alguns exemplos.</span><span class="sxs-lookup"><span data-stu-id="8ead7-106">This article describes some examples.</span></span>

## <a name="example-1-search-files"></a><span data-ttu-id="8ead7-107">Exemplo 1: Arquivos de pesquisa</span><span class="sxs-lookup"><span data-stu-id="8ead7-107">Example 1: Search files</span></span>

### <a name="request"></a><span data-ttu-id="8ead7-108">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ead7-108">Request</span></span>

```HTTP
POST /search/query
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

### <a name="response"></a><span data-ttu-id="8ead7-109">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ead7-109">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
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
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0",
                  "driveId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b",
                  "sharepointIds": {
                      "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                      "listItemId": "1027",
                      "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
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

## <a name="example-2-search-list-items"></a><span data-ttu-id="8ead7-110">Exemplo 2: Itens de lista de pesquisa</span><span class="sxs-lookup"><span data-stu-id="8ead7-110">Example 2: Search list items</span></span>

### <a name="request"></a><span data-ttu-id="8ead7-111">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ead7-111">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="8ead7-112">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ead7-112">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
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
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/Lists/Issue tracker list/DispForm.aspx?ID=1",
                "sharepointIds": {
                    "listId": "33498de0-d695-4d23-ac26-e1bf95a3206e",
                    "listItemId": "13"
                },
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
                  "sharepointIds":{
                    "listId":"da61a2b0-4120-4a3f-812b-0fc0d79bf16b"  
                  },
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

## <a name="example-3-search-sites"></a><span data-ttu-id="8ead7-113">Exemplo 3: Sites de pesquisa</span><span class="sxs-lookup"><span data-stu-id="8ead7-113">Example 3: Search sites</span></span>

### <a name="request"></a><span data-ttu-id="8ead7-114">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ead7-114">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="8ead7-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ead7-115">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
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

## <a name="example-4-search-all-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="8ead7-116">Exemplo 4: Pesquisar todo o conteúdo em OneDrive e SharePoint</span><span class="sxs-lookup"><span data-stu-id="8ead7-116">Example 4: Search all content in OneDrive and SharePoint</span></span>

<span data-ttu-id="8ead7-117">Este exemplo consulta todo o conteúdo em OneDrive e SharePoint sites aos quais o usuário inscreveu tem acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="8ead7-117">This example queries all the content in OneDrive and SharePoint sites to which the signed-in user has read access.</span></span> <span data-ttu-id="8ead7-118">A **propriedade resource** na resposta retorna corresponde a arquivos e pastas como objetos **driveItem,** corresponde a contêineres (listas SharePoint) como lista e todas as outras combinações como **listItem**. </span><span class="sxs-lookup"><span data-stu-id="8ead7-118">The **resource** property in the response returns matches that are files and folders as **driveItem** objects, matches that are containers (SharePoint lists) as **list**, and all other matches as **listItem**.</span></span>

### <a name="request"></a><span data-ttu-id="8ead7-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ead7-119">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="8ead7-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ead7-120">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
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
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0",
                  "driveId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b",
                  "sharepointIds": {
                      "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                      "listItemId": "1027",
                      "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
                  }
                },
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

## <a name="example-5-use-filters-in-search-queries"></a><span data-ttu-id="8ead7-121">Exemplo 5: Usar filtros em consultas de pesquisa</span><span class="sxs-lookup"><span data-stu-id="8ead7-121">Example 5: Use filters in search queries</span></span>

<span data-ttu-id="8ead7-122">Você pode usar KQL em termos de pesquisa de consultas para OneDrive e SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8ead7-122">You can use KQL in search terms of queries for OneDrive and SharePoint.</span></span> <span data-ttu-id="8ead7-123">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="8ead7-123">For example:</span></span>

- <span data-ttu-id="8ead7-124">`"query": "contoso filetype:docx OR filetype:doc"` escopos da consulta para documentos do Word.</span><span class="sxs-lookup"><span data-stu-id="8ead7-124">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="8ead7-125">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` escopos da consulta para uma pasta específica dentro de um site.</span><span class="sxs-lookup"><span data-stu-id="8ead7-125">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>
- <span data-ttu-id="8ead7-126">`"query": "contoso AND isDocument=true"` escopos da consulta para retornar apenas documentos.</span><span class="sxs-lookup"><span data-stu-id="8ead7-126">`"query": "contoso AND isDocument=true"` scopes the query to only return documents.</span></span> <span data-ttu-id="8ead7-127">Qualquer contêiner (pasta, biblioteca de documentos) não será retornado.</span><span class="sxs-lookup"><span data-stu-id="8ead7-127">Any container (folder, document library) will not be returned.</span></span>
- <span data-ttu-id="8ead7-128">`"query": "contoso contentclass:STS_List_Events"`escopos da consulta para eventos calendar armazenados em SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8ead7-128">`"query": "contoso contentclass:STS_List_Events"` scopes the query to Calendar events stored in SharePoint.</span></span>
- <span data-ttu-id="8ead7-129">`"query": "contoso (LastModifiedTime > 2021-02-01 AND Created > 2021-02-01)"`escopos da consulta para filtrar SharePoint e OneDrive itens por data</span><span class="sxs-lookup"><span data-stu-id="8ead7-129">`"query": "contoso (LastModifiedTime > 2021-02-01 AND Created > 2021-02-01)"` scopes the query to filter SharePoint and OneDrive items by date</span></span>

<span data-ttu-id="8ead7-130">Para ser válida, a restrição de propriedades deve especificar um nome de propriedade gerenciada válido e queryable na condição.</span><span class="sxs-lookup"><span data-stu-id="8ead7-130">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

## <a name="example-6-specify-select-properties"></a><span data-ttu-id="8ead7-131">Exemplo 6: Especificar propriedades de seleção</span><span class="sxs-lookup"><span data-stu-id="8ead7-131">Example 6: Specify select properties</span></span>

<span data-ttu-id="8ead7-132">Você pode especificar os campos que deseja retornar na resposta, como parte da sub-propriedade **fields** de um [objeto searchHit](/graph/api/resources/searchhit) na resposta.</span><span class="sxs-lookup"><span data-stu-id="8ead7-132">You can specify the fields you want back in the response, as part of the **fields** sub-property of a [searchHit](/graph/api/resources/searchhit) object in the response.</span></span> <span data-ttu-id="8ead7-133">Essa é uma maneira de cortar a resposta sobre o fio ou solicitar algumas propriedades específicas que não fazem parte do esquema fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="8ead7-133">This is a way to either trim down the response over the wire, or to request some specific properties that are not part of the out-of-the-box schema.</span></span>

<span data-ttu-id="8ead7-134">Observe que a seleção de propriedades para propriedades personalizadas no SharePoint está disponível apenas para **listItem,** pois essa é a única entidade SharePoint no Microsoft Graph que oferece suporte a propriedades personalizadas.</span><span class="sxs-lookup"><span data-stu-id="8ead7-134">Note that property selection for custom properties in SharePoint is only available for **listItem** since this is the only SharePoint entity in Microsoft Graph that supports custom properties.</span></span>

<span data-ttu-id="8ead7-135">Para recuperar uma propriedade personalizada para **um driveItem**, **listItem de** consulta.</span><span class="sxs-lookup"><span data-stu-id="8ead7-135">To retrieve a custom property for a **driveItem**, query **listItem** instead.</span></span>

### <a name="request"></a><span data-ttu-id="8ead7-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ead7-136">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="8ead7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ead7-137">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
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
                "sharepointIds": {
                    "listId": "33498de0-d695-4d23-ac26-e1bf95a3206e",
                    "listItemId": "13"
                },
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

## <a name="known-limitations"></a><span data-ttu-id="8ead7-138">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="8ead7-138">Known limitations</span></span>

<span data-ttu-id="8ead7-139">Ao pesquisar a **unidade,** você precisa incluir na **consultaString** um termo contido no nome da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="8ead7-139">When searching for **drive**, you need to include in the **queryString** a term contained in the name of the document library.</span></span> <span data-ttu-id="8ead7-140">A consulta `*` não é suportada e não retorna todas as unidades disponíveis.</span><span class="sxs-lookup"><span data-stu-id="8ead7-140">Querying `*` is not supported and does not return all available drives.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8ead7-141">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8ead7-141">Next steps</span></span>

- [<span data-ttu-id="8ead7-142">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="8ead7-142">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview)
