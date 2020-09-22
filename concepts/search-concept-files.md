---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar arquivos
description: Você pode usar a API de pesquisa da Microsoft para pesquisar arquivos armazenados no OneDrive ou no SharePoint.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 38915d4ec4e38f5bd41e67e31d5708caf34272ec
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192537"
---
# <a name="use-the-microsoft-search-api-to-search-content-in-onedrive-and-sharepoint"></a>Usar a API de pesquisa da Microsoft para pesquisar conteúdo no OneDrive e no SharePoint

Use a API de pesquisa da Microsoft para pesquisar conteúdo armazenado no OneDrive ou no SharePoint: arquivos, pastas, listas, itens de lista ou sites.

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

A API de pesquisa permite que você escopo os tipos de conteúdo a serem recuperados no OneDrive ou no SharePoint especificando a propriedade **EntityTypes** no [searchRequest](/graph/api/resources/searchRequest?view=graph-rest-beta&preserve-view=true). A parte posterior deste artigo mostra alguns exemplos:

- [Exemplo 1: Arquivos de pesquisa](#example-1-search-files)
- [Exemplo 2: itens de lista de pesquisa](#example-2-search-list-items)
- [Exemplo 3: sites de pesquisa](#example-3-search-sites)
- [Exemplo 4: Pesquisar todo o conteúdo no OneDrive e no SharePoint](#example-4-search-all-content-in-onedrive-and-sharepoint)

## <a name="specify-select-properties"></a>Especificar propriedades de seleção

Você pode especificar os campos que deseja de volta na resposta, como parte da subpropriedade **Fields** de um objeto [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta&preserve-view=true) na resposta. Essa é uma maneira de aparar a resposta sobre o fio ou para solicitar algumas propriedades específicas que não fazem parte do esquema pronto para uso.

Observe que a seleção de propriedade só está disponível para **ListItem** , pois esta é a única entidade do SharePoint no Microsoft Graph que oferece suporte a propriedades personalizadas.

Para recuperar uma propriedade personalizada de um **driveItem**, procure **ListItem** .

### <a name="request"></a>Solicitação

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

### <a name="response"></a>Resposta

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

## <a name="use-filters-in-search-queries"></a>Usar filtros em consultas de pesquisa

Você pode usar o KQL em termos de pesquisa de consultas do OneDrive e do SharePoint. Por exemplo:

- `"query": "contoso filetype:docx OR filetype:doc"` escopo a consulta em documentos do Word.
- `"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` escopo a consulta para uma determinada pasta dentro de um site.
- `"query": "contoso AND isDocument=true"` escopos a consulta para retornar apenas os documentos. Qualquer contêiner (pasta, biblioteca de documentos) não será retornado.
- `"query": "contoso contentclass:STS_List_Events"` escopos a consulta para eventos de calendário armazenados no SharePoint.

Para ser válido, a restrição de propriedades deve especificar um nome de propriedade gerenciada válido e consultável na condição.

## <a name="example-1-search-files"></a>Exemplo 1: Arquivos de pesquisa

### <a name="request"></a>Solicitação

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

### <a name="response"></a>Resposta

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

## <a name="example-2-search-list-items"></a>Exemplo 2: itens de lista de pesquisa

### <a name="request"></a>Solicitação

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

### <a name="response"></a>Resposta

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

## <a name="example-3-search-sites"></a>Exemplo 3: sites de pesquisa

### <a name="request"></a>Solicitação

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

### <a name="response"></a>Resposta

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

## <a name="example-4-search-all-content-in-onedrive-and-sharepoint"></a>Exemplo 4: Pesquisar todo o conteúdo no OneDrive e no SharePoint

Este exemplo consulta todo o conteúdo de sites do OneDrive e do SharePoint aos quais o usuário conectado tem acesso de leitura. A propriedade **Resource** na resposta retorna correspondências que são arquivos e pastas como objetos **driveItem** , correspondências que são contêineres (listas do SharePoint) como **lista**e todas as outras correspondências como **ListItem**.

### <a name="request"></a>Solicitação

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

### <a name="response"></a>Resposta

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

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
