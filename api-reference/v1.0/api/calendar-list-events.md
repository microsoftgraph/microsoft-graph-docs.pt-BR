---
title: Listar eventos
description: Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 33bdadb28129183972f8fb6f7ee051708a3f2e55
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054599"
---
# <a name="list-events"></a><span data-ttu-id="48f75-104">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="48f75-104">List events</span></span>

<span data-ttu-id="48f75-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48f75-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48f75-106">Recupere uma lista de eventos em um calendário.</span><span class="sxs-lookup"><span data-stu-id="48f75-106">Retrieve a list of events in a calendar.</span></span>  <span data-ttu-id="48f75-107">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="48f75-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span> <span data-ttu-id="48f75-108">A lista de eventos contém reuniões de instância única e reuniões mestres em série.</span><span class="sxs-lookup"><span data-stu-id="48f75-108">The list of events contains single instance meetings and series masters.</span></span>

<span data-ttu-id="48f75-109">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar-list-calendarview.md) ou [obtenha as instâncias de um evento](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="48f75-109">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="48f75-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="48f75-110">Permissions</span></span>
<span data-ttu-id="48f75-111">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="48f75-111">Depending on the type of calendar that the events are in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="48f75-112">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48f75-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48f75-113">Calendário</span><span class="sxs-lookup"><span data-stu-id="48f75-113">Calendar</span></span> | <span data-ttu-id="48f75-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48f75-114">Delegated (work or school account)</span></span> | <span data-ttu-id="48f75-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48f75-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48f75-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48f75-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="48f75-117">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="48f75-117">user calendar</span></span> | <span data-ttu-id="48f75-118">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48f75-118">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="48f75-119">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48f75-119">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="48f75-120">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48f75-120">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="48f75-121">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="48f75-121">group calendar</span></span> | <span data-ttu-id="48f75-122">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f75-122">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="48f75-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48f75-123">Not supported.</span></span> | <span data-ttu-id="48f75-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48f75-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48f75-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48f75-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="48f75-126">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="48f75-126">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="48f75-127">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="48f75-127">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events
```
<span data-ttu-id="48f75-128">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="48f75-128">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="48f75-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="48f75-129">Optional query parameters</span></span>
<span data-ttu-id="48f75-130">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="48f75-130">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="48f75-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48f75-131">Request headers</span></span>
| <span data-ttu-id="48f75-132">Nome</span><span class="sxs-lookup"><span data-stu-id="48f75-132">Name</span></span>       | <span data-ttu-id="48f75-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="48f75-133">Type</span></span> | <span data-ttu-id="48f75-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="48f75-134">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="48f75-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="48f75-135">Authorization</span></span>  | <span data-ttu-id="48f75-136">string</span><span class="sxs-lookup"><span data-stu-id="48f75-136">string</span></span> | <span data-ttu-id="48f75-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48f75-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="48f75-139">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="48f75-139">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="48f75-140">string</span><span class="sxs-lookup"><span data-stu-id="48f75-140">string</span></span> | <span data-ttu-id="48f75-p105">Use isso para especificar o fuso horário para os horários de início e término na resposta. Se não for especificado, esses valores de tempo serão retornados em UTC. Opcional.</span><span class="sxs-lookup"><span data-stu-id="48f75-p105">Use this to specify the time zone for start and end times in the response. If not specified, those time values are returned in UTC. Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48f75-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48f75-144">Request body</span></span>
<span data-ttu-id="48f75-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48f75-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48f75-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="48f75-146">Response</span></span>

<span data-ttu-id="48f75-147">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48f75-147">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="48f75-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48f75-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48f75-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48f75-149">Request</span></span>
<span data-ttu-id="48f75-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48f75-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="48f75-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="48f75-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_get_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
# <a name="c"></a>[<span data-ttu-id="48f75-152">C#</span><span class="sxs-lookup"><span data-stu-id="48f75-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48f75-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48f75-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48f75-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48f75-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48f75-155">Java</span><span class="sxs-lookup"><span data-stu-id="48f75-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="48f75-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="48f75-156">Response</span></span>
<span data-ttu-id="48f75-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48f75-157">Here is an example of the response.</span></span> <span data-ttu-id="48f75-158">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="48f75-158">Note: The response object shown here might be shortened for readability.</span></span>
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
