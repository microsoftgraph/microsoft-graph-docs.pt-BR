---
title: 'user: reminderView'
description: 'Retorne uma lista de lembretes de calendário nas horas de início e término especificadas. '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6ad00e61de2d87596527081016c3a0f77a18d3fb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975896"
---
# <a name="user-reminderview"></a><span data-ttu-id="519b1-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="519b1-103">user: reminderView</span></span>

<span data-ttu-id="519b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="519b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="519b1-105">Retornar uma lista de lembretes de eventos em um calendário de usuário dentro dos horários de início e término especificados.</span><span class="sxs-lookup"><span data-stu-id="519b1-105">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="519b1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="519b1-106">Permissions</span></span>
<span data-ttu-id="519b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="519b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="519b1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="519b1-109">Permission type</span></span>      | <span data-ttu-id="519b1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="519b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="519b1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="519b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="519b1-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="519b1-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="519b1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="519b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="519b1-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="519b1-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="519b1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="519b1-115">Application</span></span> | <span data-ttu-id="519b1-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="519b1-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="519b1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="519b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="519b1-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="519b1-118">Function parameters</span></span>
<span data-ttu-id="519b1-119">Forneça os seguintes parâmetros de função com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="519b1-119">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="519b1-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="519b1-120">Parameter</span></span>    | <span data-ttu-id="519b1-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="519b1-121">Type</span></span>   |<span data-ttu-id="519b1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="519b1-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="519b1-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="519b1-123">startDateTime</span></span>|<span data-ttu-id="519b1-124">String</span><span class="sxs-lookup"><span data-stu-id="519b1-124">String</span></span>|<span data-ttu-id="519b1-p102">A data e hora de início do evento para o qual o lembrete está definido. O valor é representado no formato ISO 8601, por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="519b1-p102">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="519b1-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="519b1-127">endDateTime</span></span>|<span data-ttu-id="519b1-128">String</span><span class="sxs-lookup"><span data-stu-id="519b1-128">String</span></span>|<span data-ttu-id="519b1-p103">A data e hora de término do evento para o qual o lembrete está definido. O valor é representado no formato ISO 8601, por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="519b1-p103">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="519b1-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="519b1-131">Request headers</span></span>
| <span data-ttu-id="519b1-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="519b1-132">Header</span></span>       | <span data-ttu-id="519b1-133">Valor</span><span class="sxs-lookup"><span data-stu-id="519b1-133">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="519b1-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="519b1-134">Authorization</span></span>  | <span data-ttu-id="519b1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="519b1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="519b1-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="519b1-137">Content-Type</span></span>   | <span data-ttu-id="519b1-138">application/json</span><span class="sxs-lookup"><span data-stu-id="519b1-138">application/json</span></span> |
| <span data-ttu-id="519b1-139">Preferir</span><span class="sxs-lookup"><span data-stu-id="519b1-139">Prefer</span></span> | <span data-ttu-id="519b1-p105">{Time-zone}. Opcional, supõe-se o UTC se estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="519b1-p105">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="519b1-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="519b1-142">Request body</span></span>
<span data-ttu-id="519b1-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="519b1-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="519b1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="519b1-144">Response</span></span>

<span data-ttu-id="519b1-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [reminder](../resources/reminder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="519b1-145">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="519b1-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="519b1-146">Example</span></span>
<span data-ttu-id="519b1-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="519b1-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="519b1-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="519b1-148">Request</span></span>
<span data-ttu-id="519b1-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="519b1-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="519b1-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="519b1-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```
# <a name="c"></a>[<span data-ttu-id="519b1-151">C#</span><span class="sxs-lookup"><span data-stu-id="519b1-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-reminderview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="519b1-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="519b1-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-reminderview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="519b1-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="519b1-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-reminderview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="519b1-154">Java</span><span class="sxs-lookup"><span data-stu-id="519b1-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-reminderview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="519b1-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="519b1-155">Response</span></span>
<span data-ttu-id="519b1-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="519b1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


