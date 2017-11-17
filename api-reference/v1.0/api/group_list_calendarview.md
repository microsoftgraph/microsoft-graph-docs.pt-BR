# <a name="list-calendarview"></a><span data-ttu-id="1739b-101">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="1739b-101">List calendarView</span></span>

<span data-ttu-id="1739b-102">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão de um grupo.</span><span class="sxs-lookup"><span data-stu-id="1739b-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>
## <a name="permissions"></a><span data-ttu-id="1739b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="1739b-103">Permissions</span></span>
<span data-ttu-id="1739b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1739b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1739b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1739b-106">Permission type</span></span>      | <span data-ttu-id="1739b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1739b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1739b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1739b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1739b-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1739b-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1739b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1739b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1739b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1739b-111">Not supported.</span></span>    |
|<span data-ttu-id="1739b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1739b-112">Application</span></span> | <span data-ttu-id="1739b-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1739b-113">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1739b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1739b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="1739b-115">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="1739b-115">Query parameters</span></span>

<span data-ttu-id="1739b-116">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="1739b-116">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="1739b-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1739b-117">Parameter</span></span>    | <span data-ttu-id="1739b-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="1739b-118">Type</span></span>   |<span data-ttu-id="1739b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1739b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1739b-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1739b-120">startDateTime</span></span>|<span data-ttu-id="1739b-121">String</span><span class="sxs-lookup"><span data-stu-id="1739b-121">String</span></span>|<span data-ttu-id="1739b-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="1739b-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="1739b-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1739b-124">endDateTime</span></span>|<span data-ttu-id="1739b-125">String</span><span class="sxs-lookup"><span data-stu-id="1739b-125">String</span></span>|<span data-ttu-id="1739b-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="1739b-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="1739b-128">Este método também dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1739b-128">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1739b-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1739b-129">Request headers</span></span>
| <span data-ttu-id="1739b-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1739b-130">Header</span></span>       | <span data-ttu-id="1739b-131">Valor</span><span class="sxs-lookup"><span data-stu-id="1739b-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1739b-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="1739b-132">Authorization</span></span>  | <span data-ttu-id="1739b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1739b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1739b-135">Preferir</span><span class="sxs-lookup"><span data-stu-id="1739b-135">Prefer</span></span> | <span data-ttu-id="1739b-136">string</span><span class="sxs-lookup"><span data-stu-id="1739b-136">string</span></span> | <span data-ttu-id="1739b-p105">outlook.timezone="Eastern Standard Time". Opcional. Use isto para especificar o fuso horário para horas de início e término na resposta. Se não especificado, a resposta retorna em UTC.</span><span class="sxs-lookup"><span data-stu-id="1739b-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1739b-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1739b-141">Request body</span></span>
<span data-ttu-id="1739b-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1739b-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1739b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1739b-143">Response</span></span>

<span data-ttu-id="1739b-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1739b-144">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1739b-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1739b-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1739b-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1739b-146">Request</span></span>
<span data-ttu-id="1739b-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1739b-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/calendarView
```
##### <a name="response"></a><span data-ttu-id="1739b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1739b-148">Response</span></span>
<span data-ttu-id="1739b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1739b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
