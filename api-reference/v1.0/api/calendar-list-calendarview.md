---
title: Listar calendarView
description: Obter as ocorrências, exceções e instâncias únicas de eventos em uma exibição de calendário definida por um intervalo de tempo, a partir do calendário padrão do usuário,
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f75d0b10a2ace16335e68957d31acfbcd030c1cd
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023079"
---
# <a name="list-calendarview"></a><span data-ttu-id="98cc5-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="98cc5-103">List calendarView</span></span>

<span data-ttu-id="98cc5-104">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida por um intervalo de tempo, do calendário padrão do usuário`(../me/calendarview)`ou de algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="98cc5-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from a user's default calendar `(../me/calendarview)` or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="98cc5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="98cc5-105">Permissions</span></span>
<span data-ttu-id="98cc5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98cc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98cc5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98cc5-108">Permission type</span></span>      | <span data-ttu-id="98cc5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98cc5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98cc5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98cc5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98cc5-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98cc5-111">Calendars.Read, Calendars.ReadWrite</span></span> |
|<span data-ttu-id="98cc5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98cc5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98cc5-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98cc5-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="98cc5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98cc5-114">Application</span></span> | <span data-ttu-id="98cc5-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98cc5-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="98cc5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98cc5-116">HTTP request</span></span>

<span data-ttu-id="98cc5-117">Um [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="98cc5-117">A user's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="98cc5-118">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="98cc5-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="98cc5-119">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="98cc5-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="98cc5-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="98cc5-120">Query parameters</span></span>

<span data-ttu-id="98cc5-121">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="98cc5-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="98cc5-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="98cc5-122">Parameter</span></span>     | <span data-ttu-id="98cc5-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="98cc5-123">Type</span></span>   | <span data-ttu-id="98cc5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="98cc5-124">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="98cc5-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="98cc5-125">startDateTime</span></span> | <span data-ttu-id="98cc5-126">String</span><span class="sxs-lookup"><span data-stu-id="98cc5-126">String</span></span> | <span data-ttu-id="98cc5-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="98cc5-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span> |
| <span data-ttu-id="98cc5-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="98cc5-129">endDateTime</span></span>   | <span data-ttu-id="98cc5-130">String</span><span class="sxs-lookup"><span data-stu-id="98cc5-130">String</span></span> | <span data-ttu-id="98cc5-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="98cc5-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>   |

<span data-ttu-id="98cc5-133">Os valores de `startDateTime` e `endDateTime` são interpretados usando o deslocamento de fuso horário especificado no valor e não são afetados pelo valor do cabeçalho `Prefer: outlook.timezone`, se presente.</span><span class="sxs-lookup"><span data-stu-id="98cc5-133">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="98cc5-134">Se nenhum deslocamento de fuso horário estiver incluído no valor, ele será interpretado como UTC.</span><span class="sxs-lookup"><span data-stu-id="98cc5-134">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="98cc5-135">Este método também dá suporte a alguns [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="98cc5-135">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="98cc5-136">As propriedades **createdDateTime** e **lastModifiedDateTime** do [evento](../resources/event.md) não são compatíveis com `$select`.</span><span class="sxs-lookup"><span data-stu-id="98cc5-136">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="98cc5-137">Para obter os valores, basta consultar no **calendarView** sem aplicar `$select`.</span><span class="sxs-lookup"><span data-stu-id="98cc5-137">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98cc5-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98cc5-138">Request headers</span></span>
| <span data-ttu-id="98cc5-139">Nome</span><span class="sxs-lookup"><span data-stu-id="98cc5-139">Name</span></span>       | <span data-ttu-id="98cc5-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="98cc5-140">Type</span></span> | <span data-ttu-id="98cc5-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="98cc5-141">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="98cc5-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="98cc5-142">Authorization</span></span>  | <span data-ttu-id="98cc5-143">string</span><span class="sxs-lookup"><span data-stu-id="98cc5-143">string</span></span> | <span data-ttu-id="98cc5-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98cc5-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="98cc5-146">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="98cc5-146">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="98cc5-147">string</span><span class="sxs-lookup"><span data-stu-id="98cc5-147">string</span></span> | <span data-ttu-id="98cc5-148">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="98cc5-148">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="98cc5-149">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="98cc5-149">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="98cc5-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="98cc5-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98cc5-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98cc5-151">Request body</span></span>
<span data-ttu-id="98cc5-152">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="98cc5-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98cc5-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="98cc5-153">Response</span></span>

<span data-ttu-id="98cc5-154">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98cc5-154">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="98cc5-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98cc5-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98cc5-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98cc5-156">Request</span></span>
<span data-ttu-id="98cc5-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98cc5-157">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="98cc5-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="98cc5-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-01-07T19:00:00-08:00
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="98cc5-159">C#</span><span class="sxs-lookup"><span data-stu-id="98cc5-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98cc5-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98cc5-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="98cc5-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98cc5-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="98cc5-162">Java</span><span class="sxs-lookup"><span data-stu-id="98cc5-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="98cc5-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="98cc5-163">Response</span></span>
<span data-ttu-id="98cc5-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98cc5-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
