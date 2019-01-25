---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Obtenha a análise
localization_priority: Normal
ms.openlocfilehash: d1f6b255747cffe7fdccb5d098e73a56151b6245
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516256"
---
# <a name="get-analytics"></a><span data-ttu-id="60603-102">Obtenha a análise</span><span class="sxs-lookup"><span data-stu-id="60603-102">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60603-103">Obtenha [itemAnalytics][] sobre os modos de exibição que foi realizada sob este recurso.</span><span class="sxs-lookup"><span data-stu-id="60603-103">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="60603-104">O recurso de **itemAnalytics** é uma maneira conveniente para obter as estatísticas de atividade do `allTime` e o `lastSevenDays`.</span><span class="sxs-lookup"><span data-stu-id="60603-104">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="60603-105">Para um intervalo de tempo personalizado ou um intervalo, use o [getActivitiesByInterval][] API.</span><span class="sxs-lookup"><span data-stu-id="60603-105">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="60603-106">**Observação:** O recurso de **itemAnalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="60603-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="60603-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="60603-109">Permissions</span></span>

<span data-ttu-id="60603-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60603-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60603-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60603-112">Permission type</span></span>                        | <span data-ttu-id="60603-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60603-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="60603-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60603-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="60603-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60603-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="60603-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60603-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60603-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60603-117">Not supported.</span></span>
|<span data-ttu-id="60603-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60603-118">Application</span></span>                            | <span data-ttu-id="60603-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60603-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="60603-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60603-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="60603-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60603-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="60603-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60603-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="60603-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="60603-123">Response</span></span>

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
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
