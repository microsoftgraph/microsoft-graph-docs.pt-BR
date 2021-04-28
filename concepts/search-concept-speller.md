---
title: Usar a API de Pesquisa da Microsoft no Microsoft Graph para solicitar correções ortográficas
description: Você pode usar a API de Pesquisa da Microsoft para obter a sugestão ortográfica ou a modificação ortográfica para a consulta de pesquisa.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 9d7f935f2de7e0777679266fc479b302fcfaf2a9
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067660"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-request-spelling-correction-preview"></a><span data-ttu-id="531c7-103">Use a API de Pesquisa da Microsoft no Microsoft Graph para solicitar correção ortográfica (visualização)</span><span class="sxs-lookup"><span data-stu-id="531c7-103">Use the Microsoft Search API in Microsoft Graph to request spelling correction (preview)</span></span>

<span data-ttu-id="531c7-104">Você pode usar a API de Pesquisa da Microsoft para solicitar correções ortográficas para lidar com incompatibilidades entre erros de digitação em consultas do usuário e palavras corretas em conteúdos matched.</span><span class="sxs-lookup"><span data-stu-id="531c7-104">You can use the Microsoft Search API to request spelling corrections to handle mismatches between typos in user queries and correct words in matched contents.</span></span> <span data-ttu-id="531c7-105">Para solicitar correções ortográficas, especifique as seguintes propriedades na **propriedade queryAlterationOptions** do corpo da solicitação do [método de](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) consulta:</span><span class="sxs-lookup"><span data-stu-id="531c7-105">To request spelling corrections, specify the following properties in the **queryAlterationOptions** property of request body of the [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) method:</span></span>

- <span data-ttu-id="531c7-106">**enableSuggestion** to enable/disable spelling suggestions for the user query.</span><span class="sxs-lookup"><span data-stu-id="531c7-106">**enableSuggestion** to enable/disable spelling suggestions for the user query.</span></span> <span data-ttu-id="531c7-107">Você pode passar `true` para obter as informações de correção ortográfica sugeridas para erros de digitação na consulta do usuário.</span><span class="sxs-lookup"><span data-stu-id="531c7-107">You can pass `true` to get the suggested spelling correction information for typos in the user query.</span></span>

- <span data-ttu-id="531c7-108">**enableModification** para habilitar/desabilitar modificações ortográficas para a consulta do usuário.</span><span class="sxs-lookup"><span data-stu-id="531c7-108">**enableModification** to enable/disable spelling modifications for the user query.</span></span> <span data-ttu-id="531c7-109">Você pode passar para obter os resultados da pesquisa para a consulta corrigida quando não houver resultados para a consulta original com erros de digitação e obter as informações de `true` correção correspondentes. </span><span class="sxs-lookup"><span data-stu-id="531c7-109">You can pass `true` to get the search results for the corrected query *when there are no results* for the original query with typos, and get the corresponding correction information.</span></span>

<span data-ttu-id="531c7-110">A prioridade da modificação ortográfica é maior do que a sugestão ortográfica se ambas estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="531c7-110">The priority of spelling modification is higher than spelling suggestion if they are both enabled.</span></span>

<span data-ttu-id="531c7-111">Todas as cadeias de caracteres de consulta do usuário devem ser as mesmas para habilitar correções ortográficas para pesquisas de várias entidades.</span><span class="sxs-lookup"><span data-stu-id="531c7-111">All the user query strings should be the same to enable spelling corrections for searches of multiple entities.</span></span>

## <a name="example-1-request-spelling-suggestions"></a><span data-ttu-id="531c7-112">Exemplo 1: Solicitar sugestões ortográficas</span><span class="sxs-lookup"><span data-stu-id="531c7-112">Example 1: Request spelling suggestions</span></span>

<span data-ttu-id="531c7-113">O exemplo a seguir consulta **recursos listItem** que contêm a cadeia de caracteres "accountt" e solicita uma sugestão ortográfica para a consulta.</span><span class="sxs-lookup"><span data-stu-id="531c7-113">The following example queries **listItem** resources that contain the string "accountt" and requests a spelling suggestion for the query.</span></span>

<span data-ttu-id="531c7-114">A resposta contém [objetos alterationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) para a sugestão ortográfica.</span><span class="sxs-lookup"><span data-stu-id="531c7-114">The response contains [alterationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) objects for the spelling suggestion.</span></span>

