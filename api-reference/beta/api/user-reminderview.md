---
title: 'user: reminderView'
description: 'Retorne uma lista de lembretes de calendário nas horas de início e término especificadas. '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4b349e499c975032fe0ea54910d05ca64ee19f4b
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107392"
---
# <a name="user-reminderview"></a><span data-ttu-id="19f59-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="19f59-103">user: reminderView</span></span>

<span data-ttu-id="19f59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19f59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19f59-105">Retornar uma lista de lembretes de eventos em um calendário de usuário dentro dos horários de início e término especificados.</span><span class="sxs-lookup"><span data-stu-id="19f59-105">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="19f59-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="19f59-106">Permissions</span></span>
<span data-ttu-id="19f59-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19f59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19f59-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19f59-109">Permission type</span></span>      | <span data-ttu-id="19f59-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19f59-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19f59-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19f59-111">Delegated (work or school account)</span></span> | <span data-ttu-id="19f59-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19f59-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="19f59-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19f59-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19f59-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19f59-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="19f59-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19f59-115">Application</span></span> | <span data-ttu-id="19f59-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19f59-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="19f59-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19f59-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="19f59-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="19f59-118">Function parameters</span></span>
<span data-ttu-id="19f59-119">Forneça os seguintes parâmetros de função com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="19f59-119">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="19f59-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="19f59-120">Parameter</span></span>    | <span data-ttu-id="19f59-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="19f59-121">Type</span></span>   |<span data-ttu-id="19f59-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="19f59-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19f59-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="19f59-123">startDateTime</span></span>|<span data-ttu-id="19f59-124">String</span><span class="sxs-lookup"><span data-stu-id="19f59-124">String</span></span>|<span data-ttu-id="19f59-p102">A data e hora de início do evento para o qual o lembrete está definido. O valor é representado no formato ISO 8601, por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="19f59-p102">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="19f59-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="19f59-127">endDateTime</span></span>|<span data-ttu-id="19f59-128">String</span><span class="sxs-lookup"><span data-stu-id="19f59-128">String</span></span>|<span data-ttu-id="19f59-p103">A data e hora de término do evento para o qual o lembrete está definido. O valor é representado no formato ISO 8601, por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="19f59-p103">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="19f59-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19f59-131">Request headers</span></span>
| <span data-ttu-id="19f59-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19f59-132">Header</span></span>       | <span data-ttu-id="19f59-133">Valor</span><span class="sxs-lookup"><span data-stu-id="19f59-133">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="19f59-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="19f59-134">Authorization</span></span>  | <span data-ttu-id="19f59-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19f59-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="19f59-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19f59-137">Content-Type</span></span>   | <span data-ttu-id="19f59-138">application/json</span><span class="sxs-lookup"><span data-stu-id="19f59-138">application/json</span></span> |
| <span data-ttu-id="19f59-139">Preferir</span><span class="sxs-lookup"><span data-stu-id="19f59-139">Prefer</span></span> | <span data-ttu-id="19f59-p105">{Time-zone}. Opcional, supõe-se o UTC se estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="19f59-p105">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19f59-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19f59-142">Request body</span></span>
<span data-ttu-id="19f59-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19f59-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19f59-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="19f59-144">Response</span></span>

<span data-ttu-id="19f59-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [reminder](../resources/reminder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19f59-145">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19f59-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19f59-146">Example</span></span>
<span data-ttu-id="19f59-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="19f59-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="19f59-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19f59-148">Request</span></span>
<span data-ttu-id="19f59-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19f59-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="19f59-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="19f59-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```
# <a name="c"></a>[<span data-ttu-id="19f59-151">C#</span><span class="sxs-lookup"><span data-stu-id="19f59-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-reminderview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19f59-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19f59-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-reminderview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19f59-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19f59-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-reminderview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="19f59-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="19f59-154">Response</span></span>
<span data-ttu-id="19f59-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19f59-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.reminder)",
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
<!--
{
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
