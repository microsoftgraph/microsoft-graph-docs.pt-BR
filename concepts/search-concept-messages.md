---
title: Usar a API de Pesquisa da Microsoft para pesquisar mensagens do Outlook
description: Você pode usar a API de Pesquisa da Microsoft no Microsoft Graph para pesquisar informações em mensagens de email e retornar mensagens classificadas por relevância.
author: knightsu
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 1769bda3a6d4f4ed2fed6fc8294b7dc049749482
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436971"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-messages"></a>Usar a API de Pesquisa da Microsoft para pesquisar mensagens do Outlook

Use a API de Pesquisa da Microsoft no Microsoft Graph para pesquisar informações em mensagens de email, retornar mensagens classificadas por relevância e renderizar uma experiência de pesquisa dedicada. A pesquisa se aplica ao corpo e aos anexos de mensagens na própria caixa de correio do usuário conectado.

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

Uma consulta de pesquisa pode incluir [filtros que](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) os usuários finais inserem na **caixa de** texto Pesquisar no Outlook.

Os resultados da pesquisa de mensagens são classificados **por receivedDateTime** em ordem decrescente.

A pesquisa de mensagens se aplica a contas corporativas ou de estudante. Os usuários podem pesquisar sua própria caixa de correio, mas não podem pesquisar caixas de correio delegadas. Para obter detalhes, confira [as limitações conhecidas](#known-limitations).

A pesquisa de mensagens também procura anexos. Os [tipos de arquivo com suporte para](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) pesquisa de anexos de mensagem são os mesmos da pesquisa do SharePoint Online.

## <a name="example-1-search-messages-in-a-users-mailbox"></a>Exemplo 1: Pesquisar mensagens na caixa de correio de um usuário

O exemplo a seguir consulta mensagens na caixa de correio do usuário conectado que contêm a cadeia de caracteres "contoso" em qualquer parte da mensagem (o nome do remetente, assunto, corpo da mensagem ou qualquer anexo). A consulta retorna os primeiros 25 resultados. Os resultados da pesquisa são ordenados **em ordem decrescente por DateTime** .

### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
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

A seguir está um exemplo da resposta, que contém uma mensagem que corresponde ao critério de pesquisa.

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

## <a name="example-2-search-top-results-messages"></a>Exemplo 2: pesquisar mensagens de resultados principais

O exemplo a seguir usa a consulta de pesquisa mostrada no Exemplo 1 e classifica os resultados por relevância. 

<!-- markdownlint-disable MD024 -->
### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
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

- Você pode acessar apenas a própria caixa de correio do usuário conectado. Não há suporte para a pesquisa de caixas de correio delegadas.
- Para mensagens, a propriedade total do tipo [searchHitsContainer](/graph/api/resources/searchhitscontainer) contém o número de resultados na página, não o número **total** de resultados correspondentes.
- Não há suporte para a classificação de resultados em eventos. Uma cláusula de classificação na solicitação retornará um código de erro de Solicitação Incorreta na resposta.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview)
