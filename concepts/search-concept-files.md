---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar arquivos
description: Você pode usar a API de pesquisa da Microsoft para pesquisar arquivos armazenados no SharePoint ou no OneDrive.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: a75eb8e90c8656ced3d9f50d6526b5ebe48584aa
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892671"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-files"></a>Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar arquivos

Você pode usar a API de pesquisa da Microsoft para pesquisar arquivos armazenados no SharePoint ou no OneDrive. A API do Microsoft Search usa um modelo de relevância que utiliza sinais do Microsoft Graph sobre as relações e atividades dos usuários. Isso permite que você retorne e promova o conteúdo que os usuários se preocupam, em uma experiência de pesquisa de arquivo consistente com a guia **arquivos** que lista os resultados da pesquisa no SharePoint.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="search-sharepoint-or-onedrive-files"></a>Pesquisar arquivos do SharePoint ou do OneDrive

Você pode usar o KQL em termos de pesquisa de consultas do SharePoint e do OneDrive. Por exemplo:

- `"query": "contoso filetype:docx OR filetype:doc"`escopo a consulta em documentos do Word.
- `"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`escopo a consulta para uma determinada pasta dentro de um site.

Para ser válido, a restrição de propriedades deve especificar um nome de propriedade gerenciada válido e consultável na condição.

### <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação

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

#### <a name="response"></a>Resposta

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

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta)
