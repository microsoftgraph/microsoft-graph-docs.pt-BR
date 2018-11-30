---
title: Listar eventos
description: Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.
ms.openlocfilehash: 4052f75abf4340d4acddbb79c1d318c7d1ca0f29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034090"
---
# <a name="list-events"></a><span data-ttu-id="e8830-104">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="e8830-104">List events</span></span>

> <span data-ttu-id="e8830-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e8830-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8830-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e8830-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8830-p103">Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.</span><span class="sxs-lookup"><span data-stu-id="e8830-p103">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="e8830-109">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar-list-calendarview.md) ou [obtenha as instâncias de um evento](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="e8830-109">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8830-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8830-110">Permissions</span></span>
<span data-ttu-id="e8830-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8830-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8830-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8830-113">Permission type</span></span>      | <span data-ttu-id="e8830-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8830-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8830-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8830-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e8830-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e8830-116">Calendars.Read</span></span>    |
|<span data-ttu-id="e8830-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8830-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8830-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e8830-118">Calendars.Read</span></span>    |
|<span data-ttu-id="e8830-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8830-119">Application</span></span> | <span data-ttu-id="e8830-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e8830-120">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8830-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8830-121">HTTP request</span></span>
<span data-ttu-id="e8830-122"><!-- { "blockType": "ignored" } -->Um usuário ou do grupo padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="e8830-122"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="e8830-123">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="e8830-123">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="e8830-124">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="e8830-124">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8830-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8830-125">Optional query parameters</span></span>
<span data-ttu-id="e8830-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8830-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e8830-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8830-127">Request headers</span></span>
| <span data-ttu-id="e8830-128">Nome</span><span class="sxs-lookup"><span data-stu-id="e8830-128">Name</span></span>       | <span data-ttu-id="e8830-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8830-129">Type</span></span> | <span data-ttu-id="e8830-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8830-130">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="e8830-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8830-131">Authorization</span></span>  | <span data-ttu-id="e8830-132">string</span><span class="sxs-lookup"><span data-stu-id="e8830-132">string</span></span> | <span data-ttu-id="e8830-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8830-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e8830-135">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e8830-135">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="e8830-136">string</span><span class="sxs-lookup"><span data-stu-id="e8830-136">string</span></span> | <span data-ttu-id="e8830-137">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="e8830-137">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="e8830-138">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="e8830-138">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="e8830-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e8830-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8830-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8830-140">Request body</span></span>
<span data-ttu-id="e8830-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8830-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8830-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8830-142">Response</span></span>

<span data-ttu-id="e8830-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8830-143">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8830-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8830-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8830-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8830-145">Request</span></span>
<span data-ttu-id="e8830-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8830-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="e8830-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8830-147">Response</span></span>
<span data-ttu-id="e8830-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8830-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
