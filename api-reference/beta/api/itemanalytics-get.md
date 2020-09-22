---
author: daspek
description: Obtenha o naanalytics sobre os modos de exibição que foram colocados sob esse recurso.
ms.date: 10/06/2017
title: Obter análises
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 239b53b716a050dd59d35b25825c38bbcd4f9be8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979991"
---
# <a name="get-analytics"></a><span data-ttu-id="0e1cd-103">Obter análises</span><span class="sxs-lookup"><span data-stu-id="0e1cd-103">Get analytics</span></span>

<span data-ttu-id="0e1cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e1cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e1cd-105">Obtenha o [naanalytics][] sobre os modos de exibição que foram colocados sob esse recurso.</span><span class="sxs-lookup"><span data-stu-id="0e1cd-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="0e1cd-106">O recurso do Microsoft **Analytics** é uma maneira conveniente de obter estatísticas de atividades para `allTime` o e o `lastSevenDays` .</span><span class="sxs-lookup"><span data-stu-id="0e1cd-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="0e1cd-107">Para um intervalo ou intervalo de tempo personalizado, use a API [funçãogetactivitiesbyinterval][] .</span><span class="sxs-lookup"><span data-stu-id="0e1cd-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="0e1cd-108">**Observação:** O recurso do **naanalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="0e1cd-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[Funçãogetactivitiesbyinterval]: ../api/itemactivity-getbyinterval.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="0e1cd-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e1cd-111">Permissions</span></span>

<span data-ttu-id="0e1cd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e1cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e1cd-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e1cd-114">Permission type</span></span>                        | <span data-ttu-id="0e1cd-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e1cd-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="0e1cd-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e1cd-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e1cd-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e1cd-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="0e1cd-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e1cd-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e1cd-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e1cd-119">Not supported.</span></span>
|<span data-ttu-id="0e1cd-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e1cd-120">Application</span></span>                            | <span data-ttu-id="0e1cd-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e1cd-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="0e1cd-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e1cd-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="0e1cd-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e1cd-123">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0e1cd-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e1cd-124">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0e1cd-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e1cd-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="c"></a>[<span data-ttu-id="0e1cd-126">C#</span><span class="sxs-lookup"><span data-stu-id="0e1cd-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e1cd-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e1cd-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e1cd-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e1cd-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0e1cd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e1cd-129">Response</span></span>

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


