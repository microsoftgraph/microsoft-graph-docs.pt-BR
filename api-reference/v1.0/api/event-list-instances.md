---
title: Listar instâncias
description: Obter as instâncias (ocorrências) de um evento para um intervalo de tempo especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 272aafdc53f117d710349a231b8e3bbca3415e1a
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720932"
---
# <a name="list-instances"></a><span data-ttu-id="091bf-103">Listar instâncias</span><span class="sxs-lookup"><span data-stu-id="091bf-103">List instances</span></span>

<span data-ttu-id="091bf-104">Obter as instâncias (ocorrências) de um evento para um intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="091bf-104">Get the instances (occurrences) of an event for a specified time range.</span></span> 

<span data-ttu-id="091bf-105">Se o evento for do tipo `seriesMaster`, isso retornará as exceções e ocorrências desse evento no intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="091bf-105">If the event is a `seriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="091bf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="091bf-106">Permissions</span></span>
<span data-ttu-id="091bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="091bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="091bf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="091bf-109">Permission type</span></span>      | <span data-ttu-id="091bf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="091bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="091bf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="091bf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="091bf-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="091bf-112">Calendars.Read</span></span>    |
|<span data-ttu-id="091bf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="091bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="091bf-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="091bf-114">Calendars.Read</span></span>    |
|<span data-ttu-id="091bf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="091bf-115">Application</span></span> | <span data-ttu-id="091bf-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="091bf-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="091bf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="091bf-117">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="091bf-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="091bf-118">Query parameters</span></span>

<span data-ttu-id="091bf-119">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="091bf-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="091bf-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="091bf-120">Parameter</span></span>    | <span data-ttu-id="091bf-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="091bf-121">Type</span></span>   |<span data-ttu-id="091bf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="091bf-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="091bf-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="091bf-123">startDateTime</span></span>|<span data-ttu-id="091bf-124">String</span><span class="sxs-lookup"><span data-stu-id="091bf-124">String</span></span>|<span data-ttu-id="091bf-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="091bf-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="091bf-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="091bf-127">endDateTime</span></span>|<span data-ttu-id="091bf-128">String</span><span class="sxs-lookup"><span data-stu-id="091bf-128">String</span></span>|<span data-ttu-id="091bf-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="091bf-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="091bf-131">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="091bf-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="091bf-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="091bf-132">Request headers</span></span>
| <span data-ttu-id="091bf-133">Nome</span><span class="sxs-lookup"><span data-stu-id="091bf-133">Name</span></span>       | <span data-ttu-id="091bf-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="091bf-134">Type</span></span> | <span data-ttu-id="091bf-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="091bf-135">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="091bf-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="091bf-136">Authorization</span></span>  | <span data-ttu-id="091bf-137">string</span><span class="sxs-lookup"><span data-stu-id="091bf-137">string</span></span> | <span data-ttu-id="091bf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="091bf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="091bf-140">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="091bf-140">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="091bf-141">string</span><span class="sxs-lookup"><span data-stu-id="091bf-141">string</span></span> | <span data-ttu-id="091bf-142">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="091bf-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="091bf-143">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="091bf-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="091bf-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="091bf-144">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="091bf-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="091bf-145">Request body</span></span>
<span data-ttu-id="091bf-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="091bf-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="091bf-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="091bf-147">Response</span></span>

<span data-ttu-id="091bf-148">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="091bf-148">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="091bf-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="091bf-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="091bf-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="091bf-150">Request</span></span>
<span data-ttu-id="091bf-151">O exemplo a seguir obtém dentro do intervalo de tempo especificado as ocorrências e exceções de um evento que é o evento mestre de uma série recorrente.</span><span class="sxs-lookup"><span data-stu-id="091bf-151">The following example gets within the specified time range the occurrences and exceptions of an event which is the master event of a recurring series.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="091bf-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="091bf-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGUzYRgWAAA="],
  "name": "get_instances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGUzYRgWAAA=/instances?startDateTime=2019-04-08T09:00:00.0000000&endDateTime=2019-04-30T09:00:00.0000000&$select=subject,bodyPreview,seriesMasterId,type,recurrence,start,end
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="091bf-153">C#</span><span class="sxs-lookup"><span data-stu-id="091bf-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-instances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="091bf-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="091bf-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-instances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="091bf-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="091bf-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-instances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="091bf-156">Java</span><span class="sxs-lookup"><span data-stu-id="091bf-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-instances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="091bf-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="091bf-157">Response</span></span>
<span data-ttu-id="091bf-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="091bf-158">Here is an example of the response.</span></span> 
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
