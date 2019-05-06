---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Obter análises
localization_priority: Normal
ms.openlocfilehash: b0112041d6b8a8fead91ff76501d9e9b5f1c3102
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598311"
---
# <a name="get-analytics"></a><span data-ttu-id="026a5-102">Obter análises</span><span class="sxs-lookup"><span data-stu-id="026a5-102">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="026a5-103">Obtenha [][] o naanalytics sobre os modos de exibição que foram colocados sob esse recurso.</span><span class="sxs-lookup"><span data-stu-id="026a5-103">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="026a5-104">O recurso do Microsoft **Analytics** é uma maneira conveniente de obter estatísticas de `allTime` atividades para `lastSevenDays`o e o.</span><span class="sxs-lookup"><span data-stu-id="026a5-104">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="026a5-105">Para um intervalo ou intervalo de tempo personalizado, use a API [funçãogetactivitiesbyinterval][] .</span><span class="sxs-lookup"><span data-stu-id="026a5-105">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="026a5-106">**Observação:** O \*\*\*\* recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="026a5-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[Funçãogetactivitiesbyinterval]: ../api/itemactivity-getbyinterval.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="026a5-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="026a5-109">Permissions</span></span>

<span data-ttu-id="026a5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="026a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="026a5-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="026a5-112">Permission type</span></span>                        | <span data-ttu-id="026a5-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="026a5-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="026a5-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="026a5-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="026a5-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="026a5-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="026a5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="026a5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="026a5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="026a5-117">Not supported.</span></span>
|<span data-ttu-id="026a5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="026a5-118">Application</span></span>                            | <span data-ttu-id="026a5-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="026a5-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="026a5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="026a5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="026a5-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="026a5-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="026a5-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="026a5-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="026a5-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="026a5-123">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="026a5-124">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="026a5-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="026a5-125">Basic</span><span class="sxs-lookup"><span data-stu-id="026a5-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-analytics-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="026a5-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="026a5-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-analytics-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
