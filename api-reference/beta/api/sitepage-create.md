---
author: rahmit
description: Criar um novo sitePage na lista de páginas do site em um site.
ms.date: 05/07/2018
title: Criar uma nova página em um site do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: cc9b7a997602252aa58f94178b30fa719bc9ee11
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475748"
---
# <a name="create-a-page-in-the-site-pages-list-of-a-site"></a><span data-ttu-id="dfd97-103">Criar uma página na lista de páginas do site de um site</span><span class="sxs-lookup"><span data-stu-id="dfd97-103">Create a page in the site pages list of a site</span></span>

<span data-ttu-id="dfd97-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfd97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfd97-105">Criar um novo [sitePage][] na lista de páginas [do][] site em um [site][].</span><span class="sxs-lookup"><span data-stu-id="dfd97-105">Create a new [sitePage][] in the site pages [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="dfd97-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfd97-106">Permissions</span></span>

<span data-ttu-id="dfd97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfd97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfd97-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfd97-109">Permission type</span></span>      | <span data-ttu-id="dfd97-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfd97-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfd97-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfd97-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dfd97-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfd97-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="dfd97-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfd97-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfd97-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfd97-114">Not supported.</span></span>    |
|<span data-ttu-id="dfd97-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfd97-115">Application</span></span> | <span data-ttu-id="dfd97-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfd97-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfd97-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfd97-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/pages
```

## <a name="request-body"></a><span data-ttu-id="dfd97-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfd97-118">Request body</span></span>

<span data-ttu-id="dfd97-119">No corpo da solicitação, fornece uma representação JSON do [recurso sitePage][] a ser criado.</span><span class="sxs-lookup"><span data-stu-id="dfd97-119">In the request body, supply a JSON representation of the [sitePage][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="dfd97-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfd97-120">Example</span></span>

<span data-ttu-id="dfd97-121">O exemplo a seguir mostra como criar uma nova página.</span><span class="sxs-lookup"><span data-stu-id="dfd97-121">The following example shows how to create a new page.</span></span>


# <a name="http"></a>[<span data-ttu-id="dfd97-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfd97-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-page", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/pages
Content-Type: application/json

{
    "name": "Events.aspx",
    "title": "Team Events",
    "publishingState": {
        "level": "checkedOut",
        "versionId": "0.1"
    },
    "webParts": [
        {
            "type": "rte",
            "innerHTML": "<p>Here are the team's upcoming events:</p>"
        },
        {
            "type": "d1d91016-032f-456d-98a4-721247c305e8",
            "data": {
                "title": "Events",
                "description": "Display upcoming events",
                "serverProcessedContent": {
                    "htmlStrings": {},
                    "searchablePlainTexts": {
                        "title": ""
                    },
                    "imageSources": {},
                    "links": {
                        "baseUrl": "https://www.contoso.com/sites/Engineering"
                    },
                    "componentDependencies": {
                        "layoutComponentId": "8ac0c53c-e8d0-4e3e-87d0-7449eb0d4027"
                    }
                },
                "dataVersion": "1.0",
                "properties": {
                    "selectedListId": "032e08ab-89b0-4d8f-bc10-73094233615c",
                    "selectedCategory": "",
                    "dateRangeOption": 0,
                    "startDate": "",
                    "endDate": "",
                    "isOnSeeAllPage": false,
                    "layoutId": "FilmStrip",
                    "dataProviderId": "Event",
                    "webId": "0764c419-1ecc-4126-ba32-0c25ae0fffe8",
                    "siteId": "6b4ffc7a-cfc2-4a76-903a-1cc3686dee23"
                }
            }
        }
    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="dfd97-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfd97-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="dfd97-124">C#</span><span class="sxs-lookup"><span data-stu-id="dfd97-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="dfd97-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfd97-125">Response</span></span>

<span data-ttu-id="dfd97-126">Se tiver êxito, este método retornará [um sitePage][] no corpo da resposta para a página criada.</span><span class="sxs-lookup"><span data-stu-id="dfd97-126">If successful, this method returns a [sitePage][] in the response body for the created page.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.sitePage", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "2",
    "eTag": "75bc70e2-6587-45be-8493-c99a956b2e05,7",
    "createdDateTime": "2016-12-06T20:04:40Z",
    "lastModifiedDateTime": "2016-12-06T20:05:09Z",
    "webUrl": "https://www.contoso.com/sites/Engineering/SitePages/Events.aspx",
    "createdBy": {
        "user": {
            "email": "rahmit",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal"
        }
    },
    "lastModifiedBy": {
        "user": {
            "email": "rahmit",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal"
        }
    },
    "parentReference": {
        "id": "eb3bfd48-56f8-4c1e-8312-e58588b22e7c"
    },
    "contentType": {
        "id": "0x0101009D1CB255DA76424F860D91F20E6C411800C9E7033636784C4B88A284B1823C45FD",
        "name": "Site Page"
    },
    "description": "",
    "title": "Team Events",
    "webParts": [
        {
            "type": "rte",
            "data": {
                "innerHTML": "<p>Here are the team's upcoming events:</p>"
            }
        },
        {
            "type": "d1d91016-032f-456d-98a4-721247c305e8",
            "data": {
                "title": "Events",
                "description": "Display upcoming events",
                "serverProcessedContent": {
                    "htmlStrings": {},
                    "searchablePlainTexts": {
                        "title": ""
                    },
                    "imageSources": {},
                    "links": {
                        "baseUrl": "https://www.contoso.com/teams/Engineering"
                    },
                    "componentDependencies": {
                        "layoutComponentId": "8ac0c53c-e8d0-4e3e-87d0-7449eb0d4027"
                    }
                },
                "dataVersion": "1.0",
                "properties": {
                    "selectedListId": "032e08ab-89b0-4d8f-bc10-73094233615c",
                    "selectedCategory": "",
                    "dateRangeOption": 0,
                    "startDate": "",
                    "endDate": "",
                    "isOnSeeAllPage": false,
                    "layoutId": "FilmStrip",
                    "dataProviderId": "Event",
                    "webId": "0764c419-1ecc-4126-ba32-0c25ae0fffe8",
                    "siteId": "6b4ffc7a-cfc2-4a76-903a-1cc3686dee23"
                }
            }
        }
    ]
}
```

<span data-ttu-id="dfd97-127">**Observação:** O objeto Response será truncado para mais clareza.</span><span class="sxs-lookup"><span data-stu-id="dfd97-127">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="dfd97-128">As propriedades padrão serão retornadas da chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfd97-128">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[listItem]: ../resources/listitem.md
[site]: ../resources/site.md
[sitePage]: ../resources/sitepage.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a sitePage in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Create",
  "suppressions": []
}
-->


