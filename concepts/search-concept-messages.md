---
title: Usar a API Pesquisa da Microsoft no Microsoft Graph para pesquisar mensagens
description: Você pode usar a API Pesquisa da Microsoft para pesquisar informações em mensagens de email, retornar mensagens classificadas por relevância e renderizar uma experiência de pesquisa dedicada.
author: knightsu
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: a4dadd4db51acf2e99e69d4d206526100187ba27
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59103932"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-messages"></a>Usar a API Pesquisa da Microsoft para pesquisar Outlook mensagens

Use a API Pesquisa da Microsoft para pesquisar informações em mensagens de email, retornar mensagens classificadas por relevância e renderizar uma experiência de pesquisa dedicada. A pesquisa se aplica ao corpo e aos anexos de mensagens na própria caixa de correio do usuário inscreveu.

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

Uma consulta de pesquisa pode incluir [filtros](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) que os usuários finais insiram na caixa **de texto Pesquisar** Outlook.

Os resultados da pesquisa de mensagens são organizados **por receivedDateTime** em ordem decrescente.

A pesquisa de mensagens se aplica a contas de trabalho ou de estudante. Os usuários podem pesquisar suas próprias caixas de correio, mas não podem pesquisar caixas de correio delegadas. Para obter detalhes, consulte [limitações conhecidas](#known-limitations).

A pesquisa de mensagens também procura por anexos. Os [tipos de arquivo com suporte para](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) pesquisa de anexos de mensagens são os mesmos da pesquisa SharePoint Online.

## <a name="example-1-search-messages-in-a-users-mailbox"></a>Exemplo 1: Pesquisar mensagens na caixa de correio de um usuário

O exemplo a seguir consulta mensagens na caixa de correio do usuário que contém a cadeia de caracteres "contoso" em qualquer parte da mensagem (o nome do remetente, assunto, corpo da mensagem ou quaisquer anexos). A consulta retorna os primeiros 25 resultados. Os resultados da pesquisa são ordenados **pela decrescente DateTime.**

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

A seguir, um exemplo da resposta, que contém uma mensagem que corresponde ao critério de pesquisa.

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

## <a name="example-2-search-top-results-messages"></a>Exemplo 2: Pesquisar mensagens de resultados principais

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

#### <a name="response"></a>Resposta
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

- Você pode acessar apenas a própria caixa de correio do usuário interno. Não há suporte para pesquisar caixas de correio delegadas.
- Para mensagens, a **propriedade total** do [tipo searchHitsContainer](/graph/api/resources/searchhitscontainer) contém o número de resultados na página, não o número total de resultados correspondentes.
- A classificação de resultados não é suportada para eventos. Uma cláusula de classificação na solicitação retornará um código de erro de Solicitação Inoposta na resposta.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API Pesquisa da Microsoft de usuário](/graph/api/resources/search-api-overview)
