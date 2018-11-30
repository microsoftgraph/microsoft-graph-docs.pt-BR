---
title: Listar calendarView
description: Obtenha as ocorrências, exceções e única instâncias de eventos em um modo de exibição de calendário definido por um intervalo de tempo de calendário, o padrão do usuário
ms.openlocfilehash: 393dd98077dffead9567115d440eb695e12dbac3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033149"
---
# <a name="list-calendarview"></a><span data-ttu-id="d45b8-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="d45b8-103">List calendarView</span></span>

> <span data-ttu-id="d45b8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d45b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d45b8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d45b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d45b8-106">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida por um intervalo de tempo, do calendário padrão do usuário ou grupo ou de algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="d45b8-106">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="d45b8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d45b8-107">Permissions</span></span>
<span data-ttu-id="d45b8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d45b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d45b8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d45b8-110">Permission type</span></span>      | <span data-ttu-id="d45b8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d45b8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d45b8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d45b8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d45b8-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d45b8-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d45b8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d45b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d45b8-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d45b8-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d45b8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d45b8-116">Application</span></span> | <span data-ttu-id="d45b8-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d45b8-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d45b8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d45b8-118">HTTP request</span></span>
<span data-ttu-id="d45b8-119">Um [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="d45b8-119">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="d45b8-120">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="d45b8-120">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="d45b8-121">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="d45b8-121">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="d45b8-122">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="d45b8-122">Query parameters</span></span>

<span data-ttu-id="d45b8-123">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="d45b8-123">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="d45b8-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d45b8-124">Parameter</span></span>    | <span data-ttu-id="d45b8-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="d45b8-125">Type</span></span>   |<span data-ttu-id="d45b8-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d45b8-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d45b8-127">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d45b8-127">startDateTime</span></span>|<span data-ttu-id="d45b8-128">String</span><span class="sxs-lookup"><span data-stu-id="d45b8-128">String</span></span>|<span data-ttu-id="d45b8-p103">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d45b8-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="d45b8-131">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d45b8-131">endDateTime</span></span>|<span data-ttu-id="d45b8-132">String</span><span class="sxs-lookup"><span data-stu-id="d45b8-132">String</span></span>|<span data-ttu-id="d45b8-p104">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d45b8-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="d45b8-135">Este método também dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d45b8-135">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d45b8-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d45b8-136">Request headers</span></span>
| <span data-ttu-id="d45b8-137">Nome</span><span class="sxs-lookup"><span data-stu-id="d45b8-137">Name</span></span>       | <span data-ttu-id="d45b8-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="d45b8-138">Type</span></span> | <span data-ttu-id="d45b8-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="d45b8-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="d45b8-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="d45b8-140">Authorization</span></span>  | <span data-ttu-id="d45b8-141">string</span><span class="sxs-lookup"><span data-stu-id="d45b8-141">string</span></span> | <span data-ttu-id="d45b8-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d45b8-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d45b8-144">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d45b8-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="d45b8-145">string</span><span class="sxs-lookup"><span data-stu-id="d45b8-145">string</span></span> | <span data-ttu-id="d45b8-146">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="d45b8-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="d45b8-147">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="d45b8-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d45b8-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d45b8-148">Optional.</span></span> |
| <span data-ttu-id="d45b8-149">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="d45b8-149">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="d45b8-150">string</span><span class="sxs-lookup"><span data-stu-id="d45b8-150">string</span></span> | <span data-ttu-id="d45b8-151">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="d45b8-151">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="d45b8-152">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="d45b8-152">Values can be "text" or "html".</span></span> <span data-ttu-id="d45b8-153">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="d45b8-153">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="d45b8-154">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="d45b8-154">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="d45b8-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d45b8-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d45b8-156">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d45b8-156">Request body</span></span>
<span data-ttu-id="d45b8-157">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d45b8-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d45b8-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d45b8-158">Response</span></span>

<span data-ttu-id="d45b8-159">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d45b8-159">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d45b8-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d45b8-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d45b8-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d45b8-161">Request</span></span>
<span data-ttu-id="d45b8-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d45b8-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="d45b8-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="d45b8-163">Response</span></span>
<span data-ttu-id="d45b8-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d45b8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "calendar",
  "section": "documentation",
  "tocPath": ""
}-->
