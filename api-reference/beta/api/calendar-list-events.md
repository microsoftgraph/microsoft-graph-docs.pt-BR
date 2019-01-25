---
title: Listar eventos
description: Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b92c9049867891f27fc7d75b3bfe4be8bd3fdb17
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519560"
---
# <a name="list-events"></a><span data-ttu-id="94717-104">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="94717-104">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94717-p102">Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.</span><span class="sxs-lookup"><span data-stu-id="94717-p102">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="94717-107">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar-list-calendarview.md) ou [obtenha as instâncias de um evento](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="94717-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94717-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="94717-108">Permissions</span></span>
<span data-ttu-id="94717-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94717-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94717-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94717-111">Permission type</span></span>      | <span data-ttu-id="94717-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94717-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94717-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94717-113">Delegated (work or school account)</span></span> | <span data-ttu-id="94717-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="94717-114">Calendars.Read</span></span>    |
|<span data-ttu-id="94717-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94717-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94717-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="94717-116">Calendars.Read</span></span>    |
|<span data-ttu-id="94717-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94717-117">Application</span></span> | <span data-ttu-id="94717-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="94717-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="94717-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94717-119">HTTP request</span></span>
<span data-ttu-id="94717-120"><!-- { "blockType": "ignored" } -->Um usuário ou do grupo padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="94717-120"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="94717-121">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="94717-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="94717-122">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="94717-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="94717-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="94717-123">Optional query parameters</span></span>
<span data-ttu-id="94717-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="94717-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="94717-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94717-125">Request headers</span></span>
| <span data-ttu-id="94717-126">Nome</span><span class="sxs-lookup"><span data-stu-id="94717-126">Name</span></span>       | <span data-ttu-id="94717-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="94717-127">Type</span></span> | <span data-ttu-id="94717-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="94717-128">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="94717-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="94717-129">Authorization</span></span>  | <span data-ttu-id="94717-130">string</span><span class="sxs-lookup"><span data-stu-id="94717-130">string</span></span> | <span data-ttu-id="94717-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94717-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="94717-133">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="94717-133">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="94717-134">string</span><span class="sxs-lookup"><span data-stu-id="94717-134">string</span></span> | <span data-ttu-id="94717-135">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="94717-135">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="94717-136">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="94717-136">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="94717-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="94717-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94717-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94717-138">Request body</span></span>
<span data-ttu-id="94717-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94717-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94717-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="94717-140">Response</span></span>

<span data-ttu-id="94717-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94717-141">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94717-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94717-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94717-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94717-143">Request</span></span>
<span data-ttu-id="94717-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94717-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="94717-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="94717-145">Response</span></span>
<span data-ttu-id="94717-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94717-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/calendar-list-events.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
