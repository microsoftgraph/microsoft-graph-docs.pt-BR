# <a name="list-calendarview"></a><span data-ttu-id="04c95-101">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="04c95-101">List calendarView</span></span>

<span data-ttu-id="04c95-102">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão `(../me/calendarview)` de um usuário ou grupo ou algum outro calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="04c95-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04c95-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04c95-103">Prerequisites</span></span>
<span data-ttu-id="04c95-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="04c95-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="04c95-105">Eventos no calendário de um usuário: _Calendars.Read_ ou _Calendars.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="04c95-105">Events in a user's calendar: _Calendars.Read_ or _Calendars.ReadWrite_</span></span>
* <span data-ttu-id="04c95-106">Eventos no calendário de um grupo: _Group.Read.All_ ou _Group.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="04c95-106">Events in a group calendar: _Group.Read.All_ or _Group.ReadWrite.All_</span></span>

## <a name="http-request"></a><span data-ttu-id="04c95-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04c95-107">HTTP request</span></span>

<span data-ttu-id="04c95-108">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="04c95-108">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="04c95-109">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="04c95-109">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="04c95-110">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="04c95-110">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="04c95-111">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="04c95-111">Query parameters</span></span>

<span data-ttu-id="04c95-112">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="04c95-112">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="04c95-113">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="04c95-113">Parameter</span></span>    | <span data-ttu-id="04c95-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="04c95-114">Type</span></span>   |<span data-ttu-id="04c95-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="04c95-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04c95-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="04c95-116">startDateTime</span></span>|<span data-ttu-id="04c95-117">String</span><span class="sxs-lookup"><span data-stu-id="04c95-117">String</span></span>|<span data-ttu-id="04c95-p101">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="04c95-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="04c95-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="04c95-120">endDateTime</span></span>|<span data-ttu-id="04c95-121">String</span><span class="sxs-lookup"><span data-stu-id="04c95-121">String</span></span>|<span data-ttu-id="04c95-p102">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="04c95-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="04c95-124">Este método também dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="04c95-124">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="04c95-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04c95-125">Request headers</span></span>
| <span data-ttu-id="04c95-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04c95-126">Header</span></span>       | <span data-ttu-id="04c95-127">Valor</span><span class="sxs-lookup"><span data-stu-id="04c95-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="04c95-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="04c95-128">Authorization</span></span>  | <span data-ttu-id="04c95-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04c95-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="04c95-131">Preferir</span><span class="sxs-lookup"><span data-stu-id="04c95-131">Prefer</span></span>  | <span data-ttu-id="04c95-p104">outlook.timezone="Eastern Standard Time". Opcional. Use isto para especificar o fuso horário para horas de início e término na resposta. Se não especificado, a resposta retorna em UTC.</span><span class="sxs-lookup"><span data-stu-id="04c95-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04c95-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04c95-136">Request body</span></span>
<span data-ttu-id="04c95-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04c95-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04c95-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="04c95-138">Response</span></span>

<span data-ttu-id="04c95-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04c95-139">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04c95-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04c95-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04c95-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04c95-141">Request</span></span>
<span data-ttu-id="04c95-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04c95-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="04c95-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="04c95-143">Response</span></span>
<span data-ttu-id="04c95-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04c95-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
