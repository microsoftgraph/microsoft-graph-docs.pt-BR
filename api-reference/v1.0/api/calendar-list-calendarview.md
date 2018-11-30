---
title: Listar calendarView
description: Obtenha as ocorrências, exceções e única instâncias de eventos em um modo de exibição de calendário definido por um intervalo de tempo
ms.openlocfilehash: 37f4b1e72f15e455ab611d9d9b85b18ca7bba68d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004705"
---
# <a name="list-calendarview"></a><span data-ttu-id="dcb7c-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="dcb7c-103">List calendarView</span></span>

<span data-ttu-id="dcb7c-104">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão `(../me/calendarview)` de um usuário ou grupo ou algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcb7c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcb7c-105">Permissions</span></span>
<span data-ttu-id="dcb7c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcb7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="dcb7c-108">Eventos no calendário de um usuário: Calendars.Read ou Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcb7c-108">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="dcb7c-109">Eventos no calendário de um grupo: Group.Read.All ou Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcb7c-109">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="dcb7c-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcb7c-110">HTTP request</span></span>

<span data-ttu-id="dcb7c-111">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-111">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="dcb7c-112">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-112">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="dcb7c-113">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-113">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="dcb7c-114">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="dcb7c-114">Query parameters</span></span>

<span data-ttu-id="dcb7c-115">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-115">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="dcb7c-116">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dcb7c-116">Parameter</span></span>    | <span data-ttu-id="dcb7c-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcb7c-117">Type</span></span>   |<span data-ttu-id="dcb7c-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcb7c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcb7c-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dcb7c-119">startDateTime</span></span>|<span data-ttu-id="dcb7c-120">String</span><span class="sxs-lookup"><span data-stu-id="dcb7c-120">String</span></span>|<span data-ttu-id="dcb7c-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="dcb7c-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="dcb7c-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="dcb7c-123">endDateTime</span></span>|<span data-ttu-id="dcb7c-124">String</span><span class="sxs-lookup"><span data-stu-id="dcb7c-124">String</span></span>|<span data-ttu-id="dcb7c-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="dcb7c-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="dcb7c-127">Este método também dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-127">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dcb7c-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcb7c-128">Request headers</span></span>
| <span data-ttu-id="dcb7c-129">Nome</span><span class="sxs-lookup"><span data-stu-id="dcb7c-129">Name</span></span>       | <span data-ttu-id="dcb7c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcb7c-130">Type</span></span> | <span data-ttu-id="dcb7c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcb7c-131">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="dcb7c-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcb7c-132">Authorization</span></span>  | <span data-ttu-id="dcb7c-133">string</span><span class="sxs-lookup"><span data-stu-id="dcb7c-133">string</span></span> | <span data-ttu-id="dcb7c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dcb7c-136">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="dcb7c-136">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="dcb7c-137">string</span><span class="sxs-lookup"><span data-stu-id="dcb7c-137">string</span></span> | <span data-ttu-id="dcb7c-138">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-138">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="dcb7c-139">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-139">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="dcb7c-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcb7c-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcb7c-141">Request body</span></span>
<span data-ttu-id="dcb7c-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcb7c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcb7c-143">Response</span></span>

<span data-ttu-id="dcb7c-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-144">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dcb7c-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dcb7c-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dcb7c-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcb7c-146">Request</span></span>
<span data-ttu-id="dcb7c-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="dcb7c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcb7c-148">Response</span></span>
<span data-ttu-id="dcb7c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcb7c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
