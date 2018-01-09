# <a name="list-calendarview"></a><span data-ttu-id="d047a-101">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="d047a-101">List calendarView</span></span>
<span data-ttu-id="d047a-102">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão de um grupo.</span><span class="sxs-lookup"><span data-stu-id="d047a-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="d047a-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="d047a-103">Permissions</span></span>
<span data-ttu-id="d047a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d047a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d047a-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d047a-106">Permission type</span></span>      | <span data-ttu-id="d047a-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d047a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d047a-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d047a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d047a-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d047a-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d047a-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d047a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d047a-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d047a-111">Not supported.</span></span>    |
|<span data-ttu-id="d047a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d047a-112">Application</span></span> | <span data-ttu-id="d047a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d047a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d047a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d047a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="d047a-115">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="d047a-115">Query parameters</span></span>
<span data-ttu-id="d047a-116">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="d047a-116">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="d047a-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d047a-117">Parameter</span></span>    | <span data-ttu-id="d047a-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="d047a-118">Type</span></span>   |<span data-ttu-id="d047a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d047a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d047a-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d047a-120">startDateTime</span></span>|<span data-ttu-id="d047a-121">String</span><span class="sxs-lookup"><span data-stu-id="d047a-121">String</span></span>|<span data-ttu-id="d047a-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d047a-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="d047a-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d047a-124">endDateTime</span></span>|<span data-ttu-id="d047a-125">String</span><span class="sxs-lookup"><span data-stu-id="d047a-125">String</span></span>|<span data-ttu-id="d047a-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d047a-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="d047a-128">Este método também dá suporte a [Parâmetros de consulta OData](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d047a-128">This method also supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d047a-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d047a-129">Request headers</span></span>
| <span data-ttu-id="d047a-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d047a-130">Header</span></span>       | <span data-ttu-id="d047a-131">Valor</span><span class="sxs-lookup"><span data-stu-id="d047a-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d047a-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d047a-132">Authorization</span></span>  | <span data-ttu-id="d047a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d047a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d047a-135">Preferir</span><span class="sxs-lookup"><span data-stu-id="d047a-135">Prefer</span></span> | <span data-ttu-id="d047a-136">string</span><span class="sxs-lookup"><span data-stu-id="d047a-136">string</span></span> | <span data-ttu-id="d047a-p105">outlook.timezone="Eastern Standard Time". Opcional. Use isto para especificar o fuso horário para horas de início e término na resposta. Se não especificado, a resposta retorna em UTC.</span><span class="sxs-lookup"><span data-stu-id="d047a-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d047a-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d047a-141">Request body</span></span>
<span data-ttu-id="d047a-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d047a-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d047a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d047a-143">Response</span></span>
<span data-ttu-id="d047a-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d047a-144">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d047a-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d047a-145">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d047a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d047a-146">Request</span></span>
<span data-ttu-id="d047a-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d047a-147">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/calendarView
```

#### <a name="response"></a><span data-ttu-id="d047a-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d047a-148">Response</span></span>
<span data-ttu-id="d047a-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d047a-149">Here is an example of the response.</span></span>
><span data-ttu-id="d047a-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d047a-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d047a-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d047a-151">All the properties will be returned from an actual call.</span></span>
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
