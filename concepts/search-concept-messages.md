---
title: Pesquisar mensagens
description: A API de pesquisa da Microsoft permite que os aplicativos pesquisem informações em mensagens de email, retornem mensagens classificadas por relevância e processem uma experiência de pesquisa dedicada.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: d5dc6357bc6250b3964722114bd242e66871869a
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703930"
---
# <a name="search-messages"></a><span data-ttu-id="a91d3-103">Pesquisar mensagens</span><span class="sxs-lookup"><span data-stu-id="a91d3-103">Search messages</span></span>

<span data-ttu-id="a91d3-104">A API de pesquisa da Microsoft permite que os aplicativos pesquisem informações em mensagens de email, retornem mensagens classificadas por relevância e processem uma experiência de pesquisa dedicada.</span><span class="sxs-lookup"><span data-stu-id="a91d3-104">The Microsoft Search API lets apps search for information in email messages, return messages ranked by relevance, and render a dedicated search experience.</span></span> <span data-ttu-id="a91d3-105">A pesquisa se aplica ao corpo e aos anexos de mensagens na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a91d3-105">The search applies to the body and attachments of messages in the user's own mailbox.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="a91d3-106">Uma consulta de pesquisa pode incluir [filtros](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) que os usuários finais inserem na caixa de texto de **pesquisa** no Outlook.</span><span class="sxs-lookup"><span data-stu-id="a91d3-106">A search query can include [filters](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) that end users enter in the **Search** text box in Outlook.</span></span>

<span data-ttu-id="a91d3-107">Os resultados da pesquisa de mensagens são classificados por **receivedDateTime** em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="a91d3-107">Message search results are sorted by **receivedDateTime** in descending order.</span></span>

<span data-ttu-id="a91d3-108">A pesquisa de mensagens aplica-se às contas corporativas ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="a91d3-108">Message search applies to work or school accounts.</span></span> <span data-ttu-id="a91d3-109">Os usuários podem pesquisar sua própria caixa de correio, mas não em caixas de correio delegadas.</span><span class="sxs-lookup"><span data-stu-id="a91d3-109">Users can search their own mailbox, but not in delegated mailboxes.</span></span> <span data-ttu-id="a91d3-110">Confira mais [limitações conhecidas](#known-limitations) abaixo.</span><span class="sxs-lookup"><span data-stu-id="a91d3-110">See further [known limitations](#known-limitations) below.</span></span>

<span data-ttu-id="a91d3-111">A pesquisa de mensagens também procura anexos.</span><span class="sxs-lookup"><span data-stu-id="a91d3-111">Message search also looks for attachments.</span></span> <span data-ttu-id="a91d3-112">Os [tipos de arquivo com suporte para anexos](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) é o mesmo que para o SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="a91d3-112">The [file types supported for attachments](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) is the same as that for SharePoint Online.</span></span>

## <a name="examples"></a><span data-ttu-id="a91d3-113">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a91d3-113">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="a91d3-114">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="a91d3-114">Example 1</span></span>

<span data-ttu-id="a91d3-115">O exemplo a seguir consulta mensagens na caixa de correio do usuário conectado que contêm a cadeia de caracteres "contoso" em qualquer parte da mensagem (o nome do remetente, assunto, corpo da mensagem ou qualquer anexo).</span><span class="sxs-lookup"><span data-stu-id="a91d3-115">The following example queries messages in the signed-in user's mailbox that contain the string "contoso" in any part of the message (the sender name, subject, message body, or any attachments).</span></span> <span data-ttu-id="a91d3-116">A consulta retorna os 25 primeiros resultados.</span><span class="sxs-lookup"><span data-stu-id="a91d3-116">The query returns the first 25 results.</span></span> <span data-ttu-id="a91d3-117">Os resultados da pesquisa são ordenados por DateTime decrescente.</span><span class="sxs-lookup"><span data-stu-id="a91d3-117">The search results are ordered by Datetime descending.</span></span>

#### <a name="request"></a><span data-ttu-id="a91d3-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a91d3-118">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a91d3-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="a91d3-119">Response</span></span>

<span data-ttu-id="a91d3-120">Veja a seguir um exemplo da resposta que contém uma mensagem que corresponde ao critério de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a91d3-120">The following is an example of the response which contains one message that matches the search criterion.</span></span>

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

### <a name="example-2-search-top-results-messages"></a><span data-ttu-id="a91d3-121">Exemplo 2 principais mensagens de resultados de pesquisa</span><span class="sxs-lookup"><span data-stu-id="a91d3-121">Example 2 Search top results messages</span></span>

<span data-ttu-id="a91d3-122">O exemplo a seguir usa a mesma consulta de pesquisa que o [exemplo 1](#example-1)e classifica os resultados por relevância.</span><span class="sxs-lookup"><span data-stu-id="a91d3-122">The following example uses the same search query as [example 1](#example-1), and sorts the results by relevance.</span></span>

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a><span data-ttu-id="a91d3-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a91d3-123">Request</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="a91d3-124">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="a91d3-124">Known limitations</span></span>

- <span data-ttu-id="a91d3-125">Você só pode acessar a caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a91d3-125">You can only access a user’s own mailbox.</span></span> <span data-ttu-id="a91d3-126">Não há suporte para pesquisa de caixa de correio delegada</span><span class="sxs-lookup"><span data-stu-id="a91d3-126">Searching delegated mailbox is not supported</span></span>

- <span data-ttu-id="a91d3-127">Para mensagens, a propriedade **total** do tipo [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) contém o número de resultados na página, e não o número total de resultados correspondentes.</span><span class="sxs-lookup"><span data-stu-id="a91d3-127">For messages, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) type contains the number of results on the page, not the total number of matching results.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a91d3-128">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a91d3-128">Next steps</span></span>

<span data-ttu-id="a91d3-129">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="a91d3-129">Find out more about:</span></span>

- [<span data-ttu-id="a91d3-130">Usar a API de pesquisa</span><span class="sxs-lookup"><span data-stu-id="a91d3-130">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
