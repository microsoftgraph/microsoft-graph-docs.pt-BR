---
title: Listar calendarView
description: Obter as ocorrências, exceções e instâncias únicas de eventos em uma exibição de calendário definida por um intervalo de tempo, a partir do calendário padrão do usuário,
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d91456806e4e81b4b211680e85dc12aca04f3084
ms.sourcegitcommit: b198efc2391a12a840e4f1b8c42c18a55b06037f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2019
ms.locfileid: "35820665"
---
# <a name="list-calendarview"></a><span data-ttu-id="09610-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="09610-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09610-104">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão `(../me/calendarview)` de um usuário ou grupo ou algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="09610-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="09610-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="09610-105">Permissions</span></span>
<span data-ttu-id="09610-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09610-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="09610-108">Eventos no calendário de um usuário: Calendars.Read ou Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09610-108">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="09610-109">Eventos no calendário de um grupo: Group.Read.All ou Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09610-109">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="09610-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09610-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="09610-111">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="09610-111">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="09610-112">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="09610-112">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="09610-113">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="09610-113">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="09610-114">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="09610-114">Query parameters</span></span>

<span data-ttu-id="09610-115">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="09610-115">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="09610-116">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="09610-116">Parameter</span></span>    | <span data-ttu-id="09610-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="09610-117">Type</span></span>   |<span data-ttu-id="09610-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="09610-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09610-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="09610-119">startDateTime</span></span>|<span data-ttu-id="09610-120">String</span><span class="sxs-lookup"><span data-stu-id="09610-120">String</span></span>|<span data-ttu-id="09610-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="09610-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="09610-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="09610-123">endDateTime</span></span>|<span data-ttu-id="09610-124">String</span><span class="sxs-lookup"><span data-stu-id="09610-124">String</span></span>|<span data-ttu-id="09610-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="09610-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="09610-127">Este método também dá suporte a alguns dos [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="09610-127">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="09610-128">As propriedades **createdDateTime** e **lastModifiedDateTime** do [evento](../resources/event.md) não oferecem suporte `$select`.</span><span class="sxs-lookup"><span data-stu-id="09610-128">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="09610-129">Para obter seus valores, basta consultar no **calendarView** sem aplicar `$select`.</span><span class="sxs-lookup"><span data-stu-id="09610-129">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09610-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09610-130">Request headers</span></span>
| <span data-ttu-id="09610-131">Nome</span><span class="sxs-lookup"><span data-stu-id="09610-131">Name</span></span>       | <span data-ttu-id="09610-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="09610-132">Type</span></span> | <span data-ttu-id="09610-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="09610-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="09610-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="09610-134">Authorization</span></span>  | <span data-ttu-id="09610-135">string</span><span class="sxs-lookup"><span data-stu-id="09610-135">string</span></span> | <span data-ttu-id="09610-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09610-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="09610-138">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="09610-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="09610-139">string</span><span class="sxs-lookup"><span data-stu-id="09610-139">string</span></span> | <span data-ttu-id="09610-140">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="09610-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="09610-141">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="09610-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="09610-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="09610-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09610-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09610-143">Request body</span></span>
<span data-ttu-id="09610-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09610-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09610-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="09610-145">Response</span></span>

<span data-ttu-id="09610-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09610-146">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09610-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09610-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09610-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09610-148">Request</span></span>
<span data-ttu-id="09610-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09610-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="09610-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="09610-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="09610-151">C#</span><span class="sxs-lookup"><span data-stu-id="09610-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="09610-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="09610-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="09610-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="09610-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="09610-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="09610-154">Response</span></span>
<span data-ttu-id="09610-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09610-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
