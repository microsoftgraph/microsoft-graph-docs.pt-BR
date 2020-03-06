---
title: Listar eventos
description: Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0b21a267c79fbde4c2a2f0099446206e9c5d2bd4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518795"
---
# <a name="list-events"></a><span data-ttu-id="d9249-104">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="d9249-104">List events</span></span>

<span data-ttu-id="d9249-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9249-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9249-106">Recupere uma lista de eventos em um calendário.</span><span class="sxs-lookup"><span data-stu-id="d9249-106">Retrieve a list of events in a calendar.</span></span>  <span data-ttu-id="d9249-107">O calendário pode ser para um [usuário](../resources/user.md) ou um calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="d9249-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> <span data-ttu-id="d9249-108">A lista de eventos contém reuniões de instância única e reuniões mestres em série.</span><span class="sxs-lookup"><span data-stu-id="d9249-108">The list of events contains single instance meetings and series masters.</span></span>

<span data-ttu-id="d9249-109">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar-list-calendarview.md) ou [obtenha as instâncias de um evento](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="d9249-109">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9249-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9249-110">Permissions</span></span>
<span data-ttu-id="d9249-111">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="d9249-111">Depending on the type of calendar that the events are in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="d9249-112">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9249-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9249-113">Calendário</span><span class="sxs-lookup"><span data-stu-id="d9249-113">Calendar</span></span> | <span data-ttu-id="d9249-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9249-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d9249-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9249-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9249-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9249-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="d9249-117">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="d9249-117">user calendar</span></span> | <span data-ttu-id="d9249-118">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9249-118">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="d9249-119">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9249-119">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="d9249-120">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9249-120">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="d9249-121">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="d9249-121">group calendar</span></span> | <span data-ttu-id="d9249-122">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9249-122">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="d9249-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9249-123">Not supported.</span></span> | <span data-ttu-id="d9249-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9249-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9249-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9249-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d9249-126">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="d9249-126">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="d9249-127">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="d9249-127">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="d9249-128">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="d9249-128">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d9249-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9249-129">Optional query parameters</span></span>
<span data-ttu-id="d9249-130">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9249-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d9249-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9249-131">Request headers</span></span>
| <span data-ttu-id="d9249-132">Nome</span><span class="sxs-lookup"><span data-stu-id="d9249-132">Name</span></span>       | <span data-ttu-id="d9249-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9249-133">Type</span></span> | <span data-ttu-id="d9249-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9249-134">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="d9249-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9249-135">Authorization</span></span>  | <span data-ttu-id="d9249-136">string</span><span class="sxs-lookup"><span data-stu-id="d9249-136">string</span></span> | <span data-ttu-id="d9249-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9249-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d9249-139">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d9249-139">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="d9249-140">string</span><span class="sxs-lookup"><span data-stu-id="d9249-140">string</span></span> | <span data-ttu-id="d9249-141">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="d9249-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="d9249-142">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="d9249-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d9249-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d9249-143">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9249-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9249-144">Request body</span></span>
<span data-ttu-id="d9249-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9249-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9249-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9249-146">Response</span></span>

<span data-ttu-id="d9249-147">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9249-147">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d9249-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9249-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9249-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9249-149">Request</span></span>
<span data-ttu-id="d9249-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9249-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9249-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9249-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_get_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
# <a name="c"></a>[<span data-ttu-id="d9249-152">C#</span><span class="sxs-lookup"><span data-stu-id="d9249-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9249-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9249-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9249-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9249-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9249-155">Java</span><span class="sxs-lookup"><span data-stu-id="d9249-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d9249-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9249-156">Response</span></span>
<span data-ttu-id="d9249-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9249-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
