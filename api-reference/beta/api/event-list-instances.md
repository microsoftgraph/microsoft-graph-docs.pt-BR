---
title: Listar instâncias
description: Obter as instâncias (ocorrências) de um evento para um intervalo de tempo especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e1c7b65777f878197e433853739b484550928204
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586714"
---
# <a name="list-instances"></a><span data-ttu-id="d8c23-103">Listar instâncias</span><span class="sxs-lookup"><span data-stu-id="d8c23-103">List instances</span></span>

<span data-ttu-id="d8c23-104">Obter as instâncias (ocorrências) de um evento para um intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="d8c23-104">Get the instances (occurrences) of an event for a specified time range.</span></span> 

<span data-ttu-id="d8c23-105">Se o evento for do tipo `seriesMaster`, isso retornará as exceções e ocorrências desse evento no intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="d8c23-105">If the event is a `seriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8c23-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8c23-106">Permissions</span></span>
<span data-ttu-id="d8c23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8c23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8c23-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8c23-109">Permission type</span></span>      | <span data-ttu-id="d8c23-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8c23-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8c23-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8c23-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d8c23-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d8c23-112">Calendars.Read</span></span>    |
|<span data-ttu-id="d8c23-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8c23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8c23-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d8c23-114">Calendars.Read</span></span>    |
|<span data-ttu-id="d8c23-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8c23-115">Application</span></span> | <span data-ttu-id="d8c23-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d8c23-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8c23-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8c23-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="d8c23-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="d8c23-118">Query parameters</span></span>

<span data-ttu-id="d8c23-119">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="d8c23-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="d8c23-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d8c23-120">Parameter</span></span>    | <span data-ttu-id="d8c23-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8c23-121">Type</span></span>   |<span data-ttu-id="d8c23-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8c23-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8c23-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d8c23-123">startDateTime</span></span>|<span data-ttu-id="d8c23-124">String</span><span class="sxs-lookup"><span data-stu-id="d8c23-124">String</span></span>|<span data-ttu-id="d8c23-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d8c23-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="d8c23-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d8c23-127">endDateTime</span></span>|<span data-ttu-id="d8c23-128">String</span><span class="sxs-lookup"><span data-stu-id="d8c23-128">String</span></span>|<span data-ttu-id="d8c23-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d8c23-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="d8c23-131">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d8c23-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d8c23-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8c23-132">Request headers</span></span>
| <span data-ttu-id="d8c23-133">Nome</span><span class="sxs-lookup"><span data-stu-id="d8c23-133">Name</span></span>       | <span data-ttu-id="d8c23-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8c23-134">Type</span></span> | <span data-ttu-id="d8c23-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8c23-135">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="d8c23-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8c23-136">Authorization</span></span>  | <span data-ttu-id="d8c23-137">string</span><span class="sxs-lookup"><span data-stu-id="d8c23-137">string</span></span> | <span data-ttu-id="d8c23-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8c23-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d8c23-140">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d8c23-140">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="d8c23-141">string</span><span class="sxs-lookup"><span data-stu-id="d8c23-141">string</span></span> | <span data-ttu-id="d8c23-142">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="d8c23-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="d8c23-143">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="d8c23-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d8c23-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d8c23-144">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8c23-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8c23-145">Request body</span></span>
<span data-ttu-id="d8c23-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8c23-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8c23-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8c23-147">Response</span></span>

<span data-ttu-id="d8c23-148">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8c23-148">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8c23-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8c23-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8c23-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8c23-150">Request</span></span>
<span data-ttu-id="d8c23-151">O exemplo a seguir obtém dentro do intervalo de tempo especificado as ocorrências e exceções de um evento que é o evento mestre de uma série recorrente.</span><span class="sxs-lookup"><span data-stu-id="d8c23-151">The following example gets within the specified time range the occurrences and exceptions of an event which is the master event of a recurring series.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGUzYRgWAAA="],
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGUzYRgWAAA=/instances?startDateTime=2019-04-08T09:00:00.0000000&endDateTime=2019-04-30T09:00:00.0000000&$select=subject,bodyPreview,seriesMasterId,type,recurrence,start,end
```
##### <a name="response"></a><span data-ttu-id="d8c23-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8c23-152">Response</span></span>
<span data-ttu-id="d8c23-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8c23-153">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "get_instances",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/events('AAMkAGUzYRgWAAA%3D')/instances(subject,bodyPreview,seriesMasterId,type,recurrence,start,end)",
    "value": [
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1sE1TatAAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "Changing meeting from 4/15 to 4/16.",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "exception",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-16T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-16T21:00:00.0000000",
                "timeZone": "UTC"
            }
        },
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1ru1JMcAAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "occurrence",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-08T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-08T21:00:00.0000000",
                "timeZone": "UTC"
            }
        },
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1sa1do_AAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "occurrence",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-22T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-22T21:00:00.0000000",
                "timeZone": "UTC"
            }
        },
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1sw1n3PAAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "occurrence",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-29T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-29T21:00:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d8c23-154">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d8c23-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d8c23-155">Basic</span><span class="sxs-lookup"><span data-stu-id="d8c23-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_instances-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8c23-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8c23-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_instances-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/event-list-instances.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/event-list-instances.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
