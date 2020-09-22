---
title: Usar a API do Microsoft Search no Microsoft Graph para pesquisar mensagens
description: Você pode usar a API de pesquisa da Microsoft para pesquisar informações em mensagens de email, devolver mensagens classificadas por relevância e renderizar uma experiência de pesquisa dedicada.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 439a6ca1d560a848a0e78b2105dc717abfa5ad44
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192552"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-messages"></a><span data-ttu-id="92984-103">Usar a API de pesquisa da Microsoft para pesquisar mensagens do Outlook</span><span class="sxs-lookup"><span data-stu-id="92984-103">Use the Microsoft Search API to search Outlook messages</span></span>

<span data-ttu-id="92984-104">Use a API de pesquisa da Microsoft para pesquisar informações em mensagens de email, retornar mensagens classificadas por relevância e renderizar uma experiência de pesquisa dedicada.</span><span class="sxs-lookup"><span data-stu-id="92984-104">Use the Microsoft Search API to search for information in email messages, return messages ranked by relevance, and render a dedicated search experience.</span></span> <span data-ttu-id="92984-105">A pesquisa se aplica ao corpo e aos anexos de mensagens na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="92984-105">The search applies to the body and attachments of messages in the signed-in user's own mailbox.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="92984-106">Uma consulta de pesquisa pode incluir [filtros](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) que os usuários finais inserem na caixa de texto de **pesquisa** no Outlook.</span><span class="sxs-lookup"><span data-stu-id="92984-106">A search query can include [filters](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) that end users enter in the **Search** text box in Outlook.</span></span>

<span data-ttu-id="92984-107">Os resultados da pesquisa de mensagens são classificados por **receivedDateTime** em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="92984-107">Message search results are sorted by **receivedDateTime** in descending order.</span></span>

<span data-ttu-id="92984-108">A pesquisa de mensagens aplica-se às contas corporativas ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="92984-108">Message search applies to work or school accounts.</span></span> <span data-ttu-id="92984-109">Os usuários podem pesquisar sua própria caixa de correio, mas não podem pesquisar caixas de correio delegadas.</span><span class="sxs-lookup"><span data-stu-id="92984-109">Users can search their own mailbox, but can't search delegated mailboxes.</span></span> <span data-ttu-id="92984-110">Para obter detalhes, consulte [limitações conhecidas](#known-limitations).</span><span class="sxs-lookup"><span data-stu-id="92984-110">For details, see [known limitations](#known-limitations).</span></span>

<span data-ttu-id="92984-111">A pesquisa de mensagens também procura anexos.</span><span class="sxs-lookup"><span data-stu-id="92984-111">Message search also looks for attachments.</span></span> <span data-ttu-id="92984-112">Os [tipos de arquivo com suporte](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) para a pesquisa de anexo de mensagens são os mesmos que para a pesquisa do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="92984-112">The [supported file types](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) for message attachment search are the same as those for SharePoint Online search.</span></span>

## <a name="example-1-search-messages-in-a-users-mailbox"></a><span data-ttu-id="92984-113">Exemplo 1: Pesquisar mensagens na caixa de correio de um usuário</span><span class="sxs-lookup"><span data-stu-id="92984-113">Example 1: Search messages in a user's mailbox</span></span>

<span data-ttu-id="92984-114">O exemplo a seguir consulta mensagens na caixa de correio do usuário conectado que contêm a cadeia de caracteres "contoso" em qualquer parte da mensagem (o nome do remetente, assunto, corpo da mensagem ou qualquer anexo).</span><span class="sxs-lookup"><span data-stu-id="92984-114">The following example queries messages in the signed-in user's mailbox that contain the string "contoso" in any part of the message (the sender name, subject, message body, or any attachments).</span></span> <span data-ttu-id="92984-115">A consulta retorna os 25 primeiros resultados.</span><span class="sxs-lookup"><span data-stu-id="92984-115">The query returns the first 25 results.</span></span> <span data-ttu-id="92984-116">Os resultados da pesquisa são ordenados por **DateTime** decrescente.</span><span class="sxs-lookup"><span data-stu-id="92984-116">The search results are ordered by **DateTime** descending.</span></span>

### <a name="request"></a><span data-ttu-id="92984-117">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92984-117">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="92984-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="92984-118">Response</span></span>

<span data-ttu-id="92984-119">Veja a seguir um exemplo da resposta, que contém uma mensagem que corresponde ao critério de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="92984-119">The following is an example of the response, which contains one message that matches the search criterion.</span></span>

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

## <a name="example-2-search-top-results-messages"></a><span data-ttu-id="92984-120">Exemplo 2: Pesquisar mensagens de resultados principais</span><span class="sxs-lookup"><span data-stu-id="92984-120">Example 2: Search top results messages</span></span>

<span data-ttu-id="92984-121">O exemplo a seguir usa a consulta de pesquisa mostrada no exemplo 1 e classifica os resultados por relevância.</span><span class="sxs-lookup"><span data-stu-id="92984-121">The following example uses the search query shown in Example 1, and sorts the results by relevance.</span></span> 

<!-- markdownlint-disable MD024 -->
### <a name="request"></a><span data-ttu-id="92984-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92984-122">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="92984-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="92984-123">Response</span></span>
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

## <a name="known-limitations"></a><span data-ttu-id="92984-124">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="92984-124">Known limitations</span></span>

- <span data-ttu-id="92984-125">Você pode acessar somente a caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="92984-125">You can access only the signed-in user’s own mailbox.</span></span> <span data-ttu-id="92984-126">Não há suporte para a pesquisa de caixas de correio delegadas.</span><span class="sxs-lookup"><span data-stu-id="92984-126">Searching delegated mailboxes is not supported.</span></span>
- <span data-ttu-id="92984-127">Para mensagens, a propriedade **total** do tipo [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta&preserve-view=true) contém o número de resultados na página, e não o número total de resultados correspondentes.</span><span class="sxs-lookup"><span data-stu-id="92984-127">For messages, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta&preserve-view=true) type contains the number of results on the page, not the total number of matching results.</span></span>
- <span data-ttu-id="92984-128">A classificação de resultados não é suportada para eventos.</span><span class="sxs-lookup"><span data-stu-id="92984-128">Sorting results is not supported for events.</span></span> <span data-ttu-id="92984-129">Uma cláusula de classificação na solicitação retornará um código de erro de solicitação inválida na resposta.</span><span class="sxs-lookup"><span data-stu-id="92984-129">A sort clause in the request will return a Bad Request error code in the response.</span></span>

## <a name="next-steps"></a><span data-ttu-id="92984-130">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="92984-130">Next steps</span></span>

- [<span data-ttu-id="92984-131">Usar a API de pesquisa da Microsoft</span><span class="sxs-lookup"><span data-stu-id="92984-131">Use the Microsoft Search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
