---
title: Arquivos de pesquisa (incluindo externalfile)
description: A API de consulta permite que você pesquise entre arquivos (DriveItem ou arquivos externos).
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: e34816e56872830cdb3b8ac524293d21588a5d9f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939548"
---
# <a name="search-files-including-externalfile"></a>Arquivos de pesquisa (incluindo externalfile)

A API do Microsoft Search permite pesquisar arquivos armazenados no SharePoint ou no OneDrive. Ele usa um modelo de relevância que utiliza sinais do Microsoft Graph sobre as relações e atividades dos usuários. Isso permite retornar e promover o conteúdo com o qual os usuários se preocupam, em uma experiência de pesquisa de arquivo consistente com a guia **arquivos** que lista os resultados da pesquisa no SharePoint. 

Além disso, a API pode trazer arquivos externos expostos por meio do recurso [externalfile](/graph/api/resources/externalfile?view=graph-rest-beta) .


## <a name="search-sharepoint-or-onedrive-files"></a>Pesquisar arquivos do SharePoint ou do OneDrive

Você pode usar o KQL em termos de pesquisa de consultas do SharePoint e do OneDrive. Por exemplo:

- "consulta": "o tipo de arquivo contoso: docx ou filetype: doc" pesquisa de escopo em documentos do Word
- "Query": "caminho do teste\\:https://contoso.sharepoint.com/sites/Team " site/documentos/\\projeto "" escopo a consulta para uma pasta específica dentro de um site.

Para ser válido, a restrição de propriedades deve especificar um nome de propriedade gerenciada válido Consultád na condição.

### <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação

```HTTP
POST /search/query
Content-Type: application/json
```

```Json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.driveItem"],
       "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25,
    }
  ]
}
```

#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!---TODO nmoreau team Include one example of externalItem response.-->
```Json
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
                      },
                      {
                      }
                  ]
              }
          ]
      }
  ]
}
```

## <a name="search-external-files-well-known-types"></a>Pesquisar arquivos externos (tipos bem conhecidos)

O [conector de compartilhamento de arquivos](/MicrosoftSearch/file-share-connector) é um conector "pronto para uso" disponível no Microsoft Search. Permite indexar arquivos disponíveis em um compartilhamento de arquivos. Você pode usar a API de consulta para consultar todos os arquivos externos.

### <a name="example"></a>Exemplo
O exemplo a seguir retorna todos os conectores externalfile configurados para o locatário e classifica os resultados por relevância.

#### <a name="request"></a>Solicitação

```HTTP
POST /search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.externalFile"],
       "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25,
    }
  ]
}
```

#### <a name="response"></a>Resposta

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
    "value": [{
        "searchTerms": [
            "contoso"
        ],
        "hitsContainers": [{
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
                            "url": "file://fileshare01/External Presentations/Contoso-Overview.pptx",
                            }
                     }
                     ,
                     {
                            ///Another searchHit
                     }
            ]
        }]
    }]
}
```

## <a name="search-all-files-including-externalfile-instances"></a>Pesquisar todos os arquivos (incluindo instâncias de arquivos externos)

Você pode pesquisar todos os arquivos de um locatário, incluindo o [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) e todos os arquivos externos, especificando dois tipos de entidade na solicitação de pesquisa.

A resposta fornece uma mistura de instâncias **driveItem** e externalItem no `_sources` campo de cada objeto [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta) .

### <a name="example"></a>Exemplo

O exemplo a seguir retorna todos os conectores **externos** defile e objetos **driveItem** do locatário que satisfazem os termos de pesquisa. Ele classifica os resultados por relevância.

### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.driveItem","microsoft.graph.externalFile"],
       "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25,
    }
  ]
}
```

## <a name="known-limitations"></a>Limitações conhecidas

Você não pode fazer o escopo de uma consulta para uma ConnectionID específica.

## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Usar a API de pesquisa](/graph/api/resources/search-api-overview?view=graph-rest-beta)