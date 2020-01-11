---
title: Listar calendarView
description: Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão de um grupo.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: bc13de3a3c94f821ebe38f04845dcfb00e0ccb8b
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023051"
---
# <a name="list-calendarview"></a><span data-ttu-id="bcf07-103">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="bcf07-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcf07-104">Obtenha as ocorrências, exceções e instâncias individuais de eventos em uma exibição de calendário definida, do calendário padrão de um grupo.</span><span class="sxs-lookup"><span data-stu-id="bcf07-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcf07-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bcf07-105">Permissions</span></span>
<span data-ttu-id="bcf07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcf07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcf07-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcf07-108">Permission type</span></span>      | <span data-ttu-id="bcf07-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bcf07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcf07-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcf07-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bcf07-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcf07-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bcf07-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcf07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcf07-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcf07-113">Not supported.</span></span>    |
|<span data-ttu-id="bcf07-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcf07-114">Application</span></span> | <span data-ttu-id="bcf07-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcf07-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcf07-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcf07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="bcf07-117">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="bcf07-117">Query parameters</span></span>
<span data-ttu-id="bcf07-118">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="bcf07-118">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="bcf07-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bcf07-119">Parameter</span></span>     | <span data-ttu-id="bcf07-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcf07-120">Type</span></span>   | <span data-ttu-id="bcf07-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcf07-121">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="bcf07-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bcf07-122">startDateTime</span></span> | <span data-ttu-id="bcf07-123">String</span><span class="sxs-lookup"><span data-stu-id="bcf07-123">String</span></span> | <span data-ttu-id="bcf07-124">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="bcf07-124">The start date and time of the time range, represented in ISO 8601 format.</span></span> <span data-ttu-id="bcf07-125">Por exemplo, "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="bcf07-125">For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="bcf07-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bcf07-126">endDateTime</span></span>   | <span data-ttu-id="bcf07-127">String</span><span class="sxs-lookup"><span data-stu-id="bcf07-127">String</span></span> | <span data-ttu-id="bcf07-128">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="bcf07-128">The end date and time of the time range, represented in ISO 8601 format.</span></span> <span data-ttu-id="bcf07-129">Por exemplo, "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="bcf07-129">For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="bcf07-130">Os valores de `startDateTime` e `endDateTime` são interpretados usando o deslocamento de fuso horário especificado no valor e não são afetados pelo valor do `Prefer: outlook.timezone` cabeçalho, se houver.</span><span class="sxs-lookup"><span data-stu-id="bcf07-130">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="bcf07-131">Se nenhum deslocamento de fuso horário for incluído no valor, será interpretado como UTC.</span><span class="sxs-lookup"><span data-stu-id="bcf07-131">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="bcf07-132">Este método também dá suporte a alguns [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bcf07-132">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="bcf07-133">As propriedades **createdDateTime** e **lastModifiedDateTime** do [evento](../resources/event.md) não são compatíveis com `$select`.</span><span class="sxs-lookup"><span data-stu-id="bcf07-133">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="bcf07-134">Para obter os valores, basta consultar no **calendarView** sem aplicar `$select`.</span><span class="sxs-lookup"><span data-stu-id="bcf07-134">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcf07-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcf07-135">Request headers</span></span>
| <span data-ttu-id="bcf07-136">Nome</span><span class="sxs-lookup"><span data-stu-id="bcf07-136">Name</span></span>       | <span data-ttu-id="bcf07-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcf07-137">Type</span></span> | <span data-ttu-id="bcf07-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcf07-138">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="bcf07-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcf07-139">Authorization</span></span>  | <span data-ttu-id="bcf07-140">string</span><span class="sxs-lookup"><span data-stu-id="bcf07-140">string</span></span> | <span data-ttu-id="bcf07-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcf07-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bcf07-143">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="bcf07-143">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="bcf07-144">string</span><span class="sxs-lookup"><span data-stu-id="bcf07-144">string</span></span> | <span data-ttu-id="bcf07-145">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="bcf07-145">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="bcf07-146">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="bcf07-146">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="bcf07-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bcf07-147">Optional.</span></span> |
| <span data-ttu-id="bcf07-148">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="bcf07-148">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="bcf07-149">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bcf07-149">string</span></span> | <span data-ttu-id="bcf07-150">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="bcf07-150">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="bcf07-151">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="bcf07-151">Values can be "text" or "html".</span></span> <span data-ttu-id="bcf07-152">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="bcf07-152">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="bcf07-153">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="bcf07-153">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="bcf07-154">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bcf07-154">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcf07-155">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcf07-155">Request body</span></span>
<span data-ttu-id="bcf07-156">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bcf07-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcf07-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcf07-157">Response</span></span>
<span data-ttu-id="bcf07-158">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcf07-158">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcf07-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcf07-159">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bcf07-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcf07-160">Request</span></span>
<span data-ttu-id="bcf07-161">O exemplo a seguir solicita que corpos de evento sejam retornados no formato de texto.</span><span class="sxs-lookup"><span data-stu-id="bcf07-161">The following example requests event bodies to be returned in text format.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bcf07-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcf07-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_calendarviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-10-01T19:00:00.00-08:00
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bcf07-163">C#</span><span class="sxs-lookup"><span data-stu-id="bcf07-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-calendarviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcf07-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcf07-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-calendarviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bcf07-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcf07-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-calendarviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bcf07-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcf07-166">Response</span></span>
<span data-ttu-id="bcf07-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bcf07-167">The following is an example of the response.</span></span>
><span data-ttu-id="bcf07-168">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bcf07-168">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bcf07-169">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bcf07-169">All the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('02bd9fd6-8f93-4758-87c3-1fb73740a315')/calendarView",
    "@odata.nextLink":"https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19%3a00%3a00.0000000&endDateTime=2017-10-01T19%3a00%3a00.00&$skip=10",
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
            "uid":"040000008200E00074C5B7101A82E00807E1080E824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
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
            "uid":"040000008200E00074C5B7101A82E00807E10810824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
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
<!--
{
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
