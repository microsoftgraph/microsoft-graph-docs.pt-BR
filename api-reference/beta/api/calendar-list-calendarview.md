---
title: Listar calendarView
description: Obter as ocorrências, exceções e instâncias únicas de eventos em uma exibição de calendário definida por um intervalo de tempo, a partir do calendário padrão do usuário,
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2102d3a2960196fa0d39ebf12d006e719f9372e5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047739"
---
# <a name="list-calendarview"></a><span data-ttu-id="5c38f-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="5c38f-103">List calendarView</span></span>

<span data-ttu-id="5c38f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c38f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c38f-105">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida por um intervalo de tempo, do calendário padrão do usuário`(../me/calendarview)`ou de algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="5c38f-105">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from a user's default calendar `(../me/calendarview)` or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c38f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c38f-106">Permissions</span></span>
<span data-ttu-id="5c38f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c38f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c38f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c38f-109">Permission type</span></span>      | <span data-ttu-id="5c38f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c38f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c38f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c38f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c38f-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c38f-112">Calendars.Read, Calendars.ReadWrite</span></span> |
|<span data-ttu-id="5c38f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c38f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c38f-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c38f-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5c38f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c38f-115">Application</span></span> | <span data-ttu-id="5c38f-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c38f-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c38f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c38f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="5c38f-118">Um [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="5c38f-118">A user's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="5c38f-119">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="5c38f-119">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="5c38f-120">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="5c38f-120">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="5c38f-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="5c38f-121">Query parameters</span></span>

<span data-ttu-id="5c38f-122">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="5c38f-122">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="5c38f-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5c38f-123">Parameter</span></span>     | <span data-ttu-id="5c38f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c38f-124">Type</span></span>   | <span data-ttu-id="5c38f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c38f-125">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5c38f-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5c38f-126">startDateTime</span></span> | <span data-ttu-id="5c38f-127">String</span><span class="sxs-lookup"><span data-stu-id="5c38f-127">String</span></span> | <span data-ttu-id="5c38f-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="5c38f-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="5c38f-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5c38f-130">endDateTime</span></span>   | <span data-ttu-id="5c38f-131">String</span><span class="sxs-lookup"><span data-stu-id="5c38f-131">String</span></span> | <span data-ttu-id="5c38f-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="5c38f-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="5c38f-134">Os valores de `startDateTime` e `endDateTime` são interpretados usando o deslocamento de fuso horário especificado no valor e não são afetados pelo valor do cabeçalho `Prefer: outlook.timezone`, se presente.</span><span class="sxs-lookup"><span data-stu-id="5c38f-134">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="5c38f-135">Se nenhum deslocamento de fuso horário estiver incluído no valor, ele será interpretado como UTC.</span><span class="sxs-lookup"><span data-stu-id="5c38f-135">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="5c38f-136">Este método também dá suporte a alguns [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5c38f-136">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="5c38f-137">As propriedades **createdDateTime** e **lastModifiedDateTime** do [evento](../resources/event.md) não são compatíveis com `$select`.</span><span class="sxs-lookup"><span data-stu-id="5c38f-137">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="5c38f-138">Para obter os valores, basta consultar no **calendarView** sem aplicar `$select`.</span><span class="sxs-lookup"><span data-stu-id="5c38f-138">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c38f-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c38f-139">Request headers</span></span>
| <span data-ttu-id="5c38f-140">Nome</span><span class="sxs-lookup"><span data-stu-id="5c38f-140">Name</span></span>       | <span data-ttu-id="5c38f-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c38f-141">Type</span></span> | <span data-ttu-id="5c38f-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c38f-142">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="5c38f-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c38f-143">Authorization</span></span>  | <span data-ttu-id="5c38f-144">string</span><span class="sxs-lookup"><span data-stu-id="5c38f-144">string</span></span> | <span data-ttu-id="5c38f-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c38f-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5c38f-147">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="5c38f-147">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="5c38f-148">string</span><span class="sxs-lookup"><span data-stu-id="5c38f-148">string</span></span> | <span data-ttu-id="5c38f-149">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="5c38f-149">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="5c38f-150">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="5c38f-150">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="5c38f-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5c38f-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c38f-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c38f-152">Request body</span></span>
<span data-ttu-id="5c38f-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c38f-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c38f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c38f-154">Response</span></span>

<span data-ttu-id="5c38f-155">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c38f-155">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c38f-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c38f-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c38f-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c38f-157">Request</span></span>
<span data-ttu-id="5c38f-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c38f-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c38f-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c38f-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-01-07T19:00:00-08:00
```
# <a name="c"></a>[<span data-ttu-id="5c38f-160">C#</span><span class="sxs-lookup"><span data-stu-id="5c38f-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c38f-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c38f-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c38f-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c38f-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c38f-163">Java</span><span class="sxs-lookup"><span data-stu-id="5c38f-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c38f-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c38f-164">Response</span></span>
<span data-ttu-id="5c38f-165">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c38f-165">Here is an example of the response.</span></span> <span data-ttu-id="5c38f-166">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c38f-166">Note: The response object shown here might be shortened for readability.</span></span>
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
