# <a name="list-instances"></a><span data-ttu-id="f1966-101">Listar instâncias</span><span class="sxs-lookup"><span data-stu-id="f1966-101">List instances</span></span>

<span data-ttu-id="f1966-p101">Obtenha as instâncias (ocorrências) de um evento para um intervalo de tempo especificado. Se o evento for do tipo `SeriesMaster`, isso retornará as exceções e ocorrências do evento no intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="f1966-p101">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1966-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1966-104">Permissions</span></span>
<span data-ttu-id="f1966-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1966-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f1966-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1966-107">Permission type</span></span>      | <span data-ttu-id="f1966-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1966-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="f1966-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1966-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f1966-110">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f1966-110">Calendars.Read</span></span>    | 
|<span data-ttu-id="f1966-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1966-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1966-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f1966-112">Calendars.Read</span></span>    | 
|<span data-ttu-id="f1966-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1966-113">Application</span></span> | <span data-ttu-id="f1966-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f1966-114">Calendars.Read</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f1966-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1966-115">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="f1966-116">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="f1966-116">Query parameters</span></span>

<span data-ttu-id="f1966-117">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="f1966-117">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="f1966-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f1966-118">Parameter</span></span>    | <span data-ttu-id="f1966-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1966-119">Type</span></span>   |<span data-ttu-id="f1966-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1966-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1966-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f1966-121">startDateTime</span></span>|<span data-ttu-id="f1966-122">String</span><span class="sxs-lookup"><span data-stu-id="f1966-122">String</span></span>|<span data-ttu-id="f1966-p103">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="f1966-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="f1966-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f1966-125">endDateTime</span></span>|<span data-ttu-id="f1966-126">String</span><span class="sxs-lookup"><span data-stu-id="f1966-126">String</span></span>|<span data-ttu-id="f1966-p104">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="f1966-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="f1966-129">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1966-129">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f1966-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1966-130">Request headers</span></span>
| <span data-ttu-id="f1966-131">Nome</span><span class="sxs-lookup"><span data-stu-id="f1966-131">Name</span></span>       | <span data-ttu-id="f1966-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1966-132">Type</span></span> | <span data-ttu-id="f1966-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1966-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f1966-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1966-134">Authorization</span></span>  | <span data-ttu-id="f1966-135">string</span><span class="sxs-lookup"><span data-stu-id="f1966-135">string</span></span>  | <span data-ttu-id="f1966-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1966-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1966-138">Preferir</span><span class="sxs-lookup"><span data-stu-id="f1966-138">Prefer</span></span> | <span data-ttu-id="f1966-139">string</span><span class="sxs-lookup"><span data-stu-id="f1966-139">string</span></span> | <span data-ttu-id="f1966-p106">outlook.timezone="Eastern Standard Time". Opcional. Use isto para especificar o fuso horário para horas de início e término na resposta. Se não especificado, a resposta retorna em UTC.</span><span class="sxs-lookup"><span data-stu-id="f1966-p106">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1966-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1966-144">Request body</span></span>
<span data-ttu-id="f1966-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1966-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1966-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1966-146">Response</span></span>

<span data-ttu-id="f1966-147">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1966-147">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1966-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1966-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1966-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1966-149">Request</span></span>
<span data-ttu-id="f1966-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1966-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="f1966-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1966-151">Response</span></span>
<span data-ttu-id="f1966-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1966-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
