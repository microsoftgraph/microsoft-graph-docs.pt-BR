# <a name="list-calendarview"></a><span data-ttu-id="51f79-101">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="51f79-101">List calendarView</span></span>

<span data-ttu-id="51f79-102">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão de um grupo.</span><span class="sxs-lookup"><span data-stu-id="51f79-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51f79-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51f79-103">Prerequisites</span></span>
<span data-ttu-id="51f79-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Group.Read.All* ou *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="51f79-104">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="51f79-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51f79-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="51f79-106">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="51f79-106">Query parameters</span></span>

<span data-ttu-id="51f79-107">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="51f79-107">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="51f79-108">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="51f79-108">Parameter</span></span>    | <span data-ttu-id="51f79-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="51f79-109">Type</span></span>   |<span data-ttu-id="51f79-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="51f79-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51f79-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="51f79-111">startDateTime</span></span>|<span data-ttu-id="51f79-112">String</span><span class="sxs-lookup"><span data-stu-id="51f79-112">String</span></span>|<span data-ttu-id="51f79-p101">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="51f79-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="51f79-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="51f79-115">endDateTime</span></span>|<span data-ttu-id="51f79-116">String</span><span class="sxs-lookup"><span data-stu-id="51f79-116">String</span></span>|<span data-ttu-id="51f79-p102">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="51f79-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="51f79-119">Este método também dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="51f79-119">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51f79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51f79-120">Request headers</span></span>
| <span data-ttu-id="51f79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51f79-121">Header</span></span>       | <span data-ttu-id="51f79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="51f79-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51f79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51f79-123">Authorization</span></span>  | <span data-ttu-id="51f79-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51f79-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="51f79-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="51f79-126">Prefer</span></span> | <span data-ttu-id="51f79-127">string</span><span class="sxs-lookup"><span data-stu-id="51f79-127">string</span></span> | <span data-ttu-id="51f79-p104">outlook.timezone="Eastern Standard Time". Opcional. Use isto para especificar o fuso horário para horas de início e término na resposta. Se não especificado, a resposta retorna em UTC.</span><span class="sxs-lookup"><span data-stu-id="51f79-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51f79-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51f79-132">Request body</span></span>
<span data-ttu-id="51f79-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51f79-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51f79-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="51f79-134">Response</span></span>

<span data-ttu-id="51f79-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51f79-135">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="51f79-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51f79-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51f79-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51f79-137">Request</span></span>
<span data-ttu-id="51f79-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51f79-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/calendarView
```
##### <a name="response"></a><span data-ttu-id="51f79-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="51f79-139">Response</span></span>
<span data-ttu-id="51f79-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51f79-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
