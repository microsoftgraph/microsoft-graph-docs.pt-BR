---
title: Usar a API de Pesquisa da Microsoft para classificar resultados de pesquisa (visualização)
description: Você classificar resultados de pesquisa usando a API de Pesquisa da Microsoft.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 4f4a2c8925e910520ca3d75d98f86d713105f6ac
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067184"
---
# <a name="use-the-microsoft-search-api-to-sort-search-results-preview"></a><span data-ttu-id="1b836-103">Usar a API de Pesquisa da Microsoft para classificar resultados de pesquisa (visualização)</span><span class="sxs-lookup"><span data-stu-id="1b836-103">Use the Microsoft Search API to sort search results (preview)</span></span>

<span data-ttu-id="1b836-104">Você pode usar a API de Pesquisa da Microsoft no Microsoft Graph classificar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="1b836-104">You can use the Microsoft Search API in Microsoft Graph to sort search results.</span></span> <span data-ttu-id="1b836-105">Para classificar os resultados, especifique a propriedade **sortProperties** em um objeto [searchRequest](/graph/api/resources/searchrequest?view=graph-rest-beta&preserve-view=true) e identifique uma propriedade de recurso em **entityTypes** para classificar as corresponde por, em ordem crescente ou decrescente.</span><span class="sxs-lookup"><span data-stu-id="1b836-105">To sort the results, specify the **sortProperties** property in a [searchRequest](/graph/api/resources/searchrequest?view=graph-rest-beta&preserve-view=true) object and identify a resource property in **entityTypes** to sort matches by, in ascending or descending order.</span></span>

<span data-ttu-id="1b836-106">A classificação só é suportada para SharePoint e OneDrive itens.</span><span class="sxs-lookup"><span data-stu-id="1b836-106">Sorting is supported only for SharePoint and OneDrive items.</span></span>
<span data-ttu-id="1b836-107">A propriedade a ser classificação deve ser *Sortable* no esquema de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="1b836-107">The property to be sorted on should be *Sortable* in the search schema.</span></span>

<span data-ttu-id="1b836-108">A ordem de classificação padrão é crescente.</span><span class="sxs-lookup"><span data-stu-id="1b836-108">The default sort order is ascending.</span></span> <span data-ttu-id="1b836-109">De definir **a propriedade isDescending** para alterá-la.</span><span class="sxs-lookup"><span data-stu-id="1b836-109">Set the **isDescending** property to change it.</span></span>

## <a name="example-1-single-level-sort"></a><span data-ttu-id="1b836-110">Exemplo 1: Classificação de nível único</span><span class="sxs-lookup"><span data-stu-id="1b836-110">Example 1: Single-level sort</span></span>

