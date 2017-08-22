# <a name="list-events"></a><span data-ttu-id="f9ddf-101">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="f9ddf-101">List events</span></span>

<span data-ttu-id="f9ddf-p101">Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.</span><span class="sxs-lookup"><span data-stu-id="f9ddf-p101">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="f9ddf-104">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar_list_calendarview.md) ou [obtenha as instâncias de um evento](event_list_instances.md).</span><span class="sxs-lookup"><span data-stu-id="f9ddf-104">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9ddf-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9ddf-105">Prerequisites</span></span>
<span data-ttu-id="f9ddf-106">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.Read*</span><span class="sxs-lookup"><span data-stu-id="f9ddf-106">One of the following **scopes** is required to execute this API: *Calendars.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="f9ddf-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9ddf-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f9ddf-108">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="f9ddf-108">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="f9ddf-109">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="f9ddf-109">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="f9ddf-110">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="f9ddf-110">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9ddf-111">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f9ddf-111">Optional query parameters</span></span>
<span data-ttu-id="f9ddf-112">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f9ddf-112">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f9ddf-113">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ddf-113">Request headers</span></span>
| <span data-ttu-id="f9ddf-114">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9ddf-114">Header</span></span>       | <span data-ttu-id="f9ddf-115">Valor</span><span class="sxs-lookup"><span data-stu-id="f9ddf-115">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f9ddf-116">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9ddf-116">Authorization</span></span>  | <span data-ttu-id="f9ddf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9ddf-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f9ddf-119">Preferir</span><span class="sxs-lookup"><span data-stu-id="f9ddf-119">Prefer</span></span>  | <span data-ttu-id="f9ddf-p103">outlook.timezone="Eastern Standard Time". Opcional. Use isto para especificar o fuso horário para horas de início e término na resposta. Se não especificado, a resposta retorna em UTC.</span><span class="sxs-lookup"><span data-stu-id="f9ddf-p103">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9ddf-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ddf-124">Request body</span></span>
<span data-ttu-id="f9ddf-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9ddf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9ddf-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9ddf-126">Response</span></span>

<span data-ttu-id="f9ddf-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9ddf-127">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9ddf-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9ddf-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9ddf-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ddf-129">Request</span></span>
<span data-ttu-id="f9ddf-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9ddf-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="f9ddf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9ddf-131">Response</span></span>
<span data-ttu-id="f9ddf-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9ddf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
