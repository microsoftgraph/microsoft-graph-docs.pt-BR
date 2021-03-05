---
author: daspek
description: Obter itemActivityStats para as atividades que ocorreram sob esse recurso dentro do intervalo de tempo especificado.
ms.date: 10/06/2017
title: Obter estatísticas de atividade de item por intervalo
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: c56169132d43843f60a9c53417271faf30f4afb1
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474691"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="fb84d-103">Obter estatísticas de atividade de item por intervalo</span><span class="sxs-lookup"><span data-stu-id="fb84d-103">Get item activity stats by interval</span></span>

<span data-ttu-id="fb84d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb84d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb84d-105">Obter [itemActivityStats][] para as atividades que ocorreram sob esse recurso dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="fb84d-105">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="fb84d-106">**Observação:** O **recurso itemAnalytics** ainda não está disponível em todas as [implantações nacionais.](/graph/deployments)</span><span class="sxs-lookup"><span data-stu-id="fb84d-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="fb84d-107">Os agregados de análise podem não estar disponíveis para todos os tipos de ação.</span><span class="sxs-lookup"><span data-stu-id="fb84d-107">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="fb84d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb84d-109">Permissions</span></span>

<span data-ttu-id="fb84d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb84d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb84d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb84d-112">Permission type</span></span>                        | <span data-ttu-id="fb84d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb84d-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="fb84d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb84d-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb84d-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb84d-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="fb84d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb84d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb84d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb84d-117">Not supported.</span></span>
|<span data-ttu-id="fb84d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb84d-118">Application</span></span>                            | <span data-ttu-id="fb84d-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb84d-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="fb84d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb84d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="fb84d-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="fb84d-121">Function parameters</span></span>

| <span data-ttu-id="fb84d-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fb84d-122">Parameter</span></span>      | <span data-ttu-id="fb84d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb84d-123">Type</span></span>               | <span data-ttu-id="fb84d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb84d-124">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="fb84d-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fb84d-125">startDateTime</span></span>  | <span data-ttu-id="fb84d-126">string (timestamp)</span><span class="sxs-lookup"><span data-stu-id="fb84d-126">string (timestamp)</span></span> | <span data-ttu-id="fb84d-127">O tempo de início sobre o qual agregar atividades.</span><span class="sxs-lookup"><span data-stu-id="fb84d-127">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="fb84d-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fb84d-128">endDateTime</span></span>    | <span data-ttu-id="fb84d-129">string (timestamp)</span><span class="sxs-lookup"><span data-stu-id="fb84d-129">string (timestamp)</span></span> | <span data-ttu-id="fb84d-130">O tempo final sobre o qual agregar atividades.</span><span class="sxs-lookup"><span data-stu-id="fb84d-130">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="fb84d-131">interval</span><span class="sxs-lookup"><span data-stu-id="fb84d-131">interval</span></span>       | <span data-ttu-id="fb84d-132">string</span><span class="sxs-lookup"><span data-stu-id="fb84d-132">string</span></span>             | <span data-ttu-id="fb84d-133">O intervalo de agregação.</span><span class="sxs-lookup"><span data-stu-id="fb84d-133">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="fb84d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb84d-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fb84d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb84d-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fb84d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb84d-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="fb84d-137">C#</span><span class="sxs-lookup"><span data-stu-id="fb84d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb84d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb84d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb84d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb84d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb84d-140">Java</span><span class="sxs-lookup"><span data-stu-id="fb84d-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activities-by-interval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fb84d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb84d-141">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "startDateTime": "2017-01-01T00:00:00.000Z",
            "endDateTime": "2017-01-02T00:00:00.000Z",
            "delete": {
                "actionCount": 1,
                "actorCount": 1
            },
            "access": {
                "actionCount": 5,
                "actorCount": 3
            }
        },
        {
            "startDateTime": "2017-01-02T00:00:00.000Z",
            "endDateTime": "2017-01-03T00:00:00.000Z",
            "edit": {
                "actionCount": 3,
                "actorCount": 1
            },
            "access": {
                "actionCount": 7,
                "actorCount": 6
            }
        }
    ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get activities by interval",
  "suppressions": []
}
-->


