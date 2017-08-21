# <a name="list-instances"></a><span data-ttu-id="a2b8d-101">Listar instâncias</span><span class="sxs-lookup"><span data-stu-id="a2b8d-101">List instances</span></span>

<span data-ttu-id="a2b8d-p101">Obtenha as instâncias (ocorrências) de um evento para um intervalo de tempo especificado. Se o evento for do tipo `SeriesMaster`, isso retornará as exceções e ocorrências do evento no intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="a2b8d-p101">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2b8d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2b8d-104">Prerequisites</span></span>
<span data-ttu-id="a2b8d-105">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.Read*</span><span class="sxs-lookup"><span data-stu-id="a2b8d-105">One of the following **scopes** is required to execute this API: *Calendars.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="a2b8d-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2b8d-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="a2b8d-107">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="a2b8d-107">Query parameters</span></span>

<span data-ttu-id="a2b8d-108">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="a2b8d-108">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="a2b8d-109">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a2b8d-109">Parameter</span></span>    | <span data-ttu-id="a2b8d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2b8d-110">Type</span></span>   |<span data-ttu-id="a2b8d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2b8d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2b8d-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a2b8d-112">startDateTime</span></span>|<span data-ttu-id="a2b8d-113">String</span><span class="sxs-lookup"><span data-stu-id="a2b8d-113">String</span></span>|<span data-ttu-id="a2b8d-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="a2b8d-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="a2b8d-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a2b8d-116">endDateTime</span></span>|<span data-ttu-id="a2b8d-117">String</span><span class="sxs-lookup"><span data-stu-id="a2b8d-117">String</span></span>|<span data-ttu-id="a2b8d-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="a2b8d-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="a2b8d-120">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a2b8d-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a2b8d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2b8d-121">Request headers</span></span>
| <span data-ttu-id="a2b8d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a2b8d-122">Name</span></span>       | <span data-ttu-id="a2b8d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2b8d-123">Type</span></span> | <span data-ttu-id="a2b8d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2b8d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a2b8d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2b8d-125">Authorization</span></span>  | <span data-ttu-id="a2b8d-126">string</span><span class="sxs-lookup"><span data-stu-id="a2b8d-126">string</span></span>  | <span data-ttu-id="a2b8d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2b8d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2b8d-129">Preferir</span><span class="sxs-lookup"><span data-stu-id="a2b8d-129">Prefer</span></span> | <span data-ttu-id="a2b8d-130">string</span><span class="sxs-lookup"><span data-stu-id="a2b8d-130">string</span></span> | <span data-ttu-id="a2b8d-p105">outlook.timezone="Eastern Standard Time". Opcional. Use isto para especificar o fuso horário para horas de início e término na resposta. Se não especificado, a resposta retorna em UTC.</span><span class="sxs-lookup"><span data-stu-id="a2b8d-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2b8d-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2b8d-135">Request body</span></span>
<span data-ttu-id="a2b8d-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2b8d-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2b8d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2b8d-137">Response</span></span>

<span data-ttu-id="a2b8d-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2b8d-138">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a2b8d-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2b8d-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2b8d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2b8d-140">Request</span></span>
<span data-ttu-id="a2b8d-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2b8d-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="a2b8d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2b8d-142">Response</span></span>
<span data-ttu-id="a2b8d-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2b8d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
