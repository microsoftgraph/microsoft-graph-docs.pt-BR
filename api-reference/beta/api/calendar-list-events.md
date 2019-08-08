---
title: Listar eventos
description: Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 20393a541505ddc5e1640cbcc6738efa3d32d05d
ms.sourcegitcommit: eb5f63deafcdd6db44e791f2d1f4c46604ab06fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245615"
---
# <a name="list-events"></a><span data-ttu-id="f5276-104">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="f5276-104">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5276-105">Recuperar uma lista de eventos em um calendário.</span><span class="sxs-lookup"><span data-stu-id="f5276-105">Retrieve a list of events in a calendar.</span></span>  <span data-ttu-id="f5276-106">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f5276-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> <span data-ttu-id="f5276-107">A lista de eventos contém reuniões de instância única e mestres de séries.</span><span class="sxs-lookup"><span data-stu-id="f5276-107">The list of events contains single instance meetings and series masters.</span></span>

<span data-ttu-id="f5276-108">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar-list-calendarview.md) ou [obtenha as instâncias de um evento](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="f5276-108">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5276-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5276-109">Permissions</span></span>
<span data-ttu-id="f5276-110">Dependendo do tipo de calendário em que os eventos estão e do tipo de permissão (delegado ou aplicativo) solicitado, uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f5276-110">Depending on the type of calendar that the events are in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="f5276-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5276-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5276-112">Calendário</span><span class="sxs-lookup"><span data-stu-id="f5276-112">Calendar</span></span> | <span data-ttu-id="f5276-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5276-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f5276-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5276-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5276-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5276-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="f5276-116">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="f5276-116">user calendar</span></span> | <span data-ttu-id="f5276-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5276-117">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="f5276-118">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5276-118">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="f5276-119">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5276-119">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="f5276-120">grupo calendar</span><span class="sxs-lookup"><span data-stu-id="f5276-120">group calendar</span></span> | <span data-ttu-id="f5276-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5276-121">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="f5276-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5276-122">Not supported.</span></span> | <span data-ttu-id="f5276-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5276-123">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="f5276-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5276-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f5276-125">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="f5276-125">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="f5276-126">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="f5276-126">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="f5276-127">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="f5276-127">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5276-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f5276-128">Optional query parameters</span></span>
<span data-ttu-id="f5276-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f5276-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f5276-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5276-130">Request headers</span></span>
| <span data-ttu-id="f5276-131">Nome</span><span class="sxs-lookup"><span data-stu-id="f5276-131">Name</span></span>       | <span data-ttu-id="f5276-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5276-132">Type</span></span> | <span data-ttu-id="f5276-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5276-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="f5276-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5276-134">Authorization</span></span>  | <span data-ttu-id="f5276-135">string</span><span class="sxs-lookup"><span data-stu-id="f5276-135">string</span></span> | <span data-ttu-id="f5276-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5276-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f5276-138">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f5276-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="f5276-139">string</span><span class="sxs-lookup"><span data-stu-id="f5276-139">string</span></span> | <span data-ttu-id="f5276-140">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="f5276-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="f5276-141">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="f5276-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="f5276-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f5276-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5276-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5276-143">Request body</span></span>
<span data-ttu-id="f5276-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5276-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5276-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5276-145">Response</span></span>

<span data-ttu-id="f5276-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5276-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5276-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5276-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5276-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5276-148">Request</span></span>
<span data-ttu-id="f5276-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5276-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f5276-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5276-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f5276-151">C#</span><span class="sxs-lookup"><span data-stu-id="f5276-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f5276-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="f5276-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f5276-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f5276-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f5276-154">Java</span><span class="sxs-lookup"><span data-stu-id="f5276-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f5276-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5276-155">Response</span></span>
<span data-ttu-id="f5276-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5276-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