### <a name="request"></a><span data-ttu-id="1b836-111">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b836-111">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
          "driveItem"
      ],
       "query": {
        "queryString": "contoso"
      },
      "sortProperties": [
          {
              "name": "CreatedDateTime",
              "isDescending": false
          }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1b836-112">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b836-112">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.searchResponse",
    "searchTerms": [
        "test"
    ],
    "hitsContainers": [
        {
            "@odata.type": "#microsoft.graph.searchHitsContainer",
            "hits": [
                {
                    "@odata.type": "#microsoft.graph.searchHit",
                    "hitId": "01VRZMWHPGDM5KTXS53RF3SSGHW7SGGPKL",
                    "rank": 1,
                    "summary": "As we work to become a more <ddd/> We <c0>test</c0> samples from the region between 10 and 100 times per day <ddd/> and surrounding areas that CPU uses to <c0>test</c0> the quality of your drinking water every day <ddd/> ",
                    "resource": {
                        "@odata.type": "#microsoft.graph.driveItem",
                        "size": 971838,
                        "fileSystemInfo": {
                            "createdDateTime": "2020-07-22T21:14:59Z",
                            "lastModifiedDateTime": "2018-09-12T16:20:16Z"
                        },
                        "id": "01VRZMWHPGDM5KTXS53RF3SSGHW7SGGPKL",
                        "createdBy": {
                            "user": {
                                "displayName": "Contoso066a"
                            }
                        },
                        "createdDateTime": "2020-07-22T21:14:59+00:00",
                        "lastModifiedBy": {
                            "user": {
                                "displayName": "Contoso066a"
                            }
                        },
                        "lastModifiedDateTime": "2018-09-12T16:20:16+00:00",
                        "name": "Our Water Our Future.docx",
                        "parentReference": {
                            "siteId": "Contoso066a,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0",
                            "driveId": "b!NAe_rKr80k-n7e5zlCVIqSnIwTNsGBVBlusjEvRHgjMmmcA3Ubc7R4Kyao9hbgL4",
                            "sharepointIds": {
                                "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                                "listItemId": "1027",
                                "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
                            }
                        },
                        "webUrl": "https://Contoso066a/sites/GlobalSales/Shared Documents/Q1 2019/Our Water Our Future.docx"
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.searchHit",
                    "hitId": "01BTQFB3LHZTAYBV2VXVEK22ETF5WOQGT2",
                    "rank": 2,
                    "summary": "QT300 Accessories Specs Costs Chart Continue <ddd/> 16 Package 5 14 Grand Total 99 Results Data <c0>Test</c0> Group Gender <c0>Test</c0> Option 1 2 3 18-25 Male Package 4 Color <ddd/> ",
                    "resource": {
                        "@odata.type": "#microsoft.graph.driveItem",
                        "size": 34428,
                        "fileSystemInfo": {
                            "createdDateTime": "2020-07-22T21:23:50Z",
                            "lastModifiedDateTime": "2012-10-29T17:52:10Z"
                        },
                        "id": "01BTQFB3LHZTAYBV2VXVEK22ETF5WOQGT2",
                        "createdBy": {
                            "user": {
                                "displayName": "Contoso066a"
                            }
                        },
                        "createdDateTime": "2020-07-22T21:23:50+00:00",
                        "lastModifiedBy": {
                            "user": {
                                "displayName": "Contoso066a"
                            }
                        },
                        "lastModifiedDateTime": "2012-10-29T17:52:10+00:00",
                        "name": "QT300 Accessories Specs.xlsx",
                        "parentReference": {
                            "siteId": "Contoso066a,893378cb-d2cd-4076-a2c9-e50587a26832,04120cf2-7863-4701-8541-eb26266a25e6",
                            "driveId": "b!H9kkVwxlEEiDzGGogYkX1twlusOfLMtIg750zfaOpaBq9eOBX6MXQapv1hTT-bIt",
                            "sharepointIds": {
                                "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                                "listItemId": "1027",
                                "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
                            }
                        },
                        "webUrl": "https://Contoso066a/sites/contosoteam/Shared Documents/QT300 Accessories Specs.xlsx"
                    }
                }
            ]
        }
    ]
}
```

## <a name="example-2-multi-level-sort"></a><span data-ttu-id="1b836-113">Exemplo 2: Classificação de vários níveis</span><span class="sxs-lookup"><span data-stu-id="1b836-113">Example 2: Multi-level sort</span></span>

### <a name="request"></a><span data-ttu-id="1b836-114">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b836-114">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
          "microsoft.graph.driveItem"
      ],
       "query": {
        "queryString": "contoso"
      },
      "sortProperties": [
          {
              "name": "name",
              "isDescending": false
          },
          {
              "name": "CreatedDateTime",
              "isDescending": false
          }
      ],
      "from": 0,
      "size": 20
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1b836-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b836-115">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.searchResponse",
    "searchTerms": [
        "test"
    ],
    "hitsContainers": [
        {
            "@odata.type": "#microsoft.graph.searchHitsContainer",
            "hits": [
                {
                    "@odata.type": "#microsoft.graph.searchHit",
                    "hitId": "01D6DZBXUX6RQ2OM7AIVEJFRQTD3W75L7V",
                    "rank": 1,
                    "summary": "If you are projecting to a second monitor, use Presenter View on your PC to read the talk track and see where to click next (note that this is a PowerPoint, so the “clicks” are <ddd/> ",
                    "resource": {
                        "@odata.type": "#microsoft.graph.driveItem",
                        "size": 34122491,
                        "fileSystemInfo": {
                            "createdDateTime": "2020-07-22T21:48:38Z",
                            "lastModifiedDateTime": "2019-01-11T22:41:06Z"
                        },
                        "id": "01D6DZBXUX6RQ2OM7AIVEJFRQTD3W75L7V",
                        "createdBy": {
                            "user": {
                                "displayName": "Contoso066a"
                            }
                        },
                        "createdDateTime": "2020-07-22T21:48:38+00:00",
                        "lastModifiedBy": {
                            "user": {
                                "displayName": "Contoso066a"
                            }
                        },
                        "lastModifiedDateTime": "2019-01-11T22:41:06+00:00",
                        "name": "Build an Approval Process with Microsoft Flow Click Through.pptx",
                        "parentReference": {
                            "siteId": "Contoso066a,506e4b2b-4af3-41e6-904c-668e67911889,04120cf2-7863-4701-8541-eb26266a25e6",
                            "driveId": "b!K0tuUPNK5kGQTGaOZ5EYifIMEgRjeAFHhUHrJiZqJeZq9eOBX6MXQapv1hTT-bIt",
                            "sharepointIds": {
                                "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                                "listItemId": "1027",
                                "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
                            }
                        },
                        "webUrl": "https://Contoso066a/sites/DigitalInitiativePublicRelations/Shared Documents/General/PowerApps/Build an Approval Process with Microsoft Flow Click Through.pptx"
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.searchHit",
                    "hitId": "013C7INN2ZPRBMXUAPJNDKMJ2YHTGQLXJT",
                    "rank": 2,
                    "summary": "You can use the Office Add-ins platform to build solutions that extend Office applications and interact with content in Office documents <ddd/> Your solution can run in Office across <ddd/> ",
                    "resource": {
                        "@odata.type": "#microsoft.graph.driveItem",
                        "size": 7816159,
                        "fileSystemInfo": {
                            "createdDateTime": "2020-07-27T11:20:22Z",
                            "lastModifiedDateTime": "2017-09-15T14:20:00Z"
                        },
                        "id": "013C7INN2ZPRBMXUAPJNDKMJ2YHTGQLXJT",
                        "createdBy": {
                            "user": {
                                "displayName": "Contoso066a"
                            }
                        },
                        "createdDateTime": "2020-07-27T11:20:22+00:00",
                        "lastModifiedBy": {
                            "user": {
                                "displayName": "Contoso066a"
                            }
                        },
                        "lastModifiedDateTime": "2017-09-15T14:20:00+00:00",
                        "name": "CR -227 Camera briefing.docx",
                        "parentReference": {
                            "siteId": "Contoso066a,7955f1b7-70eb-4a26-8fa7-313ad3a45126,04120cf2-7863-4701-8541-eb26266a25e6",
                            "driveId": "b!t_FVeetwJkqPpzE606RRJvIMEgRjeAFHhUHrJiZqJeYmmcA3Ubc7R4Kyao9hbgL4",
                            "sharepointIds": {
                                "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                                "listItemId": "1027",
                                "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
                            }
                        },
                        "webUrl": "https://Contoso066a/sites/Mark8ProjectTeam/Shared Documents/Research and Development/CR -227 Camera briefing.docx"
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.searchHit",
                    "hitId": "013C7INN67OOARDMIO3BE23AHO3AMCC62W",
                    "rank": 3,
                    "summary": "<c0>Test</c0> Credit Card Account Numbers <ddd/> While testing, use only the credit card numbers listed <ddd/> a different character count than the other <c0>test</c0> numbers, it is the correct and functional <ddd/> ",
                    "resource": {
                        "@odata.type": "#microsoft.graph.driveItem",
                        "size": 22418,
                        "fileSystemInfo": {
                            "createdDateTime": "2020-07-27T11:22:11Z",
                            "lastModifiedDateTime": "2016-06-09T16:23:00Z"
                        },
                        "id": "013C7INN67OOARDMIO3BE23AHO3AMCC62W",
                        "createdBy": {
                            "user": {
                                "displayName": "Contoso066a"
                            }
                        },
                        "createdDateTime": "2020-07-27T11:22:11+00:00",
                        "lastModifiedBy": {
                            "user": {
                                "displayName": "Contoso066a"
                            }
                        },
                        "lastModifiedDateTime": "2016-06-09T16:23:00+00:00",
                        "name": "Manufacturing and delivery plan.docx",
                        "parentReference": {
                            "siteId": "Contoso066a,7955f1b7-70eb-4a26-8fa7-313ad3a45126,04120cf2-7863-4701-8541-eb26266a25e6",
                            "driveId": "b!NAe_rKr80k-n7e5zlCVIqfIMEgRjeAFHhUHrJiZqJeYmmcA3Ubc7R4Kyao9hbgL4",
                            "sharepointIds": {
                                "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                                "listItemId": "1027",
                                "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
                            }
                        },
                        "webUrl": "https://Contoso066a/sites/Mark8ProjectTeam/Shared Documents/Research and Development/Manufacturing and delivery plan.docx"
                    }
                }
            ]
        }
    ]
}
```

## <a name="known-limitations"></a><span data-ttu-id="1b836-116">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="1b836-116">Known limitations</span></span>

- <span data-ttu-id="1b836-117">Não há suporte para classificação para **mensagem,** **evento** e **externalItem**.</span><span class="sxs-lookup"><span data-stu-id="1b836-117">Sort is not supported for **message**, **event**, and **externalItem**.</span></span>
- <span data-ttu-id="1b836-118">Classificar por relevância não pode ser especificado em **sortProperties**.</span><span class="sxs-lookup"><span data-stu-id="1b836-118">Sort by relevance cannot be specified in **sortProperties**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1b836-119">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="1b836-119">Next steps</span></span>

- [<span data-ttu-id="1b836-120">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="1b836-120">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
