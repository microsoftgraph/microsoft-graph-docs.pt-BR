---
title: Listar calendarView
description: Obtenha as ocorrências, exceções e única instâncias de eventos em um modo de exibição de calendário definido por um intervalo de tempo
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8339809f212bcd4bcdb8700826397a5ca234bdd4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956827"
---
# <a name="list-calendarview"></a><span data-ttu-id="e7d11-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="e7d11-103">List calendarView</span></span>

> <span data-ttu-id="e7d11-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7d11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7d11-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7d11-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e7d11-106">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão `(../me/calendarview)` de um usuário ou grupo ou algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="e7d11-106">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7d11-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7d11-107">Permissions</span></span>
<span data-ttu-id="e7d11-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7d11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="e7d11-110">Eventos no calendário de um usuário: Calendars.Read ou Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7d11-110">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="e7d11-111">Eventos no calendário de um grupo: Group.Read.All ou Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d11-111">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="e7d11-112">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7d11-112">HTTP request</span></span>
<span data-ttu-id="e7d11-113"><!-- { "blockType": "ignored" } -->Um usuário ou do grupo padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="e7d11-113"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="e7d11-114">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="e7d11-114">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="e7d11-115">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="e7d11-115">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="e7d11-116">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="e7d11-116">Query parameters</span></span>

<span data-ttu-id="e7d11-117">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="e7d11-117">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="e7d11-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e7d11-118">Parameter</span></span>    | <span data-ttu-id="e7d11-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7d11-119">Type</span></span>   |<span data-ttu-id="e7d11-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7d11-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7d11-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e7d11-121">startDateTime</span></span>|<span data-ttu-id="e7d11-122">String</span><span class="sxs-lookup"><span data-stu-id="e7d11-122">String</span></span>|<span data-ttu-id="e7d11-p103">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="e7d11-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="e7d11-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e7d11-125">endDateTime</span></span>|<span data-ttu-id="e7d11-126">String</span><span class="sxs-lookup"><span data-stu-id="e7d11-126">String</span></span>|<span data-ttu-id="e7d11-p104">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="e7d11-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="e7d11-129">Este método também dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d11-129">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e7d11-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d11-130">Request headers</span></span>
| <span data-ttu-id="e7d11-131">Nome</span><span class="sxs-lookup"><span data-stu-id="e7d11-131">Name</span></span>       | <span data-ttu-id="e7d11-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7d11-132">Type</span></span> | <span data-ttu-id="e7d11-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7d11-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="e7d11-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7d11-134">Authorization</span></span>  | <span data-ttu-id="e7d11-135">string</span><span class="sxs-lookup"><span data-stu-id="e7d11-135">string</span></span> | <span data-ttu-id="e7d11-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7d11-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e7d11-138">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e7d11-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="e7d11-139">string</span><span class="sxs-lookup"><span data-stu-id="e7d11-139">string</span></span> | <span data-ttu-id="e7d11-140">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d11-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="e7d11-141">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="e7d11-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="e7d11-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e7d11-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7d11-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d11-143">Request body</span></span>
<span data-ttu-id="e7d11-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7d11-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7d11-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d11-145">Response</span></span>

<span data-ttu-id="e7d11-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d11-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7d11-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7d11-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7d11-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d11-148">Request</span></span>
<span data-ttu-id="e7d11-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7d11-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="e7d11-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d11-150">Response</span></span>
<span data-ttu-id="e7d11-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7d11-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
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
