---
author: daspek
description: Obter itemAnalytics sobre os exibições que ocorreram sob esse recurso.
ms.date: 10/06/2017
title: Obter análises
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 6366106097b4f6b9b43d8fe0eacddeaeab53826d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475797"
---
# <a name="get-analytics"></a><span data-ttu-id="c891b-103">Obter análises</span><span class="sxs-lookup"><span data-stu-id="c891b-103">Get analytics</span></span>

<span data-ttu-id="c891b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c891b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c891b-105">Obter [itemAnalytics][] sobre os exibições que ocorreram sob esse recurso.</span><span class="sxs-lookup"><span data-stu-id="c891b-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="c891b-106">O **recurso itemAnalytics** é uma maneira conveniente de obter estatísticas de atividade para `allTime` e para o `lastSevenDays` .</span><span class="sxs-lookup"><span data-stu-id="c891b-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="c891b-107">Para um intervalo ou intervalo de tempo personalizado, use a API [getActivitiesByInterval.][]</span><span class="sxs-lookup"><span data-stu-id="c891b-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="c891b-108">**Observação:** O **recurso itemAnalytics** ainda não está disponível em todas as [implantações nacionais.](/graph/deployments)</span><span class="sxs-lookup"><span data-stu-id="c891b-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="c891b-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="c891b-111">Permissions</span></span>

<span data-ttu-id="c891b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c891b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c891b-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c891b-114">Permission type</span></span>                        | <span data-ttu-id="c891b-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c891b-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="c891b-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c891b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="c891b-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c891b-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="c891b-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c891b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c891b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c891b-119">Not supported.</span></span>
|<span data-ttu-id="c891b-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c891b-120">Application</span></span>                            | <span data-ttu-id="c891b-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c891b-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c891b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c891b-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="c891b-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c891b-123">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c891b-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c891b-124">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c891b-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="c891b-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="c"></a>[<span data-ttu-id="c891b-126">C#</span><span class="sxs-lookup"><span data-stu-id="c891b-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c891b-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c891b-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c891b-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c891b-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c891b-129">Java</span><span class="sxs-lookup"><span data-stu-id="c891b-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c891b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c891b-130">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```http
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


