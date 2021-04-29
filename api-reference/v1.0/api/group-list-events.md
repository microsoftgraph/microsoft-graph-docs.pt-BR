---
title: Listar eventos
description: Recuperar uma lista de objetos event.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 92689c47b456d85e605cdd509045f77b94ea12b0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052324"
---
# <a name="list-events"></a><span data-ttu-id="0f89f-103">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="0f89f-103">List events</span></span>

<span data-ttu-id="0f89f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f89f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f89f-105">Recupere uma lista de objetos [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="0f89f-105">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f89f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f89f-106">Permissions</span></span>
<span data-ttu-id="0f89f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f89f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f89f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f89f-109">Permission type</span></span>      | <span data-ttu-id="0f89f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f89f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f89f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f89f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0f89f-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f89f-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f89f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f89f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f89f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f89f-114">Not supported.</span></span>    |
|<span data-ttu-id="0f89f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f89f-115">Application</span></span> | <span data-ttu-id="0f89f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f89f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f89f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f89f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f89f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0f89f-118">Optional query parameters</span></span>
<span data-ttu-id="0f89f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0f89f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f89f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f89f-120">Request headers</span></span>
| <span data-ttu-id="0f89f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0f89f-121">Name</span></span>       | <span data-ttu-id="0f89f-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f89f-122">Type</span></span> | <span data-ttu-id="0f89f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f89f-123">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="0f89f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f89f-124">Authorization</span></span>  | <span data-ttu-id="0f89f-125">string</span><span class="sxs-lookup"><span data-stu-id="0f89f-125">string</span></span> | <span data-ttu-id="0f89f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f89f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0f89f-128">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="0f89f-128">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="0f89f-129">string</span><span class="sxs-lookup"><span data-stu-id="0f89f-129">string</span></span> | <span data-ttu-id="0f89f-p103">Use isso para especificar o fuso horário para os horários de início e término na resposta. Se não for especificado, esses valores de tempo serão retornados em UTC. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0f89f-p103">Use this to specify the time zone for start and end times in the response. If not specified, those time values are returned in UTC. Optional.</span></span> |
| <span data-ttu-id="0f89f-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="0f89f-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="0f89f-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f89f-134">string</span></span> | <span data-ttu-id="0f89f-135">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="0f89f-135">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="0f89f-136">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="0f89f-136">Values can be "text" or "html".</span></span> <span data-ttu-id="0f89f-137">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="0f89f-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="0f89f-138">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="0f89f-138">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="0f89f-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0f89f-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f89f-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f89f-140">Request body</span></span>
<span data-ttu-id="0f89f-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0f89f-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f89f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f89f-142">Response</span></span>
<span data-ttu-id="0f89f-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f89f-143">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f89f-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f89f-144">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0f89f-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f89f-145">Request</span></span>
<span data-ttu-id="0f89f-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f89f-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0f89f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f89f-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "get_group_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events
```
# <a name="c"></a>[<span data-ttu-id="0f89f-148">C#</span><span class="sxs-lookup"><span data-stu-id="0f89f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f89f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f89f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f89f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f89f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f89f-151">Java</span><span class="sxs-lookup"><span data-stu-id="0f89f-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0f89f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f89f-152">Response</span></span>
<span data-ttu-id="0f89f-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f89f-153">The following is an example of the response.</span></span>
><span data-ttu-id="0f89f-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0f89f-154">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA==",
      "createdDateTime": "2017-07-31T18:59:01.982289Z",
      "lastModifiedDateTime": "2017-09-06T04:29:38.6647687Z",
      "changeKey": "xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
      "categories": [],
      "originalStartTimeZone": "Eastern Standard Time",
      "originalEndTimeZone": "Eastern Standard Time",
      "iCalUId": "040000008200E00074C5B7101A82E00800000000824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "New Training Plans",
      "bodyPreview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "seriesMaster",
      "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA%3D%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "responseStatus": {
          "response": "organizer",
          "time": "0001-01-01T00:00:00Z"
      },
      "body": {
          "contentType": "html",
          "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Meeting to plan new trainings.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
      },
      "start": {
          "dateTime": "2017-08-14T21:00:00.0000000",
          "timeZone": "UTC"
      },
      "end": {
          "dateTime": "2017-08-14T22:00:00.0000000",
          "timeZone": "UTC"
      },
      "location": {
          "displayName": "HR Taskforce / Facilities"
      },
      "recurrence": {
          "pattern": {
              "type": "weekly",
              "interval": 1,
              "month": 0,
              "dayOfMonth": 0,
              "daysOfWeek": [
                  "monday",
                  "wednesday",
                  "friday"
              ],
              "firstDayOfWeek": "sunday",
              "index": "first"
          },
          "range": {
              "type": "noEnd",
              "startDate": "2017-08-14",
              "endDate": "0001-01-01",
              "recurrenceTimeZone": "Eastern Standard Time",
              "numberOfOccurrences": 0
          }
      },
      "attendees": [
          {
              "type": "required",
              "status": {
                  "response": "accepted",
                  "time": "2017-07-31T18:59:06.4180028Z"
              },
              "emailAddress": {
                  "name": "Joni Sherman",
                  "address": "JoniS@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "HR Taskforce",
                  "address": "HRTaskforce@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Megan Bowen",
                  "address": "MeganB@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Lidia Holloway",
                  "address": "LidiaH@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Emily Braun",
                  "address": "EmilyB@contoso.onmicrosoft.com"
              }
          }
      ],
      "organizer": {
          "emailAddress": {
              "name": "HR Taskforce",
              "address": "HRTaskforce@contoso.onmicrosoft.com"
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

