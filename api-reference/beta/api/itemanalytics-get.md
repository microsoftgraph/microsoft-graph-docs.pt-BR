---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Obter análises
localization_priority: Normal
ms.openlocfilehash: 1af4f95549a4970e6bf3758e0d9b0c70f62d9132
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880283"
---
# <a name="get-analytics"></a><span data-ttu-id="e0efd-102">Obter análises</span><span class="sxs-lookup"><span data-stu-id="e0efd-102">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0efd-103">Obtenha [][] o naanalytics sobre os modos de exibição que foram colocados sob esse recurso.</span><span class="sxs-lookup"><span data-stu-id="e0efd-103">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="e0efd-104">O recurso do Microsoft **Analytics** é uma maneira conveniente de obter estatísticas de `allTime` atividades para `lastSevenDays`o e o.</span><span class="sxs-lookup"><span data-stu-id="e0efd-104">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="e0efd-105">Para um intervalo ou intervalo de tempo personalizado, use a API [funçãogetactivitiesbyinterval][] .</span><span class="sxs-lookup"><span data-stu-id="e0efd-105">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="e0efd-106">**Observação:** O \*\*\*\* recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="e0efd-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[Funçãogetactivitiesbyinterval]: ../api/itemactivity-getbyinterval.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="e0efd-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0efd-109">Permissions</span></span>

<span data-ttu-id="e0efd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0efd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0efd-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0efd-112">Permission type</span></span>                        | <span data-ttu-id="e0efd-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0efd-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="e0efd-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0efd-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0efd-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0efd-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="e0efd-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0efd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0efd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0efd-117">Not supported.</span></span>
|<span data-ttu-id="e0efd-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0efd-118">Application</span></span>                            | <span data-ttu-id="e0efd-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0efd-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="e0efd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0efd-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="e0efd-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0efd-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e0efd-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0efd-122">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e0efd-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0efd-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e0efd-124">C#</span><span class="sxs-lookup"><span data-stu-id="e0efd-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0efd-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="e0efd-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e0efd-126">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e0efd-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e0efd-127">Java</span><span class="sxs-lookup"><span data-stu-id="e0efd-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e0efd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0efd-128">Response</span></span>

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
