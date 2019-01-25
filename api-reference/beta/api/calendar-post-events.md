---
title: Criar evento
description: Use essa API para criar um novo evento no calendário especificado ou no padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7cd5c6ddf9834163bdd3b03dd2ab2aa36cd3b48b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516326"
---
# <a name="create-event"></a><span data-ttu-id="86d36-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="86d36-103">Create Event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86d36-104">Use essa API para criar um novo evento no calendário especificado ou no padrão.</span><span class="sxs-lookup"><span data-stu-id="86d36-104">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="86d36-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="86d36-105">Permissions</span></span>
<span data-ttu-id="86d36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86d36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86d36-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86d36-108">Permission type</span></span>      | <span data-ttu-id="86d36-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86d36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86d36-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86d36-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86d36-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86d36-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="86d36-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86d36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86d36-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86d36-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="86d36-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86d36-114">Application</span></span> | <span data-ttu-id="86d36-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86d36-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="86d36-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86d36-116">HTTP request</span></span>
<span data-ttu-id="86d36-117"><!-- { "blockType": "ignored" } -->Um usuário ou do grupo padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="86d36-117"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="86d36-118">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="86d36-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="86d36-119">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="86d36-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="86d36-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86d36-120">Request headers</span></span>
| <span data-ttu-id="86d36-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86d36-121">Header</span></span>       | <span data-ttu-id="86d36-122">Valor</span><span class="sxs-lookup"><span data-stu-id="86d36-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86d36-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="86d36-123">Authorization</span></span>  | <span data-ttu-id="86d36-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86d36-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="86d36-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86d36-126">Content-Type</span></span>  | <span data-ttu-id="86d36-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86d36-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86d36-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86d36-129">Request body</span></span>
<span data-ttu-id="86d36-130">No corpo da solicitação, forneça uma representação JSON do objeto [Event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="86d36-130">In the request body, supply a JSON representation of [Event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="86d36-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="86d36-131">Response</span></span>

<span data-ttu-id="86d36-132">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86d36-132">If successful, this method returns `201 Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86d36-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86d36-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86d36-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86d36-134">Request</span></span>
<span data-ttu-id="86d36-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86d36-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="86d36-136">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="86d36-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="86d36-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="86d36-137">Response</span></span>
<span data-ttu-id="86d36-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86d36-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-post-events.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
