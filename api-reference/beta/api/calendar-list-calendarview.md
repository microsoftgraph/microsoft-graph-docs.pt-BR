---
title: Listar calendarView
description: Obter as ocorrências, exceções e instâncias únicas de eventos em uma exibição de calendário definida por um intervalo de tempo, a partir do calendário padrão do usuário,
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e951fb8fdf06d2fa6cf3edd312fb7843ae24d8aa
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419125"
---
# <a name="list-calendarview"></a><span data-ttu-id="0f5df-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="0f5df-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f5df-104">Obtenha as ocorrências, exceções e instâncias únicas de eventos em uma exibição de calendário definida por um intervalo de tempo, do calendário `(../me/calendarview)` padrão de um usuário ou de algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f5df-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from a user's default calendar `(../me/calendarview)` or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f5df-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f5df-105">Permissions</span></span>
<span data-ttu-id="0f5df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f5df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f5df-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f5df-108">Permission type</span></span>      | <span data-ttu-id="0f5df-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f5df-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f5df-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f5df-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f5df-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f5df-111">Calendars.Read, Calendars.ReadWrite</span></span> |
|<span data-ttu-id="0f5df-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f5df-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f5df-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f5df-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0f5df-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f5df-114">Application</span></span> | <span data-ttu-id="0f5df-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f5df-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f5df-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f5df-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0f5df-117">Um [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f5df-117">A user's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="0f5df-118">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="0f5df-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="0f5df-119">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="0f5df-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="0f5df-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="0f5df-120">Query parameters</span></span>

<span data-ttu-id="0f5df-121">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="0f5df-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="0f5df-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0f5df-122">Parameter</span></span>    | <span data-ttu-id="0f5df-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f5df-123">Type</span></span>   |<span data-ttu-id="0f5df-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f5df-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f5df-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0f5df-125">startDateTime</span></span>|<span data-ttu-id="0f5df-126">String</span><span class="sxs-lookup"><span data-stu-id="0f5df-126">String</span></span>|<span data-ttu-id="0f5df-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="0f5df-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="0f5df-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0f5df-129">endDateTime</span></span>|<span data-ttu-id="0f5df-130">String</span><span class="sxs-lookup"><span data-stu-id="0f5df-130">String</span></span>|<span data-ttu-id="0f5df-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="0f5df-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="0f5df-133">Este método também dá suporte a alguns dos [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0f5df-133">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="0f5df-134">As propriedades **createdDateTime** e **lastModifiedDateTime** do [evento](../resources/event.md) não oferecem suporte `$select`.</span><span class="sxs-lookup"><span data-stu-id="0f5df-134">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="0f5df-135">Para obter seus valores, basta consultar no **calendarView** sem aplicar `$select`.</span><span class="sxs-lookup"><span data-stu-id="0f5df-135">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f5df-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f5df-136">Request headers</span></span>
| <span data-ttu-id="0f5df-137">Nome</span><span class="sxs-lookup"><span data-stu-id="0f5df-137">Name</span></span>       | <span data-ttu-id="0f5df-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f5df-138">Type</span></span> | <span data-ttu-id="0f5df-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f5df-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="0f5df-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f5df-140">Authorization</span></span>  | <span data-ttu-id="0f5df-141">string</span><span class="sxs-lookup"><span data-stu-id="0f5df-141">string</span></span> | <span data-ttu-id="0f5df-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f5df-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0f5df-144">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="0f5df-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="0f5df-145">string</span><span class="sxs-lookup"><span data-stu-id="0f5df-145">string</span></span> | <span data-ttu-id="0f5df-146">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="0f5df-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="0f5df-147">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="0f5df-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="0f5df-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0f5df-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f5df-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f5df-149">Request body</span></span>
<span data-ttu-id="0f5df-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0f5df-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f5df-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f5df-151">Response</span></span>

<span data-ttu-id="0f5df-152">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f5df-152">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f5df-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f5df-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f5df-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f5df-154">Request</span></span>
<span data-ttu-id="0f5df-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f5df-155">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0f5df-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f5df-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0f5df-157">C#</span><span class="sxs-lookup"><span data-stu-id="0f5df-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f5df-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f5df-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0f5df-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0f5df-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0f5df-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f5df-160">Response</span></span>
<span data-ttu-id="0f5df-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f5df-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
