---
author: daspek
description: Obter itemActivityStats para as atividades que foram realizadas sob esse recurso dentro do intervalo de tempo especificado.
ms.date: 10/06/2017
title: Obter estatísticas de atividade de item por intervalo
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 6d1f7a3b4e6a326f107a0d0ff33db59ed73f2794
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979103"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="75fc2-103">Obter estatísticas de atividade de item por intervalo</span><span class="sxs-lookup"><span data-stu-id="75fc2-103">Get item activity stats by interval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75fc2-104">Obter [itemActivityStats][] para as atividades que foram realizadas sob esse recurso dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="75fc2-104">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="75fc2-105">**Observação:** O \*\*\*\* recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="75fc2-105">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="75fc2-106">As agregações de análise podem não estar disponíveis para todos os tipos de ação.</span><span class="sxs-lookup"><span data-stu-id="75fc2-106">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="75fc2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="75fc2-108">Permissions</span></span>

<span data-ttu-id="75fc2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75fc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75fc2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75fc2-111">Permission type</span></span>                        | <span data-ttu-id="75fc2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75fc2-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="75fc2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75fc2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="75fc2-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75fc2-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="75fc2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75fc2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75fc2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75fc2-116">Not supported.</span></span>
|<span data-ttu-id="75fc2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75fc2-117">Application</span></span>                            | <span data-ttu-id="75fc2-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75fc2-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="75fc2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75fc2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="75fc2-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="75fc2-120">Function parameters</span></span>

| <span data-ttu-id="75fc2-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="75fc2-121">Parameter</span></span>      | <span data-ttu-id="75fc2-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="75fc2-122">Type</span></span>               | <span data-ttu-id="75fc2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="75fc2-123">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="75fc2-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="75fc2-124">startDateTime</span></span>  | <span data-ttu-id="75fc2-125">Cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="75fc2-125">string (timestamp)</span></span> | <span data-ttu-id="75fc2-126">A hora de início em que as atividades serão agregadas.</span><span class="sxs-lookup"><span data-stu-id="75fc2-126">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="75fc2-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="75fc2-127">endDateTime</span></span>    | <span data-ttu-id="75fc2-128">Cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="75fc2-128">string (timestamp)</span></span> | <span data-ttu-id="75fc2-129">A hora de término sobre a qual agregar atividades.</span><span class="sxs-lookup"><span data-stu-id="75fc2-129">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="75fc2-130">interval</span><span class="sxs-lookup"><span data-stu-id="75fc2-130">interval</span></span>       | <span data-ttu-id="75fc2-131">string</span><span class="sxs-lookup"><span data-stu-id="75fc2-131">string</span></span>             | <span data-ttu-id="75fc2-132">O intervalo de agregação.</span><span class="sxs-lookup"><span data-stu-id="75fc2-132">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="75fc2-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75fc2-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="75fc2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75fc2-134">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="75fc2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="75fc2-135">Response</span></span>

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
