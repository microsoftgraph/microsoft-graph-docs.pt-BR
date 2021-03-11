---
author: daspek
title: Obter estatísticas de atividade de item por intervalo
description: Obter itemAnalyticyStats para as atividades que ocorreram nesse recurso dentro do intervalo de tempo especificado.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e5a88a95a892d5b5e8e9404dc461e56eefaa566f
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626121"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="c68c7-103">Obter estatísticas de atividade de item por intervalo</span><span class="sxs-lookup"><span data-stu-id="c68c7-103">Get item activity stats by interval</span></span>

<span data-ttu-id="c68c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c68c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c68c7-105">Obter uma coleção de [recursos itemActivityStats][] para as atividades que ocorreram nesse recurso dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="c68c7-105">Get a collection of [itemActivityStats][] resources for the activities that took place on this resource within the specified time interval.</span></span>

><span data-ttu-id="c68c7-106">**Observação:** O **recurso itemAnalytics** ainda não está disponível em todas as [implantações nacionais.](/graph/deployments)</span><span class="sxs-lookup"><span data-stu-id="c68c7-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span> 

<span data-ttu-id="c68c7-107">Os agregados de análise podem não estar disponíveis para todos os tipos de ação.</span><span class="sxs-lookup"><span data-stu-id="c68c7-107">Analytics aggregates might not be available for all action types.</span></span>

## <a name="permissions"></a><span data-ttu-id="c68c7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c68c7-108">Permissions</span></span>

<span data-ttu-id="c68c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c68c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c68c7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c68c7-111">Permission type</span></span>                        | <span data-ttu-id="c68c7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c68c7-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="c68c7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c68c7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c68c7-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c68c7-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="c68c7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c68c7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c68c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c68c7-116">Not supported.</span></span>
|<span data-ttu-id="c68c7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c68c7-117">Application</span></span>                            | <span data-ttu-id="c68c7-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c68c7-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c68c7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c68c7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016-01-01',endDateTime='2017-05-20',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',endDateTime='2017-05-20',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="c68c7-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c68c7-120">Function parameters</span></span>

| <span data-ttu-id="c68c7-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c68c7-121">Parameter</span></span>      | <span data-ttu-id="c68c7-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="c68c7-122">Type</span></span>               | <span data-ttu-id="c68c7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c68c7-123">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="c68c7-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c68c7-124">startDateTime</span></span>  | <span data-ttu-id="c68c7-125">string (timestamp)</span><span class="sxs-lookup"><span data-stu-id="c68c7-125">string (timestamp)</span></span> | <span data-ttu-id="c68c7-126">O tempo de início sobre o qual agregar atividades.</span><span class="sxs-lookup"><span data-stu-id="c68c7-126">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="c68c7-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c68c7-127">endDateTime</span></span>    | <span data-ttu-id="c68c7-128">string (timestamp)</span><span class="sxs-lookup"><span data-stu-id="c68c7-128">string (timestamp)</span></span> | <span data-ttu-id="c68c7-129">O tempo final sobre o qual agregar atividades.</span><span class="sxs-lookup"><span data-stu-id="c68c7-129">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="c68c7-130">interval</span><span class="sxs-lookup"><span data-stu-id="c68c7-130">interval</span></span>       | <span data-ttu-id="c68c7-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c68c7-131">string</span></span>             | <span data-ttu-id="c68c7-132">O intervalo de agregação.</span><span class="sxs-lookup"><span data-stu-id="c68c7-132">The aggregation interval.</span></span>

><span data-ttu-id="c68c7-133">**Observação:** Essa API só dá suporte a um intervalo de tempo de 90 dias para contagens diárias.</span><span class="sxs-lookup"><span data-stu-id="c68c7-133">**Note:** This API only supports a time range of 90 days for daily counts.</span></span> <span data-ttu-id="c68c7-134">O valor dos parâmetros e deve representar um intervalo `startDateTime` de tempo inferior a `endDateTime` 90 dias.</span><span class="sxs-lookup"><span data-stu-id="c68c7-134">The value of the `startDateTime` and `endDateTime` parameters must represent a time range of less than 90 days.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c68c7-135">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c68c7-135">Optional query parameters</span></span>
<span data-ttu-id="c68c7-136">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c68c7-136">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c68c7-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c68c7-137">Request headers</span></span>

| <span data-ttu-id="c68c7-138">Nome</span><span class="sxs-lookup"><span data-stu-id="c68c7-138">Name</span></span>      |<span data-ttu-id="c68c7-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="c68c7-139">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c68c7-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="c68c7-140">Authorization</span></span>  | <span data-ttu-id="c68c7-141">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="c68c7-141">Bearer {code}.</span></span> <span data-ttu-id="c68c7-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c68c7-142">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c68c7-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c68c7-143">Request body</span></span>

<span data-ttu-id="c68c7-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c68c7-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c68c7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c68c7-145">Response</span></span> 

<span data-ttu-id="c68c7-146">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objeto itemActivityStats][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c68c7-146">If successful, this method returns a `200 OK` response code and a collection of [itemActivityStats][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="c68c7-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c68c7-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="c68c7-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c68c7-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c68c7-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c68c7-149">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="c68c7-150">C#</span><span class="sxs-lookup"><span data-stu-id="c68c7-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c68c7-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c68c7-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c68c7-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c68c7-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c68c7-153">Java</span><span class="sxs-lookup"><span data-stu-id="c68c7-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activities-by-interval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c68c7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="c68c7-154">Response</span></span>

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

