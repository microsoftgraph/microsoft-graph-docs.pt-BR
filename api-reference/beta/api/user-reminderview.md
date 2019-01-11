---
title: 'user: reminderView'
description: 'Retorne uma lista de lembretes de calendário nas horas de início e término especificadas. '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 4edcc4a6a46cbdee1233ad7496fa231bba8bfd27
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886076"
---
# <a name="user-reminderview"></a><span data-ttu-id="e869b-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="e869b-103">user: reminderView</span></span>

> <span data-ttu-id="e869b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e869b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e869b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e869b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e869b-106">Retorne uma lista de lembretes de evento em um calendário do usuário dentro do especificados de início e término.</span><span class="sxs-lookup"><span data-stu-id="e869b-106">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e869b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e869b-107">Permissions</span></span>
<span data-ttu-id="e869b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e869b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e869b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e869b-110">Permission type</span></span>      | <span data-ttu-id="e869b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e869b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e869b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e869b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e869b-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e869b-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e869b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e869b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e869b-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e869b-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e869b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e869b-116">Application</span></span> | <span data-ttu-id="e869b-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e869b-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e869b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e869b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="e869b-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e869b-119">Function parameters</span></span>
<span data-ttu-id="e869b-120">Forneça os seguintes parâmetros de função com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="e869b-120">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="e869b-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e869b-121">Parameter</span></span>    | <span data-ttu-id="e869b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e869b-122">Type</span></span>   |<span data-ttu-id="e869b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e869b-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e869b-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e869b-124">startDateTime</span></span>|<span data-ttu-id="e869b-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e869b-125">String</span></span>|<span data-ttu-id="e869b-p103">A data e hora de início do evento para o qual o lembrete está definido. O valor é representado no formato ISO 8601, por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="e869b-p103">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="e869b-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e869b-128">endDateTime</span></span>|<span data-ttu-id="e869b-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e869b-129">String</span></span>|<span data-ttu-id="e869b-p104">A data e hora de término do evento para o qual o lembrete está definido. O valor é representado no formato ISO 8601, por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="e869b-p104">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e869b-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e869b-132">Request headers</span></span>
| <span data-ttu-id="e869b-133">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e869b-133">Header</span></span>       | <span data-ttu-id="e869b-134">Valor</span><span class="sxs-lookup"><span data-stu-id="e869b-134">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e869b-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="e869b-135">Authorization</span></span>  | <span data-ttu-id="e869b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e869b-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e869b-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e869b-138">Content-Type</span></span>   | <span data-ttu-id="e869b-139">application/json</span><span class="sxs-lookup"><span data-stu-id="e869b-139">application/json</span></span> |
| <span data-ttu-id="e869b-140">Preferir</span><span class="sxs-lookup"><span data-stu-id="e869b-140">Prefer</span></span> | <span data-ttu-id="e869b-p106">{Time-zone}. Opcional, supõe-se o UTC se estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="e869b-p106">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e869b-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e869b-143">Request body</span></span>
<span data-ttu-id="e869b-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e869b-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e869b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e869b-145">Response</span></span>

<span data-ttu-id="e869b-146">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [reminder](../resources/reminder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e869b-146">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e869b-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e869b-147">Example</span></span>
<span data-ttu-id="e869b-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e869b-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e869b-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e869b-149">Request</span></span>
<span data-ttu-id="e869b-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e869b-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/beta/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```

##### <a name="response"></a><span data-ttu-id="e869b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e869b-151">Response</span></span>
<span data-ttu-id="e869b-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e869b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
