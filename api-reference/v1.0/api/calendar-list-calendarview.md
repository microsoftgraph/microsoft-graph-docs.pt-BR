---
title: Listar calendarView
description: Obter as ocorrências, exceções e instâncias únicas de eventos em uma exibição de calendário definida por um intervalo de tempo, a partir do calendário padrão do usuário,
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 21aea0bd0c9b2c99ac6b2a55796c61c7c3393e9f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264775"
---
# <a name="list-calendarview"></a><span data-ttu-id="62b69-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="62b69-103">List calendarView</span></span>

<span data-ttu-id="62b69-104">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão `(../me/calendarview)` de um usuário ou grupo ou algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="62b69-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="62b69-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="62b69-105">Permissions</span></span>
<span data-ttu-id="62b69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62b69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="62b69-108">Eventos no calendário de um usuário: Calendars.Read ou Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62b69-108">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="62b69-109">Eventos no calendário de um grupo: Group.Read.All ou Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62b69-109">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="62b69-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62b69-110">HTTP request</span></span>

<span data-ttu-id="62b69-111">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="62b69-111">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="62b69-112">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="62b69-112">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="62b69-113">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="62b69-113">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="62b69-114">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="62b69-114">Query parameters</span></span>

<span data-ttu-id="62b69-115">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="62b69-115">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="62b69-116">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="62b69-116">Parameter</span></span>    | <span data-ttu-id="62b69-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="62b69-117">Type</span></span>   |<span data-ttu-id="62b69-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="62b69-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62b69-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="62b69-119">startDateTime</span></span>|<span data-ttu-id="62b69-120">String</span><span class="sxs-lookup"><span data-stu-id="62b69-120">String</span></span>|<span data-ttu-id="62b69-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="62b69-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="62b69-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="62b69-123">endDateTime</span></span>|<span data-ttu-id="62b69-124">String</span><span class="sxs-lookup"><span data-stu-id="62b69-124">String</span></span>|<span data-ttu-id="62b69-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="62b69-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="62b69-127">Este método também dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="62b69-127">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="62b69-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62b69-128">Request headers</span></span>
| <span data-ttu-id="62b69-129">Nome</span><span class="sxs-lookup"><span data-stu-id="62b69-129">Name</span></span>       | <span data-ttu-id="62b69-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="62b69-130">Type</span></span> | <span data-ttu-id="62b69-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="62b69-131">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="62b69-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="62b69-132">Authorization</span></span>  | <span data-ttu-id="62b69-133">string</span><span class="sxs-lookup"><span data-stu-id="62b69-133">string</span></span> | <span data-ttu-id="62b69-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62b69-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="62b69-136">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="62b69-136">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="62b69-137">string</span><span class="sxs-lookup"><span data-stu-id="62b69-137">string</span></span> | <span data-ttu-id="62b69-138">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="62b69-138">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="62b69-139">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="62b69-139">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="62b69-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="62b69-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62b69-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62b69-141">Request body</span></span>
<span data-ttu-id="62b69-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62b69-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62b69-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="62b69-143">Response</span></span>

<span data-ttu-id="62b69-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62b69-144">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="62b69-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62b69-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62b69-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62b69-146">Request</span></span>
<span data-ttu-id="62b69-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62b69-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="62b69-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="62b69-148">Response</span></span>
<span data-ttu-id="62b69-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62b69-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "response": "response-value",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="62b69-152">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="62b69-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="62b69-153">C#</span><span class="sxs-lookup"><span data-stu-id="62b69-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendarview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62b69-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="62b69-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendarview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="62b69-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62b69-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_calendarview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/calendar-list-calendarview.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/calendar-list-calendarview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/calendar-list-calendarview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
