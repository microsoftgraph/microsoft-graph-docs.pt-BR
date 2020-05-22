---
author: daspek
ms.author: dspektor
title: Obter estatísticas de atividade de item por intervalo
description: Obter itemAnalyticyStats para as atividades que foram realizadas nesse recurso dentro do intervalo de tempo especificado.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f39fdcb00b367bed4044bad521b658c897fdc016
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345706"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="3ba23-103">Obter estatísticas de atividade de item por intervalo</span><span class="sxs-lookup"><span data-stu-id="3ba23-103">Get item activity stats by interval</span></span>

<span data-ttu-id="3ba23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ba23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ba23-105">Obtenha uma coleção de recursos [itemActivityStats][] para as atividades que foram realizadas nesse recurso dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="3ba23-105">Get a collection of [itemActivityStats][] resources for the activities that took place on this resource within the specified time interval.</span></span>

><span data-ttu-id="3ba23-106">**Observação:** O recurso do **naanalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="3ba23-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="3ba23-107">As agregações de análise podem não estar disponíveis para todos os tipos de ação.</span><span class="sxs-lookup"><span data-stu-id="3ba23-107">Analytics aggregates might not be available for all action types.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ba23-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ba23-108">Permissions</span></span>

<span data-ttu-id="3ba23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ba23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ba23-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ba23-111">Permission type</span></span>                        | <span data-ttu-id="3ba23-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ba23-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="3ba23-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ba23-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ba23-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ba23-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="3ba23-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ba23-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ba23-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ba23-116">Not supported.</span></span>
|<span data-ttu-id="3ba23-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ba23-117">Application</span></span>                            | <span data-ttu-id="3ba23-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ba23-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="3ba23-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ba23-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016-01-01',endDateTime='2017-05-20',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="3ba23-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3ba23-120">Function parameters</span></span>

| <span data-ttu-id="3ba23-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3ba23-121">Parameter</span></span>      | <span data-ttu-id="3ba23-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ba23-122">Type</span></span>               | <span data-ttu-id="3ba23-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ba23-123">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="3ba23-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3ba23-124">startDateTime</span></span>  | <span data-ttu-id="3ba23-125">Cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="3ba23-125">string (timestamp)</span></span> | <span data-ttu-id="3ba23-126">A hora de início em que as atividades serão agregadas.</span><span class="sxs-lookup"><span data-stu-id="3ba23-126">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="3ba23-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3ba23-127">endDateTime</span></span>    | <span data-ttu-id="3ba23-128">Cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="3ba23-128">string (timestamp)</span></span> | <span data-ttu-id="3ba23-129">A hora de término sobre a qual agregar atividades.</span><span class="sxs-lookup"><span data-stu-id="3ba23-129">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="3ba23-130">interval</span><span class="sxs-lookup"><span data-stu-id="3ba23-130">interval</span></span>       | <span data-ttu-id="3ba23-131">string</span><span class="sxs-lookup"><span data-stu-id="3ba23-131">string</span></span>             | <span data-ttu-id="3ba23-132">O intervalo de agregação.</span><span class="sxs-lookup"><span data-stu-id="3ba23-132">The aggregation interval.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="3ba23-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3ba23-133">Optional query parameters</span></span>
<span data-ttu-id="3ba23-134">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3ba23-134">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ba23-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ba23-135">Request headers</span></span>

| <span data-ttu-id="3ba23-136">Nome</span><span class="sxs-lookup"><span data-stu-id="3ba23-136">Name</span></span>      |<span data-ttu-id="3ba23-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ba23-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3ba23-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ba23-138">Authorization</span></span>  | <span data-ttu-id="3ba23-139">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="3ba23-139">Bearer {code}.</span></span> <span data-ttu-id="3ba23-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ba23-140">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ba23-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ba23-141">Request body</span></span>

<span data-ttu-id="3ba23-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ba23-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ba23-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ba23-143">Response</span></span> 

<span data-ttu-id="3ba23-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [itemActivityStats][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ba23-144">If successful, this method returns a `200 OK` response code and a collection of [itemActivityStats][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="3ba23-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ba23-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ba23-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ba23-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3ba23-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ba23-147">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="3ba23-148">C#</span><span class="sxs-lookup"><span data-stu-id="3ba23-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ba23-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ba23-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ba23-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ba23-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ba23-151">Java</span><span class="sxs-lookup"><span data-stu-id="3ba23-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activities-by-interval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3ba23-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ba23-152">Response</span></span>

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
