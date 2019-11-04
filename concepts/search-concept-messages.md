---
title: Mensagens de pesquisa
description: A API de pesquisa da Microsoft permite que os aplicativos pesquisem informações em mensagens de email, retornem mensagens classificadas por relevância e processem uma experiência de pesquisa dedicada.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: f78ad8af81a7d2b72ab61914cc441db279913dc1
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939541"
---
# <a name="search-messages"></a>Mensagens de pesquisa

A API de pesquisa da Microsoft permite que os aplicativos pesquisem informações em mensagens de email, retornem mensagens classificadas por relevância e processem uma experiência de pesquisa dedicada. A pesquisa se aplica ao corpo e aos anexos de mensagens na caixa de correio do usuário. 

Uma consulta de pesquisa pode incluir [filtros](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) que os usuários finais inserem na caixa de texto de **pesquisa** no Outlook.

Os resultados da pesquisa de mensagens são classificados por **receivedDateTime** em ordem decrescente.

No momento, a pesquisa de mensagens aplica-se apenas às contas pessoais dos usuários, mas não às contas corporativas ou de estudante, e não às caixas de correio delegadas. Confira mais [limitações conhecidas](#known-limitations) abaixo.

## <a name="examples"></a>Exemplos

### <a name="example-1"></a>Exemplo 1

O exemplo a seguir consulta mensagens na caixa de correio do usuário conectado que contêm a cadeia de caracteres "contoso" em qualquer parte da mensagem (o nome do remetente, assunto, corpo da mensagem ou qualquer anexo). A consulta retorna os 25 primeiros resultados. Os resultados da pesquisa são ordenados por DateTime decrescente.

#### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [{
      "entityTypes": ["microsoft.graph.message"],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

#### <a name="response"></a>Resposta 

Veja a seguir um exemplo da resposta que contém uma mensagem que corresponde ao critério de pesquisa. 

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
    "value": [
        {
            "searchTerms": [
                "contoso"
            ],
            "hitsContainers": [
                {
                    "total": 1,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "_id": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
                            "_score": 1,
                            "_sortField": "DateTime",
                            "_summary": "Here is a summary of your messages from last week",
                            "_source": {
                                "@odata.type": "#microsoft.graph.message",
                                "createdDateTime": "2019-10-07T10:00:08Z",
                                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                                "receivedDateTime": "2019-10-07T10:00:09Z",
                                "sentDateTime": "2019-10-07T09:59:52Z",
                                "hasAttachments": false,
                                "subject": "Weekly digest: Office 365 changes",
                                "bodyPreview": "Here is a summary of your messages from last week -   New Feature: Live captions in English-US a",
                                "importance": "normal",
                                "replyTo": [
                                    {
                                        "emailAddress": {
                                            "name": "Goncalo Torres"
                                        }
                                    }
                                ],
                                "sender": {
                                    "emailAddress": {
                                        "name": "Office365 Message Center",
                                        "address": "gtorres@contoso.com"
                                    }
                                },
                                "from": {
                                    "emailAddress": {
                                        "name": "Office365 Message Center",
                                        "address": "gtorres@contoso.com",
                                    }
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

### <a name="example-2-search-top-results-messages"></a>Exemplo 2 principais mensagens de resultados de pesquisa
O exemplo a seguir usa a mesma consulta de pesquisa que o [exemplo 1](#example-1)e classifica os resultados por relevância. 

#### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
    "requests": [{
        "entityTypes": ["microsoft.graph.message"],
        "query": {
            "query_string": {
                "query": "contoso"
            }
        },
        "from": 0,
        "size": 15,
        "enableTopResults": true
    }]
}
```

## <a name="known-limitations"></a>Limitações conhecidas

- Você só pode acessar a caixa de correio de um usuário. Não há suporte para pesquisa de caixa de correio delegada 

- Para mensagens, a propriedade **total** do tipo [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) contém o número de resultados na página, e não o número total de resultados correspondentes.

## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Usar a API de pesquisa](/graph/api/resources/search-api-overview?view=graph-rest-beta)
