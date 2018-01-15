# <a name="list-calendarview"></a><span data-ttu-id="d6980-101">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="d6980-101">List calendarView</span></span>

<span data-ttu-id="d6980-102">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão `(../me/calendarview)` de um usuário ou grupo ou algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="d6980-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6980-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6980-103">Permissions</span></span>
<span data-ttu-id="d6980-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d6980-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

* <span data-ttu-id="d6980-106">Eventos no calendário de um usuário: Calendars.Read ou Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6980-106">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="d6980-107">Eventos no calendário de um grupo: Group.Read.All ou Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6980-107">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d6980-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6980-108">HTTP request</span></span>

<span data-ttu-id="d6980-109">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="d6980-109">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="d6980-110">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="d6980-110">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="d6980-111">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="d6980-111">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="d6980-112">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="d6980-112">Query parameters</span></span>

<span data-ttu-id="d6980-113">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="d6980-113">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="d6980-114">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d6980-114">Parameter</span></span>    | <span data-ttu-id="d6980-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6980-115">Type</span></span>   |<span data-ttu-id="d6980-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6980-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6980-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d6980-117">startDateTime</span></span>|<span data-ttu-id="d6980-118">String</span><span class="sxs-lookup"><span data-stu-id="d6980-118">String</span></span>|<span data-ttu-id="d6980-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d6980-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="d6980-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d6980-121">endDateTime</span></span>|<span data-ttu-id="d6980-122">String</span><span class="sxs-lookup"><span data-stu-id="d6980-122">String</span></span>|<span data-ttu-id="d6980-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d6980-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="d6980-125">Este método também dá suporte a [Parâmetros de consulta OData]((http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters)) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d6980-125">This method also supports the [OData Query Parameters]((http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d6980-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6980-126">Request headers</span></span>
| <span data-ttu-id="d6980-127">Nome</span><span class="sxs-lookup"><span data-stu-id="d6980-127">Name</span></span>       | <span data-ttu-id="d6980-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6980-128">Type</span></span> | <span data-ttu-id="d6980-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6980-129">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="d6980-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6980-130">Authorization</span></span>  | <span data-ttu-id="d6980-131">string</span><span class="sxs-lookup"><span data-stu-id="d6980-131">string</span></span> | <span data-ttu-id="d6980-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6980-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d6980-134">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d6980-134">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="d6980-135">string</span><span class="sxs-lookup"><span data-stu-id="d6980-135">string</span></span> | <span data-ttu-id="d6980-136">Use isto para especificar o fuso horário das horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="d6980-136">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> <span data-ttu-id="d6980-137">Quando não especificado, esses valores de tempo são retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="d6980-137">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d6980-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d6980-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6980-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6980-139">Request body</span></span>
<span data-ttu-id="d6980-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6980-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6980-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6980-141">Response</span></span>

<span data-ttu-id="d6980-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6980-142">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6980-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6980-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6980-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6980-144">Request</span></span>
<span data-ttu-id="d6980-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6980-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="d6980-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6980-146">Response</span></span>
<span data-ttu-id="d6980-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6980-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
