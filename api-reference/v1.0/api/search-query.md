---
title: 'searchEntity: query'
description: Executa a consulta especificada no corpo da solicitação. Os resultados da pesquisa são fornecidos na resposta.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: e675b9b9301e7b0fc918c4631757a9bb21f82ce7
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983759"
---
# <a name="searchentity-query"></a><span data-ttu-id="51c33-104">searchEntity: query</span><span class="sxs-lookup"><span data-stu-id="51c33-104">searchEntity: query</span></span>

<span data-ttu-id="51c33-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51c33-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51c33-106">Executa a consulta especificada no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51c33-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="51c33-107">Os resultados da pesquisa são fornecidos na resposta.</span><span class="sxs-lookup"><span data-stu-id="51c33-107">Search results are provided in the response.</span></span>


## <a name="permissions"></a><span data-ttu-id="51c33-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="51c33-108">Permissions</span></span>

<span data-ttu-id="51c33-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51c33-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span> 

| <span data-ttu-id="51c33-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51c33-111">Permission type</span></span>                        | <span data-ttu-id="51c33-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51c33-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51c33-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51c33-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="51c33-114">Mail.Read, Mail.ReadWrite, Calendars.Read, Calendars.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All, ExternalItem.Read.All</span><span class="sxs-lookup"><span data-stu-id="51c33-114">Mail.Read, Mail.ReadWrite, Calendars.Read, Calendars.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="51c33-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51c33-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51c33-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51c33-116">Not supported.</span></span> |
| <span data-ttu-id="51c33-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51c33-117">Application</span></span>                            | <span data-ttu-id="51c33-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51c33-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51c33-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51c33-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="51c33-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51c33-120">Request headers</span></span>

| <span data-ttu-id="51c33-121">Nome</span><span class="sxs-lookup"><span data-stu-id="51c33-121">Name</span></span>          | <span data-ttu-id="51c33-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="51c33-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="51c33-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51c33-123">Authorization</span></span> | <span data-ttu-id="51c33-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51c33-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51c33-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="51c33-126">Content-type</span></span> | <span data-ttu-id="51c33-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51c33-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51c33-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51c33-129">Request body</span></span>

