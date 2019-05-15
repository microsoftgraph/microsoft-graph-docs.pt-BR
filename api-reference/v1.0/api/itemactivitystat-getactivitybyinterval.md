---
author: daspek
ms.author: dspektor
title: Obter estatísticas de atividade de item por intervalo
description: Obter itemAnalyticyStats para as atividades que foram realizadas nesse recurso dentro do intervalo de tempo especificado.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2f8f2a449ddb730b31275ba2789fb14ea4f279b6
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970587"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="d796a-103">Obter estatísticas de atividade de item por intervalo</span><span class="sxs-lookup"><span data-stu-id="d796a-103">Get item activity stats by interval</span></span>

<span data-ttu-id="d796a-104">Obtenha uma coleção de recursos [itemActivityStats][] para as atividades que foram realizadas nesse recurso dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="d796a-104">Get a collection of [itemActivityStats][] resources for the activities that took place on this resource within the specified time interval.</span></span>

><span data-ttu-id="d796a-105">**Observação:** O \*\*\*\* recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="d796a-105">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="d796a-106">As agregações de análise podem não estar disponíveis para todos os tipos de ação.</span><span class="sxs-lookup"><span data-stu-id="d796a-106">Analytics aggregates might not be available for all action types.</span></span>

## <a name="permissions"></a><span data-ttu-id="d796a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d796a-107">Permissions</span></span>

<span data-ttu-id="d796a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d796a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d796a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d796a-110">Permission type</span></span>                        | <span data-ttu-id="d796a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d796a-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d796a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d796a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d796a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d796a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="d796a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d796a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d796a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d796a-115">Not supported.</span></span>
|<span data-ttu-id="d796a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d796a-116">Application</span></span>                            | <span data-ttu-id="d796a-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d796a-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d796a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d796a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="d796a-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d796a-119">Function parameters</span></span>

| <span data-ttu-id="d796a-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d796a-120">Parameter</span></span>      | <span data-ttu-id="d796a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d796a-121">Type</span></span>               | <span data-ttu-id="d796a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d796a-122">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="d796a-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d796a-123">startDateTime</span></span>  | <span data-ttu-id="d796a-124">Cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="d796a-124">string (timestamp)</span></span> | <span data-ttu-id="d796a-125">A hora de início em que as atividades serão agregadas.</span><span class="sxs-lookup"><span data-stu-id="d796a-125">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="d796a-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d796a-126">endDateTime</span></span>    | <span data-ttu-id="d796a-127">Cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="d796a-127">string (timestamp)</span></span> | <span data-ttu-id="d796a-128">A hora de término sobre a qual agregar atividades.</span><span class="sxs-lookup"><span data-stu-id="d796a-128">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="d796a-129">interval</span><span class="sxs-lookup"><span data-stu-id="d796a-129">interval</span></span>       | <span data-ttu-id="d796a-130">string</span><span class="sxs-lookup"><span data-stu-id="d796a-130">string</span></span>             | <span data-ttu-id="d796a-131">O intervalo de agregação.</span><span class="sxs-lookup"><span data-stu-id="d796a-131">The aggregation interval.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="d796a-132">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d796a-132">Optional query parameters</span></span>
<span data-ttu-id="d796a-133">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d796a-133">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d796a-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d796a-134">Request headers</span></span>

| <span data-ttu-id="d796a-135">Nome</span><span class="sxs-lookup"><span data-stu-id="d796a-135">Name</span></span>      |<span data-ttu-id="d796a-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d796a-136">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d796a-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="d796a-137">Authorization</span></span>  | <span data-ttu-id="d796a-138">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="d796a-138">Bearer {code}.</span></span> <span data-ttu-id="d796a-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d796a-139">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d796a-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d796a-140">Request body</span></span>

<span data-ttu-id="d796a-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d796a-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d796a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d796a-142">Response</span></span> 

<span data-ttu-id="d796a-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [itemActivityStats][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d796a-143">If successful, this method returns a `200 OK` response code and a collection of [itemActivityStats][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="d796a-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d796a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="d796a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d796a-145">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

### <a name="response"></a><span data-ttu-id="d796a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d796a-146">Response</span></span>

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
[itemActivityStats]: ../resources/itemactivitystat.md

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
