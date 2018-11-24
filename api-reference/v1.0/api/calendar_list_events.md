# <a name="list-events"></a><span data-ttu-id="0d55b-101">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="0d55b-101">List events</span></span>

<span data-ttu-id="0d55b-p101">Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.</span><span class="sxs-lookup"><span data-stu-id="0d55b-p101">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="0d55b-104">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar_list_calendarview.md) ou [obtenha as instâncias de um evento](event_list_instances.md).</span><span class="sxs-lookup"><span data-stu-id="0d55b-104">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d55b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d55b-105">Permissions</span></span>
<span data-ttu-id="0d55b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0d55b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0d55b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d55b-108">Permission type</span></span>      | <span data-ttu-id="0d55b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d55b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d55b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d55b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0d55b-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0d55b-111">Calendars.Read</span></span>    |
|<span data-ttu-id="0d55b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d55b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d55b-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0d55b-113">Calendars.Read</span></span>    |
|<span data-ttu-id="0d55b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d55b-114">Application</span></span> | <span data-ttu-id="0d55b-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0d55b-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d55b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d55b-116">HTTP request</span></span>
<span data-ttu-id="0d55b-117"><!-- { "blockType": "ignored" } -->Um usuário ou do grupo padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="0d55b-117"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="0d55b-118">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="0d55b-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="0d55b-119">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="0d55b-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0d55b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0d55b-120">Optional query parameters</span></span>
<span data-ttu-id="0d55b-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0d55b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0d55b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d55b-122">Request headers</span></span>
| <span data-ttu-id="0d55b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="0d55b-123">Name</span></span>       | <span data-ttu-id="0d55b-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d55b-124">Type</span></span> | <span data-ttu-id="0d55b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d55b-125">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="0d55b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d55b-126">Authorization</span></span>  | <span data-ttu-id="0d55b-127">string</span><span class="sxs-lookup"><span data-stu-id="0d55b-127">string</span></span> | <span data-ttu-id="0d55b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d55b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0d55b-130">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="0d55b-130">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="0d55b-131">string</span><span class="sxs-lookup"><span data-stu-id="0d55b-131">string</span></span> | <span data-ttu-id="0d55b-132">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="0d55b-132">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="0d55b-133">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="0d55b-133">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="0d55b-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0d55b-134">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d55b-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d55b-135">Request body</span></span>
<span data-ttu-id="0d55b-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d55b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d55b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d55b-137">Response</span></span>

<span data-ttu-id="0d55b-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d55b-138">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d55b-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d55b-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d55b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d55b-140">Request</span></span>
<span data-ttu-id="0d55b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d55b-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="0d55b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d55b-142">Response</span></span>
<span data-ttu-id="0d55b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d55b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
