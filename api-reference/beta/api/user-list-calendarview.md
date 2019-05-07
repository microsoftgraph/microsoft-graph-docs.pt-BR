---
title: Listar calendarView
description: Obter as ocorrências, exceções e instâncias únicas de eventos em uma exibição de calendário definida por um intervalo de tempo, a partir do calendário padrão do usuário,
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d4372609c7f81d7f832d9bd62ed90bec4e1df05e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637504"
---
# <a name="list-calendarview"></a><span data-ttu-id="d6a2c-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="d6a2c-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6a2c-104">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida por um intervalo de tempo, do calendário padrão do usuário ou grupo ou de algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6a2c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6a2c-105">Permissions</span></span>
<span data-ttu-id="d6a2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6a2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6a2c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6a2c-108">Permission type</span></span>      | <span data-ttu-id="d6a2c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6a2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6a2c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6a2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6a2c-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6a2c-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d6a2c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6a2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6a2c-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6a2c-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d6a2c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6a2c-114">Application</span></span> | <span data-ttu-id="d6a2c-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6a2c-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6a2c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6a2c-116">HTTP request</span></span>
<span data-ttu-id="d6a2c-117">Um [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-117">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="d6a2c-118">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="d6a2c-119">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="d6a2c-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="d6a2c-120">Query parameters</span></span>

<span data-ttu-id="d6a2c-121">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="d6a2c-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d6a2c-122">Parameter</span></span>    | <span data-ttu-id="d6a2c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6a2c-123">Type</span></span>   |<span data-ttu-id="d6a2c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6a2c-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6a2c-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d6a2c-125">startDateTime</span></span>|<span data-ttu-id="d6a2c-126">String</span><span class="sxs-lookup"><span data-stu-id="d6a2c-126">String</span></span>|<span data-ttu-id="d6a2c-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d6a2c-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="d6a2c-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d6a2c-129">endDateTime</span></span>|<span data-ttu-id="d6a2c-130">String</span><span class="sxs-lookup"><span data-stu-id="d6a2c-130">String</span></span>|<span data-ttu-id="d6a2c-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d6a2c-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="d6a2c-133">Este método também dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-133">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d6a2c-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6a2c-134">Request headers</span></span>
| <span data-ttu-id="d6a2c-135">Nome</span><span class="sxs-lookup"><span data-stu-id="d6a2c-135">Name</span></span>       | <span data-ttu-id="d6a2c-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6a2c-136">Type</span></span> | <span data-ttu-id="d6a2c-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6a2c-137">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="d6a2c-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6a2c-138">Authorization</span></span>  | <span data-ttu-id="d6a2c-139">string</span><span class="sxs-lookup"><span data-stu-id="d6a2c-139">string</span></span> | <span data-ttu-id="d6a2c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d6a2c-142">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d6a2c-142">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="d6a2c-143">string</span><span class="sxs-lookup"><span data-stu-id="d6a2c-143">string</span></span> | <span data-ttu-id="d6a2c-144">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-144">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="d6a2c-145">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-145">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d6a2c-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-146">Optional.</span></span> |
| <span data-ttu-id="d6a2c-147">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="d6a2c-147">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="d6a2c-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6a2c-148">string</span></span> | <span data-ttu-id="d6a2c-149">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-149">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="d6a2c-150">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="d6a2c-150">Values can be "text" or "html".</span></span> <span data-ttu-id="d6a2c-151">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-151">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="d6a2c-152">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-152">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="d6a2c-153">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6a2c-154">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6a2c-154">Request body</span></span>
<span data-ttu-id="d6a2c-155">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6a2c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6a2c-156">Response</span></span>

<span data-ttu-id="d6a2c-157">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-157">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6a2c-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6a2c-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6a2c-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6a2c-159">Request</span></span>
<span data-ttu-id="d6a2c-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="d6a2c-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6a2c-161">Response</span></span>
<span data-ttu-id="d6a2c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6a2c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d6a2c-165">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d6a2c-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d6a2c-166">Basic</span><span class="sxs-lookup"><span data-stu-id="d6a2c-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendarview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6a2c-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6a2c-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendarview-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "calendar",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-calendarview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-calendarview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
