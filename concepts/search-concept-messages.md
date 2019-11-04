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
# <a name="search-messages"></a><span data-ttu-id="8cef8-103">Mensagens de pesquisa</span><span class="sxs-lookup"><span data-stu-id="8cef8-103">Search messages</span></span>

<span data-ttu-id="8cef8-104">A API de pesquisa da Microsoft permite que os aplicativos pesquisem informações em mensagens de email, retornem mensagens classificadas por relevância e processem uma experiência de pesquisa dedicada.</span><span class="sxs-lookup"><span data-stu-id="8cef8-104">The Microsoft Search API lets apps search for information in email messages, return messages ranked by relevance, and render a dedicated search experience.</span></span> <span data-ttu-id="8cef8-105">A pesquisa se aplica ao corpo e aos anexos de mensagens na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8cef8-105">The search applies to the body and attachments of messages in the user's own mailbox.</span></span> 

<span data-ttu-id="8cef8-106">Uma consulta de pesquisa pode incluir [filtros](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) que os usuários finais inserem na caixa de texto de **pesquisa** no Outlook.</span><span class="sxs-lookup"><span data-stu-id="8cef8-106">A search query can include [filters](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) that end users enter in the **Search** text box in Outlook.</span></span>

<span data-ttu-id="8cef8-107">Os resultados da pesquisa de mensagens são classificados por **receivedDateTime** em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="8cef8-107">Message search results are sorted by **receivedDateTime** in descending order.</span></span>

<span data-ttu-id="8cef8-108">No momento, a pesquisa de mensagens aplica-se apenas às contas pessoais dos usuários, mas não às contas corporativas ou de estudante, e não às caixas de correio delegadas.</span><span class="sxs-lookup"><span data-stu-id="8cef8-108">Currently, message search applies to only users' own personal accounts, but not work or school accounts, and not in delegated mailboxes.</span></span> <span data-ttu-id="8cef8-109">Confira mais [limitações conhecidas](#known-limitations) abaixo.</span><span class="sxs-lookup"><span data-stu-id="8cef8-109">See further [known limitations](#known-limitations) below.</span></span>

## <a name="examples"></a><span data-ttu-id="8cef8-110">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8cef8-110">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="8cef8-111">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="8cef8-111">Example 1</span></span>

<span data-ttu-id="8cef8-112">O exemplo a seguir consulta mensagens na caixa de correio do usuário conectado que contêm a cadeia de caracteres "contoso" em qualquer parte da mensagem (o nome do remetente, assunto, corpo da mensagem ou qualquer anexo).</span><span class="sxs-lookup"><span data-stu-id="8cef8-112">The following example queries messages in the signed-in user's mailbox that contain the string "contoso" in any part of the message (the sender name, subject, message body, or any attachments).</span></span> <span data-ttu-id="8cef8-113">A consulta retorna os 25 primeiros resultados.</span><span class="sxs-lookup"><span data-stu-id="8cef8-113">The query returns the first 25 results.</span></span> <span data-ttu-id="8cef8-114">Os resultados da pesquisa são ordenados por DateTime decrescente.</span><span class="sxs-lookup"><span data-stu-id="8cef8-114">The search results are ordered by Datetime descending.</span></span>

#### <a name="request"></a><span data-ttu-id="8cef8-115">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cef8-115">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="8cef8-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cef8-116">Response</span></span> 

<span data-ttu-id="8cef8-117">Veja a seguir um exemplo da resposta que contém uma mensagem que corresponde ao critério de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8cef8-117">The following is an example of the response which contains one message that matches the search criterion.</span></span> 

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

### <a name="example-2-search-top-results-messages"></a><span data-ttu-id="8cef8-118">Exemplo 2 principais mensagens de resultados de pesquisa</span><span class="sxs-lookup"><span data-stu-id="8cef8-118">Example 2 Search top results messages</span></span>
<span data-ttu-id="8cef8-119">O exemplo a seguir usa a mesma consulta de pesquisa que o [exemplo 1](#example-1)e classifica os resultados por relevância.</span><span class="sxs-lookup"><span data-stu-id="8cef8-119">The following example uses the same search query as [example 1](#example-1), and sorts the results by relevance.</span></span> 

#### <a name="request"></a><span data-ttu-id="8cef8-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cef8-120">Request</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="8cef8-121">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="8cef8-121">Known limitations</span></span>

- <span data-ttu-id="8cef8-122">Você só pode acessar a caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8cef8-122">You can only access a user’s own mailbox.</span></span> <span data-ttu-id="8cef8-123">Não há suporte para pesquisa de caixa de correio delegada</span><span class="sxs-lookup"><span data-stu-id="8cef8-123">Searching delegated mailbox is not supported</span></span> 

- <span data-ttu-id="8cef8-124">Para mensagens, a propriedade **total** do tipo [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) contém o número de resultados na página, e não o número total de resultados correspondentes.</span><span class="sxs-lookup"><span data-stu-id="8cef8-124">For messages, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) type contains the number of results on the page, not the total number of matching results.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8cef8-125">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8cef8-125">Next steps</span></span>

<span data-ttu-id="8cef8-126">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="8cef8-126">Find out more about:</span></span>

- [<span data-ttu-id="8cef8-127">Usar a API de pesquisa</span><span class="sxs-lookup"><span data-stu-id="8cef8-127">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
