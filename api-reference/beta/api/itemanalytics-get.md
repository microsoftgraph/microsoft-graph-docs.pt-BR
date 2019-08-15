---
author: daspek
description: Obtenha o naanalytics sobre os modos de exibição que foram colocados sob esse recurso.
ms.date: 10/06/2017
title: Obter análises
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 9e388f913e310d7f8a294a1f5d1703e72cdc1ddd
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415483"
---
# <a name="get-analytics"></a><span data-ttu-id="4b639-103">Obter análises</span><span class="sxs-lookup"><span data-stu-id="4b639-103">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b639-104">Obtenha [][] o naanalytics sobre os modos de exibição que foram colocados sob esse recurso.</span><span class="sxs-lookup"><span data-stu-id="4b639-104">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="4b639-105">O recurso do Microsoft **Analytics** é uma maneira conveniente de obter estatísticas de `allTime` atividades para `lastSevenDays`o e o.</span><span class="sxs-lookup"><span data-stu-id="4b639-105">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="4b639-106">Para um intervalo ou intervalo de tempo personalizado, use a API [funçãogetactivitiesbyinterval][] .</span><span class="sxs-lookup"><span data-stu-id="4b639-106">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="4b639-107">**Observação:** O \*\*\*\* recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="4b639-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[Funçãogetactivitiesbyinterval]: ../api/itemactivity-getbyinterval.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="4b639-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b639-110">Permissions</span></span>

<span data-ttu-id="4b639-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b639-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b639-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b639-113">Permission type</span></span>                        | <span data-ttu-id="4b639-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b639-114">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="4b639-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b639-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b639-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b639-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="4b639-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b639-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b639-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b639-118">Not supported.</span></span>
|<span data-ttu-id="4b639-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b639-119">Application</span></span>                            | <span data-ttu-id="4b639-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b639-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4b639-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b639-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="4b639-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b639-122">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4b639-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b639-123">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4b639-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b639-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4b639-125">C#</span><span class="sxs-lookup"><span data-stu-id="4b639-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b639-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b639-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4b639-127">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4b639-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4b639-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b639-128">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
  ]
}
-->
