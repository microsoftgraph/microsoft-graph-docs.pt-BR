---
title: Tipos personalizados de pesquisa
description: A API de consulta permite pesquisar entre tipos personalizados ingeridos por meio da API de indexação.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: d4381529d66eaae19d9866eeb594201cec115735
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939562"
---
# <a name="search-custom-types-externalitem"></a>Tipos personalizados de pesquisa (externalItem)

A API do Microsoft Search permite que você importe dados externos por meio do recurso [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) e execute consultas de pesquisa nesse conteúdo externo.

Para Pesquisar tipos personalizados, especifique o seguinte no corpo da solicitação do método de [consulta](/graph/api/search-query?view=graph-rest-beta) :

- A propriedade **ContentSources** para incluir a ID de conexão atribuída durante a configuração do conector

- A propriedade **EntityType** como`externalItem`

- A propriedade **stored_fields** para incluir os campos no item externo que você deseja recuperar

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.externalItem"],
       "contentSources": ["/external/connections/servicenow-connector-contoso"],
       "query": {
        "query_string": {
          "query": "contoso tickets"
        }
      },
      "from": 0,
      "size": 25,
    "stored_fields": [
        "title",
        "priority",
        "description"
       ]
    }
  ]
}
```
### <a name="response"></a>Resposta

Resposta

```Json
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


## <a name="known-limitations"></a>Limitações conhecidas

- Tipos personalizados não dão suporte à pesquisa em várias fontes (especificado em **ContentSources**). Você pode pesquisar apenas uma conexão por vez.

- Você deve especificar a propriedade **stored_fields** , caso contrário os resultados da pesquisa não serão retornados.

## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Usar a API de pesquisa](/graph/api/resources/search-api-overview?view=graph-rest-beta)