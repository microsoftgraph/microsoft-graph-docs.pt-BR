# <a name="list-calendarview"></a><span data-ttu-id="26e52-101">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="26e52-101">List calendarView</span></span>

<span data-ttu-id="26e52-102">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida por um intervalo de tempo, do calendário padrão do usuário ou grupo ou de algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="26e52-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="26e52-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="26e52-103">Permissions</span></span>
<span data-ttu-id="26e52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="26e52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="26e52-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26e52-106">Permission type</span></span>      | <span data-ttu-id="26e52-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26e52-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26e52-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26e52-108">Delegated (work or school account)</span></span> | <span data-ttu-id="26e52-109">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26e52-109">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="26e52-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26e52-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26e52-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26e52-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="26e52-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26e52-112">Application</span></span> | <span data-ttu-id="26e52-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26e52-113">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="26e52-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26e52-114">HTTP request</span></span>

<span data-ttu-id="26e52-115">Um [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="26e52-115">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="26e52-116">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="26e52-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="26e52-117">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="26e52-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="26e52-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="26e52-118">Query parameters</span></span>

<span data-ttu-id="26e52-119">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="26e52-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="26e52-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="26e52-120">Parameter</span></span>    | <span data-ttu-id="26e52-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="26e52-121">Type</span></span>   |<span data-ttu-id="26e52-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="26e52-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26e52-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="26e52-123">startDateTime</span></span>|<span data-ttu-id="26e52-124">String</span><span class="sxs-lookup"><span data-stu-id="26e52-124">String</span></span>|<span data-ttu-id="26e52-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="26e52-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="26e52-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="26e52-127">endDateTime</span></span>|<span data-ttu-id="26e52-128">String</span><span class="sxs-lookup"><span data-stu-id="26e52-128">String</span></span>|<span data-ttu-id="26e52-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="26e52-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="26e52-131">Este método também dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="26e52-131">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="26e52-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26e52-132">Request headers</span></span>
| <span data-ttu-id="26e52-133">Nome</span><span class="sxs-lookup"><span data-stu-id="26e52-133">Name</span></span>       | <span data-ttu-id="26e52-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="26e52-134">Type</span></span> | <span data-ttu-id="26e52-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="26e52-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="26e52-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="26e52-136">Authorization</span></span>  | <span data-ttu-id="26e52-137">string</span><span class="sxs-lookup"><span data-stu-id="26e52-137">string</span></span>  | <span data-ttu-id="26e52-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26e52-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26e52-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26e52-140">Content-Type</span></span>   | <span data-ttu-id="26e52-141">string</span><span class="sxs-lookup"><span data-stu-id="26e52-141">string</span></span>  | <span data-ttu-id="26e52-142">application/json</span><span class="sxs-lookup"><span data-stu-id="26e52-142">application/json</span></span> |
| <span data-ttu-id="26e52-143">Preferir</span><span class="sxs-lookup"><span data-stu-id="26e52-143">Prefer</span></span> | <span data-ttu-id="26e52-144">string</span><span class="sxs-lookup"><span data-stu-id="26e52-144">string</span></span> | <span data-ttu-id="26e52-p105">outlook.timezone="Eastern Standard Time". Opcional. Use isto para especificar o fuso horário para horas de início e término na resposta. Se não especificado, a resposta retorna em UTC.</span><span class="sxs-lookup"><span data-stu-id="26e52-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26e52-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26e52-149">Request body</span></span>
<span data-ttu-id="26e52-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26e52-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26e52-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="26e52-151">Response</span></span>

<span data-ttu-id="26e52-152">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26e52-152">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="26e52-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26e52-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26e52-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26e52-154">Request</span></span>
<span data-ttu-id="26e52-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26e52-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="26e52-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="26e52-156">Response</span></span>
<span data-ttu-id="26e52-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26e52-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
