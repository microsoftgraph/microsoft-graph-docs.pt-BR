---
title: Usar a API do Microsoft Search no Microsoft Graph para pesquisar mensagens
description: Você pode usar a API de pesquisa da Microsoft para pesquisar informações em mensagens de email, devolver mensagens classificadas por relevância e renderizar uma experiência de pesquisa dedicada.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 978ce45b9882190a31e7840ba402d6eb283270dd
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332324"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-messages"></a>Usar a API do Microsoft Search no Microsoft Graph para pesquisar mensagens

Você pode usar a API de pesquisa da Microsoft para pesquisar informações em mensagens de email, devolver mensagens classificadas por relevância e renderizar uma experiência de pesquisa dedicada. A pesquisa se aplica ao corpo e aos anexos de mensagens na caixa de correio do usuário.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

Uma consulta de pesquisa pode incluir [filtros](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) que os usuários finais inserem na caixa de texto de **pesquisa** no Outlook.

Os resultados da pesquisa de mensagens são classificados por **receivedDateTime** em ordem decrescente.

A pesquisa de mensagens aplica-se às contas corporativas ou de estudante. Os usuários podem pesquisar sua própria caixa de correio, mas não podem pesquisar caixas de correio delegadas. Para obter detalhes, consulte [limitações conhecidas](#known-limitations).

A pesquisa de mensagens também procura anexos. Os [tipos de arquivo com suporte](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) para a pesquisa de anexo de mensagens são os mesmos que para a pesquisa do SharePoint Online.

## <a name="examples"></a>Exemplos

### <a name="example-1-search-messages-in-a-users-mailbox"></a>Exemplo 1: Pesquisar mensagens na caixa de correio de um usuário

O exemplo a seguir consulta mensagens na caixa de correio do usuário conectado que contêm a cadeia de caracteres "contoso" em qualquer parte da mensagem (o nome do remetente, assunto, corpo da mensagem ou qualquer anexo). A consulta retorna os 25 primeiros resultados. Os resultados da pesquisa são ordenados por **DateTime** decrescente.

#### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.message"
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

Veja a seguir um exemplo da resposta, que contém uma mensagem que corresponde ao critério de pesquisa. 

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
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "_id": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
              "_score": 1,
              "_sortField": "DateTime",
              "_summary": "Here is a summary of your messages from last week",
              "_source": {
                "@odata.type": "#microsoft.graph.message",
                "createdDateTime": "2019-10-07T10:00:08Z",
                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                "receivedDateTime": "2019-10-07T10:00:09Z",
                "sentDateTime": "2019-10-07T09:59:52Z",
                "hasAttachments": false,
                "subject": "Weekly digest: Office 365 changes",
                "bodyPreview": "Here is a summary of your messages from last week -   New Feature: Live captions in English-US a",
                "importance": "normal",
                "replyTo": [
                  {
                    "emailAddress": {
                      "name": "Goncalo Torres"
                    }
                  }
                ],
                "sender": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
                  }
                },
                "from": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
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

### <a name="example-2-search-top-results-messages"></a>Exemplo 2: Pesquisar mensagens de resultados principais
O exemplo a seguir usa a consulta de pesquisa mostrada no exemplo 1 e classifica os resultados por relevância. 

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.message"
      ],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 15,
      "enableTopResults": true
    }
  ]
}
```

## <a name="known-limitations"></a>Limitações conhecidas

- Você só pode acessar a caixa de correio de um usuário. Não há suporte para a pesquisa de caixas de correio delegadas.
- Para mensagens, a propriedade **total** do tipo [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) contém o número de resultados na página, e não o número total de resultados correspondentes.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de pesquisa da Microsoft](/graph/api/resources/search-api-overview?view=graph-rest-beta)
