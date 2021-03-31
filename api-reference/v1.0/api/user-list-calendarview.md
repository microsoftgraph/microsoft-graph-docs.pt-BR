---
title: Listar calendarView
description: 'Obter as ocorrências, exceções e instâncias únicas de eventos em uma exibição de calendário definida por um intervalo de tempo, a partir do calendário padrão do usuário, '
localization_priority: Priority
doc_type: apiPageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: 5094e412de24a26e5381ae0763299760bac1699d
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51472097"
---
# <a name="list-calendarview"></a><span data-ttu-id="06b9a-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="06b9a-103">List calendarView</span></span>

<span data-ttu-id="06b9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06b9a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="06b9a-105">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida por um intervalo de tempo, do calendário padrão do usuário ou grupo ou de algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="06b9a-105">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="06b9a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="06b9a-106">Permissions</span></span>
<span data-ttu-id="06b9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06b9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06b9a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06b9a-109">Permission type</span></span>      | <span data-ttu-id="06b9a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06b9a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06b9a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06b9a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="06b9a-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06b9a-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="06b9a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06b9a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06b9a-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06b9a-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="06b9a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06b9a-115">Application</span></span> | <span data-ttu-id="06b9a-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06b9a-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="06b9a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06b9a-117">HTTP request</span></span>

<span data-ttu-id="06b9a-118">Um [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="06b9a-118">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="06b9a-119">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="06b9a-119">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="06b9a-120">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="06b9a-120">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="06b9a-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="06b9a-121">Query parameters</span></span>

<span data-ttu-id="06b9a-122">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="06b9a-122">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="06b9a-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="06b9a-123">Parameter</span></span>     | <span data-ttu-id="06b9a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="06b9a-124">Type</span></span>   | <span data-ttu-id="06b9a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="06b9a-125">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="06b9a-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="06b9a-126">startDateTime</span></span> | <span data-ttu-id="06b9a-127">String</span><span class="sxs-lookup"><span data-stu-id="06b9a-127">String</span></span> | <span data-ttu-id="06b9a-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="06b9a-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="06b9a-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="06b9a-130">endDateTime</span></span>   | <span data-ttu-id="06b9a-131">String</span><span class="sxs-lookup"><span data-stu-id="06b9a-131">String</span></span> | <span data-ttu-id="06b9a-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="06b9a-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="06b9a-134">Os valores de `startDateTime` e `endDateTime` são interpretados usando o deslocamento de fuso horário especificado no valor e não são afetados pelo valor do cabeçalho `Prefer: outlook.timezone`, se presente.</span><span class="sxs-lookup"><span data-stu-id="06b9a-134">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="06b9a-135">Se nenhum deslocamento de fuso horário estiver incluído no valor, ele será interpretado como UTC.</span><span class="sxs-lookup"><span data-stu-id="06b9a-135">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="06b9a-136">Este método também dá suporte a alguns [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="06b9a-136">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="06b9a-137">As propriedades **createdDateTime** e **lastModifiedDateTime** do [evento](../resources/event.md) não são compatíveis com `$select`.</span><span class="sxs-lookup"><span data-stu-id="06b9a-137">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="06b9a-138">Para obter os valores, basta consultar no **calendarView** sem aplicar `$select`.</span><span class="sxs-lookup"><span data-stu-id="06b9a-138">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06b9a-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06b9a-139">Request headers</span></span>
| <span data-ttu-id="06b9a-140">Nome</span><span class="sxs-lookup"><span data-stu-id="06b9a-140">Name</span></span>       | <span data-ttu-id="06b9a-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="06b9a-141">Type</span></span> | <span data-ttu-id="06b9a-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="06b9a-142">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="06b9a-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="06b9a-143">Authorization</span></span>  | <span data-ttu-id="06b9a-144">string</span><span class="sxs-lookup"><span data-stu-id="06b9a-144">string</span></span> | <span data-ttu-id="06b9a-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06b9a-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="06b9a-147">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="06b9a-147">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="06b9a-148">string</span><span class="sxs-lookup"><span data-stu-id="06b9a-148">string</span></span> | <span data-ttu-id="06b9a-149">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="06b9a-149">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="06b9a-150">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="06b9a-150">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="06b9a-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="06b9a-151">Optional.</span></span> |
| <span data-ttu-id="06b9a-152">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="06b9a-152">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="06b9a-153">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06b9a-153">string</span></span> | <span data-ttu-id="06b9a-154">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="06b9a-154">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="06b9a-155">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="06b9a-155">Values can be "text" or "html".</span></span> <span data-ttu-id="06b9a-156">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="06b9a-156">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="06b9a-157">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="06b9a-157">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="06b9a-158">Opcional.</span><span class="sxs-lookup"><span data-stu-id="06b9a-158">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06b9a-159">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06b9a-159">Request body</span></span>
<span data-ttu-id="06b9a-160">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06b9a-160">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06b9a-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="06b9a-161">Response</span></span>

<span data-ttu-id="06b9a-162">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06b9a-162">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06b9a-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06b9a-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06b9a-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06b9a-164">Request</span></span>
<span data-ttu-id="06b9a-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06b9a-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="06b9a-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="06b9a-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2020-01-01T19:00:00-08:00&endDateTime=2020-01-02T19:00:00-08:00
```
# <a name="c"></a>[<span data-ttu-id="06b9a-167">C#</span><span class="sxs-lookup"><span data-stu-id="06b9a-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06b9a-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06b9a-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06b9a-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06b9a-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06b9a-170">Java</span><span class="sxs-lookup"><span data-stu-id="06b9a-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="06b9a-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="06b9a-171">Response</span></span>
<span data-ttu-id="06b9a-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06b9a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "originalStartTimeZone": "Pacific Standard Time",
      "originalEndTimeZone": "Pacific Standard Time",
      "responseStatus": {
        "response": "accepted",
        "time": "2016-10-19T10:37:00Z"
      },
      "iCalUId": "040000008200E00074C5B7101A82E00800000000D3D70B8A6A17D70100000000000000001000000074665914A06C3F49BB4B7D7EEE4304DA",
      "reminderMinutesBeforeStart": 15,
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