### <a name="request"></a><span data-ttu-id="531c7-115">Solicitação</span><span class="sxs-lookup"><span data-stu-id="531c7-115">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "listItem"
            ],
            "query": {
                "queryString": "accountt"
            },
            "from": 0,
            "size": 25
        }
    ],
    "queryAlterationOptions": {
        "enableSuggestion": true,
        "enableModification": false
    }
}
```

### <a name="response"></a><span data-ttu-id="531c7-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="531c7-116">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [
                "accountt"
            ],
            "hitsContainers": [
                {
                    "total": 0,
                    "moreResultsAvailable": false
                }
            ]
        }
    ],
    "queryAlterationResponse": {
        "@odata.type": "#microsoft.substrateSearch.alterationResponse",
        "originalQueryString": "accountt",
        "queryAlteration": {
            "@odata.type": "#microsoft.substrateSearch.searchAlteration",
            "alteredQueryString": "account",
            "alteredHighlightedQueryString": "account",
            "alteredQueryTokens": [
                {
                    "offset": 0,
                    "length": 8,
                    "suggestion": "account"
                }
            ]
        },
        "queryAlterationType": "Suggestion"
    }
}
```

## <a name="example-2-request-spelling-modifications"></a><span data-ttu-id="531c7-117">Exemplo 2: Solicitar modificações ortográficas</span><span class="sxs-lookup"><span data-stu-id="531c7-117">Example 2: Request spelling modifications</span></span>

<span data-ttu-id="531c7-118">O exemplo a seguir consulta **recursos listItem** que contêm a cadeia de caracteres "accountt" e solicita uma modificação ortográfica para a consulta.</span><span class="sxs-lookup"><span data-stu-id="531c7-118">The following example queries **listItem** resources that contain the string "accountt" and requests a spelling modification for the query.</span></span>

<span data-ttu-id="531c7-119">Neste exemplo, não há resultados para consulta original com typo "accountt".</span><span class="sxs-lookup"><span data-stu-id="531c7-119">In this example, there are no results for original query with typo "accountt".</span></span> <span data-ttu-id="531c7-120">A resposta contém resultados relacionados aos objetos "account" e [alterationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) da cadeia de caracteres corrigidos para a modificação ortográfica.</span><span class="sxs-lookup"><span data-stu-id="531c7-120">The response contains results related to corrected string "account" and [alterationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) objects for the spelling modification.</span></span>

### <a name="request"></a><span data-ttu-id="531c7-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="531c7-121">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "listItem"
            ],
            "query": {
                "queryString": "accountt"
            },
            "from": 0,
            "size": 25
        }
    ],
    "queryAlterationOptions": {
        "enableSuggestion": true,
        "enableModification": true
    }
}
```

### <a name="response"></a><span data-ttu-id="531c7-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="531c7-122">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [
                "account"
            ],
            "hitsContainers": [
                {
                    "total": 1,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
                            "rank": 1,
                            "summary": "",
                            "resource": {
                                "@odata.type": "#microsoft.graph.listItem",
                                "createdDateTime": "2019-06-10T06:37:43Z",
                                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                                "name": "web_part_test_long Notebook",
                                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/Lists/Issue tracker list/DispForm.aspx?ID=1",
                                "sharepointIds": {
                                    "listId": "33498de0-d695-4d23-ac26-e1bf95a3206e",
                                    "listItemId": "13"
                                },
                                "createdBy": {
                                    "user": {
                                        "displayName": "System Account"
                                    }
                                },
                                "lastModifiedBy": {
                                    "user": {
                                        "displayName": "System Account"
                                    }
                                },
                                "parentReference": {
                                    "sharepointIds": {
                                        "listId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b"
                                    },
                                    "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
                                }
                            }
                        }
                    ]
                }
            ]
        }
    ],
    "queryAlterationResponse": {
        "@odata.type": "#microsoft.substrateSearch.alterationResponse",
        "originalQueryString": "accountt",
        "queryAlteration": {
            "@odata.type": "#microsoft.substrateSearch.searchAlteration",
            "alteredQueryString": "account",
            "alteredHighlightedQueryString": "account",
            "alteredQueryTokens": [
                {
                    "offset": 0,
                    "length": 8,
                    "suggestion": "account"
                }
            ]
        },
        "queryAlterationType": "Modification"
    }
}
```

## <a name="known-limitations"></a><span data-ttu-id="531c7-123">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="531c7-123">Known limitations</span></span>

<span data-ttu-id="531c7-124">A correção ortográfica só é suportada para os seguintes recursos: **message**, **event**, **site**, **drive**, **driveItem**, **list**, **listItem** **e externalItem**.</span><span class="sxs-lookup"><span data-stu-id="531c7-124">Spelling correction is only supported for the following resources: **message**, **event**, **site**, **drive**, **driveItem**, **list**, **listItem** and **externalItem**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="531c7-125">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="531c7-125">Next steps</span></span>

- [<span data-ttu-id="531c7-126">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="531c7-126">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
