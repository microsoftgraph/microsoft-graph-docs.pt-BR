---
title: 'event: decline'
description: Recusar o convite para o evento específico em um calendário de usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 343322decb240d174030f76469c605fa562edc78
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42423368"
---
# <a name="event-decline"></a><span data-ttu-id="2f9d2-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="2f9d2-103">event: decline</span></span>

<span data-ttu-id="2f9d2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2f9d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f9d2-105">Recusar o convite para o [evento](../resources/event.md) especificado em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-105">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

<span data-ttu-id="2f9d2-106">Se o evento permitir propostas para novos horários, ao recusar o evento, um convidado poderá optar por sugerir um tempo alternativo, incluindo o parâmetro **proposedNewTime** .</span><span class="sxs-lookup"><span data-stu-id="2f9d2-106">If the event allows proposals for new times, on declining the event, an invitee can choose to suggest an alternative time by including the **proposedNewTime** parameter.</span></span> <span data-ttu-id="2f9d2-107">Para obter mais informações sobre como propor um horário e como receber e aceitar uma nova proposta de tempo, confira [propor novos horários da reunião](/graph/outlook-calendar-meeting-proposals).</span><span class="sxs-lookup"><span data-stu-id="2f9d2-107">For more information on how to propose a time, and how to receive and accept a new time proposal, see [Propose new meeting times](/graph/outlook-calendar-meeting-proposals).</span></span>


## <a name="permissions"></a><span data-ttu-id="2f9d2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f9d2-108">Permissions</span></span>
<span data-ttu-id="2f9d2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f9d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f9d2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f9d2-111">Permission type</span></span>      | <span data-ttu-id="2f9d2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f9d2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f9d2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f9d2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2f9d2-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f9d2-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2f9d2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f9d2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f9d2-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f9d2-116">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2f9d2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f9d2-117">Application</span></span> | <span data-ttu-id="2f9d2-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f9d2-118">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f9d2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f9d2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/decline
POST /users/{id | userPrincipalName}/events/{id}/decline

POST /me/calendar/events/{id}/decline
POST /users/{id | userPrincipalName}/calendar/events/{id}/decline

POST /me/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline

POST /me/calendargroup/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/decline

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="2f9d2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f9d2-120">Request headers</span></span>

| <span data-ttu-id="2f9d2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2f9d2-121">Name</span></span>       | <span data-ttu-id="2f9d2-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f9d2-122">Type</span></span> | <span data-ttu-id="2f9d2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f9d2-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f9d2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f9d2-124">Authorization</span></span>  | <span data-ttu-id="2f9d2-125">string</span><span class="sxs-lookup"><span data-stu-id="2f9d2-125">string</span></span>  | <span data-ttu-id="2f9d2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f9d2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f9d2-128">Content-Type</span></span> | <span data-ttu-id="2f9d2-129">string</span><span class="sxs-lookup"><span data-stu-id="2f9d2-129">string</span></span>  | <span data-ttu-id="2f9d2-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f9d2-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f9d2-132">Request body</span></span>

<span data-ttu-id="2f9d2-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f9d2-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2f9d2-134">Parameter</span></span>    | <span data-ttu-id="2f9d2-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f9d2-135">Type</span></span>   |<span data-ttu-id="2f9d2-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f9d2-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f9d2-137">comment</span><span class="sxs-lookup"><span data-stu-id="2f9d2-137">comment</span></span>|<span data-ttu-id="2f9d2-138">String</span><span class="sxs-lookup"><span data-stu-id="2f9d2-138">String</span></span>|<span data-ttu-id="2f9d2-p105">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="2f9d2-141">sendResponse</span><span class="sxs-lookup"><span data-stu-id="2f9d2-141">sendResponse</span></span>|<span data-ttu-id="2f9d2-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f9d2-142">Boolean</span></span>|<span data-ttu-id="2f9d2-p106">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|
|<span data-ttu-id="2f9d2-146">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="2f9d2-146">proposedNewTime</span></span>|[<span data-ttu-id="2f9d2-147">timeSlot</span><span class="sxs-lookup"><span data-stu-id="2f9d2-147">timeSlot</span></span>](../resources/timeslot.md)|<span data-ttu-id="2f9d2-148">Uma data/hora alternativa propostas por um convidado para uma solicitação de reunião para iniciar e finalizar.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-148">An alternate date/time proposed by an invitee for a meeting request to start and end.</span></span> <span data-ttu-id="2f9d2-149">Válido somente para eventos que permitem novas propostas de horários.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-149">Valid only for events that allow new time proposals.</span></span> <span data-ttu-id="2f9d2-150">A definição desse parâmetro requer \*\*\*\* a definição `true`de sendResponse como.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-150">Setting this parameter requires setting **sendResponse** to `true`.</span></span> <span data-ttu-id="2f9d2-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-151">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="2f9d2-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f9d2-152">Response</span></span>

<span data-ttu-id="2f9d2-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-p108">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="2f9d2-155">Esta ação retornará HTTP 400 se ocorrer uma das seguintes ações:</span><span class="sxs-lookup"><span data-stu-id="2f9d2-155">This action returns HTTP 400 if one or both of the following occur:</span></span>

- <span data-ttu-id="2f9d2-156">O parâmetro **proposedNewTime** está incluído, mas a propriedade **allowNewTimeProposals** do **evento** é `false`.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-156">The **proposedNewTime** parameter is included but the **allowNewTimeProposals** property of the **event** is `false`.</span></span> 
- <span data-ttu-id="2f9d2-157">O parâmetro **proposedNewTime** está incluído, mas o parâmetro **sendResponse** está definido `false`como.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-157">The **proposedNewTime** parameter is included but the **sendResponse** parameter is set to `false`.</span></span>

## <a name="example"></a><span data-ttu-id="2f9d2-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f9d2-158">Example</span></span>

<span data-ttu-id="2f9d2-159">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-159">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2f9d2-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f9d2-160">Request</span></span>

<span data-ttu-id="2f9d2-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-161">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f9d2-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f9d2-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/decline
Content-type: application/json

{
  "comment": "I won't be able to make this week. How about next week?",
  "sendResponse": true,
  "proposedNewTime": {
      "start": { 
          "dateTime": "2019-12-02T18:00:00", 
          "timeZone": "Pacific Standard Time" 
      }, 
      "end": { 
          "dateTime": "2019-12-02T19:00:00", 
          "timeZone": "Pacific Standard Time" 
      }     
  }
}
```
# <a name="c"></a>[<span data-ttu-id="2f9d2-163">C#</span><span class="sxs-lookup"><span data-stu-id="2f9d2-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f9d2-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f9d2-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f9d2-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f9d2-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2f9d2-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f9d2-166">Response</span></span>

<span data-ttu-id="2f9d2-167">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f9d2-167">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
