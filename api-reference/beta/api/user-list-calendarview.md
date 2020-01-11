---
title: Listar calendarView
description: Obter as ocorrências, exceções e instâncias únicas de eventos em uma exibição de calendário definida por um intervalo de tempo, a partir do calendário padrão do usuário,
localization_priority: Normal
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4117fa6e0ff1d714576d894d23fa9c8ff4863413
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023086"
---
# <a name="list-calendarview"></a><span data-ttu-id="9016f-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="9016f-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9016f-104">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida por um intervalo de tempo, do calendário padrão do usuário ou grupo ou de algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="9016f-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="9016f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9016f-105">Permissions</span></span>
<span data-ttu-id="9016f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9016f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9016f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9016f-108">Permission type</span></span>      | <span data-ttu-id="9016f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9016f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9016f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9016f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9016f-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9016f-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9016f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9016f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9016f-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9016f-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9016f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9016f-114">Application</span></span> | <span data-ttu-id="9016f-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9016f-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9016f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9016f-116">HTTP request</span></span>
<span data-ttu-id="9016f-117">Um [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="9016f-117">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="9016f-118">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="9016f-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="9016f-119">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="9016f-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="9016f-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="9016f-120">Query parameters</span></span>

<span data-ttu-id="9016f-121">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="9016f-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="9016f-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9016f-122">Parameter</span></span>     | <span data-ttu-id="9016f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9016f-123">Type</span></span>   | <span data-ttu-id="9016f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9016f-124">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9016f-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9016f-125">startDateTime</span></span> | <span data-ttu-id="9016f-126">String</span><span class="sxs-lookup"><span data-stu-id="9016f-126">String</span></span> | <span data-ttu-id="9016f-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="9016f-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="9016f-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9016f-129">endDateTime</span></span>   | <span data-ttu-id="9016f-130">String</span><span class="sxs-lookup"><span data-stu-id="9016f-130">String</span></span> | <span data-ttu-id="9016f-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="9016f-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="9016f-133">Os valores de `startDateTime` e `endDateTime` são interpretados usando o deslocamento de fuso horário especificado no valor e não são afetados pelo valor do `Prefer: outlook.timezone` cabeçalho, se houver.</span><span class="sxs-lookup"><span data-stu-id="9016f-133">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="9016f-134">Se nenhum deslocamento de fuso horário for incluído no valor, será interpretado como UTC.</span><span class="sxs-lookup"><span data-stu-id="9016f-134">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="9016f-135">Este método também dá suporte a alguns [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9016f-135">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9016f-136">As propriedades **createdDateTime** e **lastModifiedDateTime** do [evento](../resources/event.md) não são compatíveis com `$select`.</span><span class="sxs-lookup"><span data-stu-id="9016f-136">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="9016f-137">Para obter os valores, basta consultar no **calendarView** sem aplicar `$select`.</span><span class="sxs-lookup"><span data-stu-id="9016f-137">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9016f-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9016f-138">Request headers</span></span>
| <span data-ttu-id="9016f-139">Nome</span><span class="sxs-lookup"><span data-stu-id="9016f-139">Name</span></span>       | <span data-ttu-id="9016f-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="9016f-140">Type</span></span> | <span data-ttu-id="9016f-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="9016f-141">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="9016f-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="9016f-142">Authorization</span></span>  | <span data-ttu-id="9016f-143">string</span><span class="sxs-lookup"><span data-stu-id="9016f-143">string</span></span> | <span data-ttu-id="9016f-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9016f-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9016f-146">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="9016f-146">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="9016f-147">string</span><span class="sxs-lookup"><span data-stu-id="9016f-147">string</span></span> | <span data-ttu-id="9016f-148">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="9016f-148">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="9016f-149">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="9016f-149">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="9016f-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9016f-150">Optional.</span></span> |
| <span data-ttu-id="9016f-151">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="9016f-151">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="9016f-152">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9016f-152">string</span></span> | <span data-ttu-id="9016f-153">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="9016f-153">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="9016f-154">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="9016f-154">Values can be "text" or "html".</span></span> <span data-ttu-id="9016f-155">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="9016f-155">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="9016f-156">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="9016f-156">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="9016f-157">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9016f-157">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9016f-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9016f-158">Request body</span></span>
<span data-ttu-id="9016f-159">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9016f-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9016f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="9016f-160">Response</span></span>

<span data-ttu-id="9016f-161">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9016f-161">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9016f-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9016f-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9016f-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9016f-163">Request</span></span>
<span data-ttu-id="9016f-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9016f-164">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9016f-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="9016f-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2020-01-01T19:00:00-08:00&endDateTime=2020-01-02T19:00:00-08:00
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9016f-166">C#</span><span class="sxs-lookup"><span data-stu-id="9016f-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9016f-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9016f-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9016f-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9016f-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9016f-169">Java</span><span class="sxs-lookup"><span data-stu-id="9016f-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9016f-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="9016f-170">Response</span></span>
<span data-ttu-id="9016f-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9016f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "calendar",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
