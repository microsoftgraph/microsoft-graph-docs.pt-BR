---
title: Listar instâncias
description: 'Obtenha as instâncias (ocorrências) de um evento para um intervalo de tempo especificado. Se o evento for um `SeriesMaster` digitar, isto retorna o '
localization_priority: Normal
ms.openlocfilehash: 194d911b6c5ea05eb0d3f797287773c516da9ee3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811393"
---
# <a name="list-instances"></a><span data-ttu-id="944bb-104">Listar instâncias</span><span class="sxs-lookup"><span data-stu-id="944bb-104">List instances</span></span>

<span data-ttu-id="944bb-p102">Obtenha as instâncias (ocorrências) de um evento para um intervalo de tempo especificado. Se o evento for do tipo `SeriesMaster`, isso retornará as exceções e ocorrências do evento no intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="944bb-p102">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="944bb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="944bb-107">Permissions</span></span>
<span data-ttu-id="944bb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="944bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="944bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="944bb-110">Permission type</span></span>      | <span data-ttu-id="944bb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="944bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="944bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="944bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="944bb-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="944bb-113">Calendars.Read</span></span>    |
|<span data-ttu-id="944bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="944bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="944bb-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="944bb-115">Calendars.Read</span></span>    |
|<span data-ttu-id="944bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="944bb-116">Application</span></span> | <span data-ttu-id="944bb-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="944bb-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="944bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="944bb-118">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="944bb-119">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="944bb-119">Query parameters</span></span>

<span data-ttu-id="944bb-120">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="944bb-120">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="944bb-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="944bb-121">Parameter</span></span>    | <span data-ttu-id="944bb-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="944bb-122">Type</span></span>   |<span data-ttu-id="944bb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="944bb-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="944bb-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="944bb-124">startDateTime</span></span>|<span data-ttu-id="944bb-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="944bb-125">String</span></span>|<span data-ttu-id="944bb-p104">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="944bb-p104">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="944bb-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="944bb-128">endDateTime</span></span>|<span data-ttu-id="944bb-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="944bb-129">String</span></span>|<span data-ttu-id="944bb-p105">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="944bb-p105">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="944bb-132">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="944bb-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="944bb-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="944bb-133">Request headers</span></span>
| <span data-ttu-id="944bb-134">Nome</span><span class="sxs-lookup"><span data-stu-id="944bb-134">Name</span></span>       | <span data-ttu-id="944bb-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="944bb-135">Type</span></span> | <span data-ttu-id="944bb-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="944bb-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="944bb-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="944bb-137">Authorization</span></span>  | <span data-ttu-id="944bb-138">string</span><span class="sxs-lookup"><span data-stu-id="944bb-138">string</span></span> | <span data-ttu-id="944bb-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="944bb-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="944bb-141">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="944bb-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="944bb-142">string</span><span class="sxs-lookup"><span data-stu-id="944bb-142">string</span></span> | <span data-ttu-id="944bb-143">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="944bb-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="944bb-144">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="944bb-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="944bb-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="944bb-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="944bb-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="944bb-146">Request body</span></span>
<span data-ttu-id="944bb-147">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="944bb-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="944bb-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="944bb-148">Response</span></span>

<span data-ttu-id="944bb-149">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="944bb-149">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="944bb-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="944bb-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="944bb-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="944bb-151">Request</span></span>
<span data-ttu-id="944bb-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="944bb-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="944bb-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="944bb-153">Response</span></span>
<span data-ttu-id="944bb-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="944bb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
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
  "tocPath": ""
}-->
