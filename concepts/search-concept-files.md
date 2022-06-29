---
title: Usar a API de Pesquisa da Microsoft para pesquisar o conteúdo do OneDrive e do SharePoint
description: 'Use a API de Pesquisa da Microsoft no Microsoft Graph para pesquisar conteúdo armazenado no OneDrive ou no SharePoint: arquivos, pastas, listas, itens de lista ou sites.'
author: nmoreau
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: a4730bb9c959ee5cb27514cd27b890c4bcb2c095
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445843"
---
# <a name="use-the-microsoft-search-api-to-search-onedrive-and-sharepoint-content"></a>Usar a API de Pesquisa da Microsoft para pesquisar o conteúdo do OneDrive e do SharePoint

Use a API de Pesquisa da Microsoft no Microsoft Graph para pesquisar conteúdo armazenado no OneDrive ou no SharePoint: arquivos, pastas, listas, itens de lista ou sites.

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

A API de Pesquisa permite definir o escopo dos tipos de conteúdo a serem recuperados no OneDrive ou no SharePoint especificando a propriedade **entityTypes** na [searchRequest](/graph/api/resources/searchRequest). Este artigo descreve alguns exemplos.

## <a name="example-1-search-files"></a>Exemplo 1: Arquivos de pesquisa

### <a name="request"></a>Solicitação

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

### <a name="response"></a>Resposta

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

## <a name="example-2-search-list-items"></a>Exemplo 2: Pesquisar itens de lista

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

## <a name="example-4-search-all-content-in-onedrive-and-sharepoint"></a>Exemplo 4: Pesquisar todo o conteúdo no OneDrive e no SharePoint

Este exemplo consulta todo o conteúdo nos sites do OneDrive e do SharePoint aos quais o usuário conectado tem acesso de leitura. **A propriedade** de recurso na resposta retorna as correspondentes que são arquivos e pastas como objetos **driveItem**, correspondentes que são contêineres (listas do SharePoint) como lista e todas as outras corresponde como **listItem**.

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

## <a name="example-5-use-filters-in-search-queries"></a>Exemplo 5: Usar filtros em consultas de pesquisa

Você pode usar o KQL em termos de pesquisa de consultas para o OneDrive e o SharePoint. Por exemplo:

- `"query": "contoso filetype:docx OR filetype:doc"` o escopo da consulta para documentos do Word.
- `"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\""` O  define o escopo da consulta para uma pasta específica dentro de um site.
- `"query": "contoso AND isDocument=true"` O  escopos da consulta para retornar apenas documentos. Nenhum contêiner (pasta, biblioteca de documentos) será retornado.
- `"query": "contoso contentclass:STS_List_Events"` O  define o escopo da consulta para eventos de Calendário armazenados no SharePoint.
- `"query": "contoso (LastModifiedTime > 2021-02-01 AND Created > 2021-02-01)"` escopos da consulta para filtrar itens do SharePoint e do OneDrive por data

Para ser válida, a restrição de propriedades deve especificar um nome de propriedade gerenciado válido e que pode ser consultado na condição.

## <a name="example-6-specify-select-properties"></a>Exemplo 6: especificar propriedades de seleção

Você pode especificar os campos desejados de volta na resposta, como parte da sub-propriedade **fields** de um [objeto searchHit](/graph/api/resources/searchhit) na resposta. Essa é uma maneira de cortar a resposta pela transmissão ou solicitar algumas propriedades específicas que não fazem parte do esquema inicial.

Observe que a seleção de propriedades personalizadas no SharePoint só está disponível para **listItem** , pois essa é a única entidade do SharePoint no Microsoft Graph que dá suporte a propriedades personalizadas.

Para recuperar uma propriedade personalizada para um **driveItem**, consulte **listItem** .

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

## <a name="known-limitations"></a>Limitações conhecidas

Ao pesquisar a **unidade**, você precisa incluir na **queryString** um termo contido no nome da biblioteca de documentos. Não há suporte `*` para a consulta e não retorna todas as unidades disponíveis.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview)
