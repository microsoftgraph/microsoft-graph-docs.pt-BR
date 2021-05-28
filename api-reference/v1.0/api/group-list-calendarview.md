---
title: Listar calendarView
description: Obter as ocorrências, exceções e instâncias únicas de eventos em uma exibição de calendário definida por um intervalo de tempo, a partir do calendário padrão do usuário,
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 42c1ed3d4409d0a209e44b8cb16a7f32928a4cee
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682585"
---
# <a name="list-calendarview"></a><span data-ttu-id="be67f-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="be67f-103">List calendarView</span></span>

<span data-ttu-id="be67f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be67f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="be67f-105">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão de um grupo.</span><span class="sxs-lookup"><span data-stu-id="be67f-105">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="be67f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="be67f-106">Permissions</span></span>
<span data-ttu-id="be67f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be67f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be67f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be67f-109">Permission type</span></span>      | <span data-ttu-id="be67f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be67f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be67f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be67f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="be67f-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be67f-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="be67f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be67f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be67f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be67f-114">Not supported.</span></span>    |
|<span data-ttu-id="be67f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be67f-115">Application</span></span> | <span data-ttu-id="be67f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be67f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be67f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be67f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="be67f-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="be67f-118">Query parameters</span></span>
<span data-ttu-id="be67f-119">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="be67f-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="be67f-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="be67f-120">Parameter</span></span>     | <span data-ttu-id="be67f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="be67f-121">Type</span></span>   | <span data-ttu-id="be67f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="be67f-122">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="be67f-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="be67f-123">startDateTime</span></span> | <span data-ttu-id="be67f-124">String</span><span class="sxs-lookup"><span data-stu-id="be67f-124">String</span></span> | <span data-ttu-id="be67f-p102">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="be67f-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="be67f-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="be67f-127">endDateTime</span></span>   | <span data-ttu-id="be67f-128">String</span><span class="sxs-lookup"><span data-stu-id="be67f-128">String</span></span> | <span data-ttu-id="be67f-p103">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="be67f-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="be67f-131">Os valores de `startDateTime` e `endDateTime` são interpretados usando o deslocamento de fuso horário especificado no valor e não são afetados pelo valor do cabeçalho `Prefer: outlook.timezone`, se presente.</span><span class="sxs-lookup"><span data-stu-id="be67f-131">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="be67f-132">Se nenhum deslocamento de fuso horário estiver incluído no valor, ele será interpretado como UTC.</span><span class="sxs-lookup"><span data-stu-id="be67f-132">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="be67f-133">Este método também dá suporte a alguns [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="be67f-133">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="be67f-134">As propriedades **createdDateTime** e **lastModifiedDateTime** do [evento](../resources/event.md) não são compatíveis com `$select`.</span><span class="sxs-lookup"><span data-stu-id="be67f-134">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="be67f-135">Para obter os valores, basta consultar no **calendarView** sem aplicar `$select`.</span><span class="sxs-lookup"><span data-stu-id="be67f-135">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be67f-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be67f-136">Request headers</span></span>
| <span data-ttu-id="be67f-137">Nome</span><span class="sxs-lookup"><span data-stu-id="be67f-137">Name</span></span>       | <span data-ttu-id="be67f-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="be67f-138">Type</span></span> | <span data-ttu-id="be67f-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="be67f-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="be67f-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="be67f-140">Authorization</span></span>  | <span data-ttu-id="be67f-141">string</span><span class="sxs-lookup"><span data-stu-id="be67f-141">string</span></span> | <span data-ttu-id="be67f-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be67f-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="be67f-144">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="be67f-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="be67f-145">string</span><span class="sxs-lookup"><span data-stu-id="be67f-145">string</span></span> | <span data-ttu-id="be67f-p107">Use isso para especificar o fuso horário para os horários de início e término na resposta. Se não for especificado, esses valores de tempo serão retornados em UTC. Opcional.</span><span class="sxs-lookup"><span data-stu-id="be67f-p107">Use this to specify the time zone for start and end times in the response. If not specified, those time values are returned in UTC. Optional.</span></span> |
| <span data-ttu-id="be67f-149">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="be67f-149">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="be67f-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be67f-150">string</span></span> | <span data-ttu-id="be67f-151">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="be67f-151">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="be67f-152">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="be67f-152">Values can be "text" or "html".</span></span> <span data-ttu-id="be67f-153">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="be67f-153">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="be67f-154">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="be67f-154">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="be67f-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="be67f-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be67f-156">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be67f-156">Request body</span></span>
<span data-ttu-id="be67f-157">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be67f-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be67f-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="be67f-158">Response</span></span>
<span data-ttu-id="be67f-159">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be67f-159">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be67f-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be67f-160">Example</span></span>
#### <a name="request"></a><span data-ttu-id="be67f-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be67f-161">Request</span></span>
<span data-ttu-id="be67f-162">O exemplo a seguir solicita que corpos de evento sejam retornados no formato de texto.</span><span class="sxs-lookup"><span data-stu-id="be67f-162">The following example requests event bodies to be returned in text format.</span></span>

# <a name="http"></a>[<span data-ttu-id="be67f-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="be67f-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "group_get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-10-01T19:00:00.00-08:00
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="be67f-164">C#</span><span class="sxs-lookup"><span data-stu-id="be67f-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be67f-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be67f-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be67f-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be67f-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be67f-167">Java</span><span class="sxs-lookup"><span data-stu-id="be67f-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="be67f-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="be67f-168">Response</span></span>
<span data-ttu-id="be67f-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be67f-169">The following is an example of the response.</span></span>
><span data-ttu-id="be67f-170">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="be67f-170">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1354
Preference-Applied: outlook.body-content-type="text"

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('02bd9fd6-8f93-4758-87c3-1fb73740a315')/calendarView",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19%3a00%3a00.0000000&endDateTime=2017-10-01T19%3a00%3a00.00&$skip=10",
    "value":[
        {
            "@odata.etag":"W/\"xPZF2y46pEiVBni87OnrpgAAFq78Xw==\"",
            "id":"AAMkAGI5MWYJOwAAEA==",
            "createdDateTime":"2017-07-31T18:59:01.982289Z",
            "lastModifiedDateTime":"2017-09-06T04:29:38.6647687Z",
            "changeKey":"xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
            "categories":[

            ],
            "originalStartTimeZone":"Eastern Standard Time",
            "originalEndTimeZone":"Eastern Standard Time",
            "iCalUId":"040000008200E00074C5B7101A82E00807E1080E824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
            "reminderMinutesBeforeStart":15,
            "isReminderOn":true,
            "hasAttachments":false,
            "subject":"New Training Plans",
            "bodyPreview":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
            "importance":"normal",
            "sensitivity":"normal",
            "isAllDay":false,
            "isCancelled":false,
            "isOrganizer":true,
            "responseRequested":true,
            "seriesMasterId":null,
            "showAs":"busy",
            "type":"singleInstance",
            "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI5MWYJOwAAEA%3D%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl":null,
            "responseStatus":{
                "response":"organizer",
                "time":"0001-01-01T00:00:00Z"
            },
            "body":{
                "contentType":"text",
                "content":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>\r\n"
            },
            "start":{
                "dateTime":"2017-08-14T21:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2017-08-14T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"HR Taskforce / Facilities"
            },
            "recurrence":null,
            "attendees":[
                 {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"HR Taskforce",
                        "address":"HRTaskforce@contoso.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Megan Bowen",
                        "address":"MeganB@contoso.onmicrosoft.com"
                    }
                }
             ],
            "organizer":{
                "emailAddress":{
                    "name":"HR Taskforce",
                    "address":"HRTaskforce@contoso.onmicrosoft.com"
                }
            }
        },
        {
            "@odata.etag":"W/\"xPZF2y46pEiVBni87OnrpgAAFq78Xw==\"",
            "id":"AAMkAGI5MWYJOwAAEA==",
            "createdDateTime":"2017-07-31T18:59:01.982289Z",
            "lastModifiedDateTime":"2017-09-06T04:29:38.6647687Z",
            "changeKey":"xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
            "categories":[

            ],
            "originalStartTimeZone":"Eastern Standard Time",
            "originalEndTimeZone":"Eastern Standard Time",
            "iCalUId":"040000008200E00074C5B7101A82E00807E10810824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
            "reminderMinutesBeforeStart":15,
            "isReminderOn":true,
            "hasAttachments":false,
            "subject":"New Training Plans",
            "bodyPreview":"Follow-up meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
            "importance":"normal",
            "sensitivity":"normal",
            "isAllDay":false,
            "isCancelled":false,
            "isOrganizer":true,
            "responseRequested":true,
            "seriesMasterId":null,
            "showAs":"busy",
            "type":"singleInstance",
            "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI5MWYJOwAAEA%3D%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl":null,
            "responseStatus":{
                "response":"organizer",
                "time":"0001-01-01T00:00:00Z"
            },
            "body":{
                "contentType":"text",
                "content":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>\r\n"
            },
            "start":{
                "dateTime":"2017-08-16T21:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2017-08-16T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"HR Taskforce / Facilities"
            },
            "recurrence":null,
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"HR Taskforce",
                        "address":"HRTaskforce@contoso.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Megan Bowen",
                        "address":"MeganB@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer":{
                "emailAddress":{
                    "name":"HR Taskforce",
                    "address":"HRTaskforce@contoso.onmicrosoft.com"
                }
            }
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
