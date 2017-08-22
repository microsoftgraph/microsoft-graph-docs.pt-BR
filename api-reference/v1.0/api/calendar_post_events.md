# <a name="create-event"></a><span data-ttu-id="3b29b-101">Criar evento</span><span class="sxs-lookup"><span data-stu-id="3b29b-101">Create Event</span></span>

<span data-ttu-id="3b29b-102">Use essa API para criar um novo evento no calendário especificado ou no padrão.</span><span class="sxs-lookup"><span data-stu-id="3b29b-102">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b29b-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b29b-103">Prerequisites</span></span>
<span data-ttu-id="3b29b-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="3b29b-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="3b29b-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b29b-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="3b29b-106">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="3b29b-106">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="3b29b-107">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="3b29b-107">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="3b29b-108">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="3b29b-108">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="3b29b-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b29b-109">Request headers</span></span>
| <span data-ttu-id="3b29b-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b29b-110">Header</span></span>       | <span data-ttu-id="3b29b-111">Valor</span><span class="sxs-lookup"><span data-stu-id="3b29b-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b29b-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b29b-112">Authorization</span></span>  | <span data-ttu-id="3b29b-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b29b-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3b29b-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b29b-115">Content-Type</span></span>  | <span data-ttu-id="3b29b-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b29b-p102">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b29b-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b29b-118">Request body</span></span>
<span data-ttu-id="3b29b-119">No corpo da solicitação, forneça uma representação JSON do objeto [Event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="3b29b-119">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3b29b-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b29b-120">Response</span></span>

<span data-ttu-id="3b29b-121">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b29b-121">If successful, this method returns `201, Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b29b-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b29b-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b29b-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b29b-123">Request</span></span>
<span data-ttu-id="3b29b-124">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b29b-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="3b29b-125">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="3b29b-125">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3b29b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b29b-126">Response</span></span>
<span data-ttu-id="3b29b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b29b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
