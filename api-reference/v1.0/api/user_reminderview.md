# <a name="user-reminderview"></a><span data-ttu-id="b9990-101">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="b9990-101">user: reminderView</span></span>
<span data-ttu-id="b9990-102">Retorne uma lista de lembretes de calendário nas horas de início e término especificadas.</span><span class="sxs-lookup"><span data-stu-id="b9990-102">Return a list of calendar reminders within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b9990-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9990-103">Permissions</span></span>
<span data-ttu-id="b9990-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9990-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9990-106">Permission type</span></span>      | <span data-ttu-id="b9990-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9990-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9990-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9990-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b9990-109">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9990-109">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b9990-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9990-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9990-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9990-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b9990-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9990-112">Application</span></span> | <span data-ttu-id="b9990-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9990-113">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9990-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9990-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="b9990-115">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b9990-115">Function Parameters</span></span>
<span data-ttu-id="b9990-116">Forneça os seguintes parâmetros de função com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="b9990-116">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="b9990-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9990-117">Parameter</span></span>    | <span data-ttu-id="b9990-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9990-118">Type</span></span>   |<span data-ttu-id="b9990-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9990-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9990-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b9990-120">startDateTime</span></span>|<span data-ttu-id="b9990-121">String</span><span class="sxs-lookup"><span data-stu-id="b9990-121">String</span></span>|<span data-ttu-id="b9990-p102">A data e hora de início do evento para o qual o lembrete está definido. O valor é representado no formato ISO 8601, por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="b9990-p102">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="b9990-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b9990-124">endDateTime</span></span>|<span data-ttu-id="b9990-125">String</span><span class="sxs-lookup"><span data-stu-id="b9990-125">String</span></span>|<span data-ttu-id="b9990-p103">A data e hora de término do evento para o qual o lembrete está definido. O valor é representado no formato ISO 8601, por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="b9990-p103">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b9990-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9990-128">Request headers</span></span>
| <span data-ttu-id="b9990-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9990-129">Header</span></span>       | <span data-ttu-id="b9990-130">Valor</span><span class="sxs-lookup"><span data-stu-id="b9990-130">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b9990-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9990-131">Authorization</span></span>  | <span data-ttu-id="b9990-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9990-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b9990-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9990-134">Content-Type</span></span>   | <span data-ttu-id="b9990-135">application/json</span><span class="sxs-lookup"><span data-stu-id="b9990-135">application/json</span></span> |
| <span data-ttu-id="b9990-136">Preferir</span><span class="sxs-lookup"><span data-stu-id="b9990-136">Prefer</span></span> | <span data-ttu-id="b9990-p105">{Time-zone}. Opcional, supõe-se o UTC se estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="b9990-p105">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9990-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9990-139">Request body</span></span>
<span data-ttu-id="b9990-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9990-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9990-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9990-141">Response</span></span>

<span data-ttu-id="b9990-142">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [reminder](../resources/reminder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9990-142">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9990-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9990-143">Example</span></span>
<span data-ttu-id="b9990-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b9990-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9990-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9990-145">Request</span></span>
<span data-ttu-id="b9990-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9990-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```

##### <a name="response"></a><span data-ttu-id="b9990-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9990-147">Response</span></span>
<span data-ttu-id="b9990-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9990-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reminder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 673

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.reminder)",
    "value": [
        {
            "eventId": "AAMkADNsvAAA=",
            "changeKey": "SuFHwDRP1EeXJUopWbSLlgAAmBvk2g==",
            "eventSubject": "Plan summer company picnic",
            "eventWebLink": "https://outlook.office365.com/owa/?itemid=AAMkADNsvAAA%3D&exvsurl=1&path=/calendar/item",
            "eventStartTime": {
                "dateTime": "2017-06-09T18:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventEndTime": {
                "dateTime": "2017-06-09T19:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventLocation": {
                "displayName": "Conf Room 3"
            },
            "reminderFireTime": {
                "dateTime": "2017-06-09T17:45:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
