---
title: Listar calendarView
description: Obter as ocorrências, exceções e instâncias únicas de eventos em uma exibição de calendário definida por um intervalo de tempo, a partir do calendário padrão do usuário,
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 99e6b7c1d41b05a8141f579562cb2b9813610dee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369175"
---
# <a name="list-calendarview"></a><span data-ttu-id="4b3f2-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="4b3f2-103">List calendarView</span></span>

<span data-ttu-id="4b3f2-104">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida por um intervalo de tempo, do calendário padrão do usuário`(../me/calendarview)`ou de algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b3f2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b3f2-105">Permissions</span></span>
<span data-ttu-id="4b3f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b3f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b3f2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b3f2-108">Permission type</span></span>      | <span data-ttu-id="4b3f2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b3f2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b3f2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b3f2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b3f2-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b3f2-111">Calendars.Read, Calendars.ReadWrite</span></span> |
|<span data-ttu-id="4b3f2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b3f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b3f2-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b3f2-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4b3f2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b3f2-114">Application</span></span> | <span data-ttu-id="4b3f2-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b3f2-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b3f2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b3f2-116">HTTP request</span></span>

<span data-ttu-id="4b3f2-117">Um [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-117">A user's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="4b3f2-118">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="4b3f2-119">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="4b3f2-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="4b3f2-120">Query parameters</span></span>

<span data-ttu-id="4b3f2-121">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="4b3f2-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4b3f2-122">Parameter</span></span>    | <span data-ttu-id="4b3f2-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b3f2-123">Type</span></span>   |<span data-ttu-id="4b3f2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b3f2-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b3f2-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4b3f2-125">startDateTime</span></span>|<span data-ttu-id="4b3f2-126">String</span><span class="sxs-lookup"><span data-stu-id="4b3f2-126">String</span></span>|<span data-ttu-id="4b3f2-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="4b3f2-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="4b3f2-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4b3f2-129">endDateTime</span></span>|<span data-ttu-id="4b3f2-130">String</span><span class="sxs-lookup"><span data-stu-id="4b3f2-130">String</span></span>|<span data-ttu-id="4b3f2-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="4b3f2-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="4b3f2-133">Este método também dá suporte a alguns [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-133">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="4b3f2-134">As propriedades **createdDateTime** e **lastModifiedDateTime** do [evento](../resources/event.md) não são compatíveis com `$select`.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-134">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="4b3f2-135">Para obter os valores, basta consultar no **calendarView** sem aplicar `$select`.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-135">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b3f2-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b3f2-136">Request headers</span></span>
| <span data-ttu-id="4b3f2-137">Nome</span><span class="sxs-lookup"><span data-stu-id="4b3f2-137">Name</span></span>       | <span data-ttu-id="4b3f2-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b3f2-138">Type</span></span> | <span data-ttu-id="4b3f2-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b3f2-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="4b3f2-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b3f2-140">Authorization</span></span>  | <span data-ttu-id="4b3f2-141">string</span><span class="sxs-lookup"><span data-stu-id="4b3f2-141">string</span></span> | <span data-ttu-id="4b3f2-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4b3f2-144">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="4b3f2-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="4b3f2-145">string</span><span class="sxs-lookup"><span data-stu-id="4b3f2-145">string</span></span> | <span data-ttu-id="4b3f2-146">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="4b3f2-147">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="4b3f2-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b3f2-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b3f2-149">Request body</span></span>
<span data-ttu-id="4b3f2-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b3f2-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b3f2-151">Response</span></span>

<span data-ttu-id="4b3f2-152">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-152">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4b3f2-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b3f2-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b3f2-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b3f2-154">Request</span></span>
<span data-ttu-id="4b3f2-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-155">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4b3f2-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b3f2-156">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4b3f2-157">C#</span><span class="sxs-lookup"><span data-stu-id="4b3f2-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b3f2-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b3f2-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4b3f2-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b3f2-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4b3f2-160">Java</span><span class="sxs-lookup"><span data-stu-id="4b3f2-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4b3f2-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b3f2-161">Response</span></span>
<span data-ttu-id="4b3f2-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b3f2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
