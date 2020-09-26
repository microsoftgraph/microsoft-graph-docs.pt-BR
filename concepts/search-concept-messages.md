---
title: Usar a API do Microsoft Search no Microsoft Graph para pesquisar mensagens
description: Você pode usar a API de pesquisa da Microsoft para pesquisar informações em mensagens de email, devolver mensagens classificadas por relevância e renderizar uma experiência de pesquisa dedicada.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: e9917b8153946161168e90f78399f29b6a7f3df3
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288823"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-messages"></a>Usar a API de pesquisa da Microsoft para pesquisar mensagens do Outlook

Use a API de pesquisa da Microsoft para pesquisar informações em mensagens de email, retornar mensagens classificadas por relevância e renderizar uma experiência de pesquisa dedicada. A pesquisa se aplica ao corpo e aos anexos de mensagens na caixa de correio do usuário conectado.

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

Uma consulta de pesquisa pode incluir [filtros](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) que os usuários finais inserem na caixa de texto de **pesquisa** no Outlook.

Os resultados da pesquisa de mensagens são classificados por **receivedDateTime** em ordem decrescente.

A pesquisa de mensagens aplica-se às contas corporativas ou de estudante. Os usuários podem pesquisar sua própria caixa de correio, mas não podem pesquisar caixas de correio delegadas. Para obter detalhes, consulte [limitações conhecidas](#known-limitations).

A pesquisa de mensagens também procura anexos. Os [tipos de arquivo com suporte](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) para a pesquisa de anexo de mensagens são os mesmos que para a pesquisa do SharePoint Online.

## <a name="example-1-search-messages-in-a-users-mailbox"></a>Exemplo 1: Pesquisar mensagens na caixa de correio de um usuário

O exemplo a seguir consulta mensagens na caixa de correio do usuário conectado que contêm a cadeia de caracteres "contoso" em qualquer parte da mensagem (o nome do remetente, assunto, corpo da mensagem ou qualquer anexo). A consulta retorna os 25 primeiros resultados. Os resultados da pesquisa são ordenados por **DateTime** decrescente.

### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "queryString": "contoso"
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta, que contém uma mensagem que corresponde ao critério de pesquisa.

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
              "hitId": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
              "rank": 1,
              "summary": "Here is a summary of your messages from last week",
              "resource": {
                "@odata.type": "#microsoft.graph.message",
                "createdDateTime": "2019-10-07T10:00:08Z",
                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                "receivedDateTime": "2019-10-07T10:00:09Z",
                "sentDateTime": "2019-10-07T09:59:52Z",
                "hasAttachments": false,
                "subject": "Weekly digest: Microsoft 365 changes",
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

## <a name="example-2-search-top-results-messages"></a>Exemplo 2: Pesquisar mensagens de resultados principais

O exemplo a seguir usa a consulta de pesquisa mostrada no exemplo 1 e classifica os resultados por relevância. 

<!-- markdownlint-disable MD024 -->
### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "queryString": "contoso"
      },
      "from": 0,
      "size": 15,
      "enableTopResults": true
    }
  ]
}
```

#### <a name="response"></a>Resposta
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
              "hitId": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
              "rank": 1,
              "summary": "Here is a summary of your messages from last week",
              "resource": {
                "@odata.type": "#microsoft.graph.message",
                "createdDateTime": "2019-10-07T10:00:08Z",
                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                "receivedDateTime": "2019-10-07T10:00:09Z",
                "sentDateTime": "2019-10-07T09:59:52Z",
                "hasAttachments": false,
                "subject": "Weekly digest: Microsoft 365 changes",
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

## <a name="known-limitations"></a>Limitações conhecidas

- Você pode acessar somente a caixa de correio do usuário conectado. Não há suporte para a pesquisa de caixas de correio delegadas.
- Para mensagens, a propriedade **total** do tipo [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta&preserve-view=true) contém o número de resultados na página, e não o número total de resultados correspondentes.
- A classificação de resultados não é suportada para eventos. Uma cláusula de classificação na solicitação retornará um código de erro de solicitação inválida na resposta.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de pesquisa da Microsoft](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)