<span data-ttu-id="51c33-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51c33-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="51c33-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="51c33-131">Parameter</span></span>    | <span data-ttu-id="51c33-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="51c33-132">Type</span></span>        | <span data-ttu-id="51c33-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="51c33-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="51c33-134">requests</span><span class="sxs-lookup"><span data-stu-id="51c33-134">requests</span></span>|<span data-ttu-id="51c33-135">[Coleção searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="51c33-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="51c33-136">Uma coleção de uma ou mais solicitações de pesquisa cada formatada em um blob JSON.</span><span class="sxs-lookup"><span data-stu-id="51c33-136">A collection of one or more search requests each formatted in a JSON blob.</span></span> <span data-ttu-id="51c33-137">Cada blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de paging, os campos solicitados e a consulta de pesquisa real.</span><span class="sxs-lookup"><span data-stu-id="51c33-137">Each JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, requested fields, and actual search query.</span></span> <br> <span data-ttu-id="51c33-138">Esteja ciente das [limitações conhecidas](../resources/search-api-overview.md#known-limitations) em pesquisar combinações específicas de tipos de entidade e classificar ou agregar resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="51c33-138">Be aware of [known limitations](../resources/search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span> |

## <a name="response"></a><span data-ttu-id="51c33-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="51c33-139">Response</span></span>

<span data-ttu-id="51c33-140">Se bem-sucedido, este método retorna o código de resposta e um objeto da coleção `HTTP 200 OK` [searchResponse](../resources/searchresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51c33-140">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>
 

## <a name="examples"></a><span data-ttu-id="51c33-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="51c33-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51c33-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51c33-142">Request</span></span>

<span data-ttu-id="51c33-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51c33-143">The following is an example of the request.</span></span>

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-type: application/json

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

### <a name="response"></a><span data-ttu-id="51c33-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="51c33-144">Response</span></span>

<span data-ttu-id="51c33-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51c33-145">The following is an example of the response.</span></span>

> <span data-ttu-id="51c33-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51c33-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.searchResponse",
  "isCollection": true
} -->

```HTTP
HTTP/1.1 200 OK
Content-type: application/json
```

```json
{
    "value": [
        {
            "searchTerms": [
                "searchTerms-value"
            ],
            "hitsContainers": [
                {
                    "hits": [
                        {
                            "hitId": "AAMkADdmODdhN2NjLTMwZWYtNDBiNy1iMDYxLWZhZTkyOGM4YmRhZABGAAAAAACsLZF5BeQoRLYm4UlvnOXZBwCav2PZy/7/R52ssyzmS9f0AAAAAAEMAACav2PZy/7/R52ssyzmS9f0AABM0pr/AAA=",
                            "rank": 1,
                            "summary": "...Identity Protection Weekly Digest <c0>Contoso</c0> New risky users detected <https://azure.microsoft.com/email/?destination=https%3A%2F%2Fportal.azure.com%2Fcontoso.com%23blade%2FMicrosoft_AAD_IAM%2FIdentityProtectionMenuBlade%2FRiskyUsers%2F...",
                            "resource": {
                                "@odata.type": "#microsoft.graph.message",
                                "createdDateTime": "2020-11-17T16:02:34Z",
                                "lastModifiedDateTime": "2020-11-17T16:02:37Z",
                                "changeKey": "CQAAAA==",
                                "receivedDateTime": "2020-11-17T16:02:34Z",
                                "sentDateTime": "2020-11-17T16:02:27Z",
                                "hasAttachments": false,
                                "internetMessageId": "<1e506769-c6da-4f44-bb54-6ba1bd59d300@az.northcentralus.production.microsoft.com>",
                                "subject": "Azure AD Identity Protection Weekly Digest",
                                "bodyPreview": "...Identity Protection Weekly Digest Contoso New risky users detected <https://azure.microsoft.com/email/?destination=https%3A%2F%2Fportal.azure.com%2Fcontoso.com%23blade%2FMicrosoft_AAD_IAM%2FIdentityProtectionMenuBlade%2FRiskyUsers%2F...",
                                "importance": "normal",
                                "parentFolderId": "AQMkADdmODdhN2NjAC0zMGVmLTQwYjctYjA2MS1mYWU5MjhjOGJkYWQALgAAA6wtkXkF5ChEtibhSW+c5dkBAJq/Y9nL/v9HnayzLOZL1/QAAAIBDAAAAA==",
                                "conversationId": "AAQkADdmODdhN2NjLTMwZWYtNDBiNy1iMDYxLWZhZTkyOGM4YmRhZAAQAKQ6a/rTEmVCtGMTER183jw=",
                                "isRead": false,
                                "isDraft": false,
                                "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADdmODdhN2NjLTMwZWYtNDBiNy1iMDYxLWZhZTkyOGM4YmRhZABGAAAAAACsLZF5BeQoRLYm4UlvnOXZBwCav2PZy%2F7%2FR52ssyzmS9f0AAAAAAEMAACav2PZy%2F7%2FR52ssyzmS9f0AABM0pr%2FAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
                                "inferenceClassification": "focused",
                                "replyTo": [
                                    {
                                        "emailAddress": {
                                            "name": "MOD Administrator"
                                        }
                                    }
                                ],
                                "sender": {
                                    "emailAddress": {
                                        "name": "Microsoft Azure",
                                        "address": "azure-noreply@contoso.com"
                                    }
                                },
                                "from": {
                                    "emailAddress": {
                                        "name": "Microsoft Azure",
                                        "address": "azure-noreply@contoso.com"
                                    }
                                }
                            }
                        }
                    ],
                    "total": 47,
                    "moreResultsAvailable": true
                }
            ]
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="51c33-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="51c33-148">See also</span></span>
- <span data-ttu-id="51c33-149">Pesquisar [mensagens de email](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="51c33-149">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="51c33-150">Pesquisar [eventos de calendário](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="51c33-150">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="51c33-151">Pesquisar conteúdo no SharePoint e no OneDrive[(arquivos, listas e sites)](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="51c33-151">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="51c33-152">Pesquisar [dados de tipos personalizados (Conectores do Graph)](/graph/search-concept-custom-types)</span><span class="sxs-lookup"><span data-stu-id="51c33-152">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


