---
author: daspek
description: Obter itemActivityStats para as atividades que foram realizadas sob esse recurso dentro do intervalo de tempo especificado.
ms.date: 10/06/2017
title: Obter estatísticas de atividade de item por intervalo
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: f2c3158fbc7ac8c925bc0bf2556623d01aa7b48d
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123180"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="c23ca-103">Obter estatísticas de atividade de item por intervalo</span><span class="sxs-lookup"><span data-stu-id="c23ca-103">Get item activity stats by interval</span></span>

<span data-ttu-id="c23ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c23ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c23ca-105">Obter [itemActivityStats][] para as atividades que foram realizadas sob esse recurso dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="c23ca-105">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="c23ca-106">**Observação:** O recurso do **naanalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="c23ca-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="c23ca-107">As agregações de análise podem não estar disponíveis para todos os tipos de ação.</span><span class="sxs-lookup"><span data-stu-id="c23ca-107">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="c23ca-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c23ca-109">Permissions</span></span>

<span data-ttu-id="c23ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c23ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c23ca-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c23ca-112">Permission type</span></span>                        | <span data-ttu-id="c23ca-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c23ca-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="c23ca-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c23ca-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c23ca-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c23ca-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="c23ca-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c23ca-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c23ca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c23ca-117">Not supported.</span></span>
|<span data-ttu-id="c23ca-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c23ca-118">Application</span></span>                            | <span data-ttu-id="c23ca-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c23ca-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c23ca-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c23ca-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="c23ca-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c23ca-121">Function parameters</span></span>

| <span data-ttu-id="c23ca-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c23ca-122">Parameter</span></span>      | <span data-ttu-id="c23ca-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c23ca-123">Type</span></span>               | <span data-ttu-id="c23ca-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c23ca-124">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="c23ca-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c23ca-125">startDateTime</span></span>  | <span data-ttu-id="c23ca-126">Cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="c23ca-126">string (timestamp)</span></span> | <span data-ttu-id="c23ca-127">A hora de início em que as atividades serão agregadas.</span><span class="sxs-lookup"><span data-stu-id="c23ca-127">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="c23ca-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c23ca-128">endDateTime</span></span>    | <span data-ttu-id="c23ca-129">Cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="c23ca-129">string (timestamp)</span></span> | <span data-ttu-id="c23ca-130">A hora de término sobre a qual agregar atividades.</span><span class="sxs-lookup"><span data-stu-id="c23ca-130">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="c23ca-131">interval</span><span class="sxs-lookup"><span data-stu-id="c23ca-131">interval</span></span>       | <span data-ttu-id="c23ca-132">string</span><span class="sxs-lookup"><span data-stu-id="c23ca-132">string</span></span>             | <span data-ttu-id="c23ca-133">O intervalo de agregação.</span><span class="sxs-lookup"><span data-stu-id="c23ca-133">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="c23ca-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c23ca-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c23ca-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c23ca-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c23ca-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c23ca-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="c23ca-137">C#</span><span class="sxs-lookup"><span data-stu-id="c23ca-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c23ca-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c23ca-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c23ca-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c23ca-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c23ca-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c23ca-140">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```json
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
