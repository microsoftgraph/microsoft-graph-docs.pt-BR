---
title: 'event: decline'
description: Recusar o convite para o evento específico em um calendário de usuário.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7d6c89e6b143373e6e1e3822a192dd443ecf7bd9
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992280"
---
# <a name="event-decline"></a><span data-ttu-id="95386-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="95386-103">event: decline</span></span>

<span data-ttu-id="95386-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95386-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95386-105">Recusar convite para o evento [especificado](../resources/event.md) em um calendário do [usuário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="95386-105">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

<span data-ttu-id="95386-106">Se o evento permitir propostas para novos horários, ao declinar o evento, um convidado poderá optar por sugerir uma hora alternativa incluindo o parâmetro **proposedNewTime.**</span><span class="sxs-lookup"><span data-stu-id="95386-106">If the event allows proposals for new times, on declining the event, an invitee can choose to suggest an alternative time by including the **proposedNewTime** parameter.</span></span> <span data-ttu-id="95386-107">Para obter mais informações sobre como propor uma hora e como receber e aceitar uma nova proposta de hora, consulte [Propor novos horários de reunião.](/graph/outlook-calendar-meeting-proposals)</span><span class="sxs-lookup"><span data-stu-id="95386-107">For more information on how to propose a time, and how to receive and accept a new time proposal, see [Propose new meeting times](/graph/outlook-calendar-meeting-proposals).</span></span>


## <a name="permissions"></a><span data-ttu-id="95386-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="95386-108">Permissions</span></span>
<span data-ttu-id="95386-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95386-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95386-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95386-111">Permission type</span></span>      | <span data-ttu-id="95386-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95386-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95386-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95386-113">Delegated (work or school account)</span></span> | <span data-ttu-id="95386-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95386-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="95386-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95386-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95386-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95386-116">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="95386-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95386-117">Application</span></span> | <span data-ttu-id="95386-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95386-118">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="95386-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95386-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/decline
POST /users/{id | userPrincipalName}/events/{id}/decline

POST /me/calendar/events/{id}/decline
POST /users/{id | userPrincipalName}/calendar/events/{id}/decline

POST /me/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="95386-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95386-120">Request headers</span></span>

| <span data-ttu-id="95386-121">Nome</span><span class="sxs-lookup"><span data-stu-id="95386-121">Name</span></span>       | <span data-ttu-id="95386-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="95386-122">Type</span></span> | <span data-ttu-id="95386-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="95386-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="95386-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="95386-124">Authorization</span></span>  | <span data-ttu-id="95386-125">string</span><span class="sxs-lookup"><span data-stu-id="95386-125">string</span></span>  | <span data-ttu-id="95386-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95386-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="95386-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95386-128">Content-Type</span></span> | <span data-ttu-id="95386-129">string</span><span class="sxs-lookup"><span data-stu-id="95386-129">string</span></span>  | <span data-ttu-id="95386-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95386-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95386-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95386-132">Request body</span></span>

<span data-ttu-id="95386-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95386-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="95386-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="95386-134">Parameter</span></span>    | <span data-ttu-id="95386-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="95386-135">Type</span></span>   |<span data-ttu-id="95386-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="95386-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95386-137">comment</span><span class="sxs-lookup"><span data-stu-id="95386-137">comment</span></span>|<span data-ttu-id="95386-138">String</span><span class="sxs-lookup"><span data-stu-id="95386-138">String</span></span>|<span data-ttu-id="95386-p105">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="95386-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="95386-141">sendResponse</span><span class="sxs-lookup"><span data-stu-id="95386-141">sendResponse</span></span>|<span data-ttu-id="95386-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="95386-142">Boolean</span></span>|<span data-ttu-id="95386-p106">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="95386-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|
|<span data-ttu-id="95386-146">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="95386-146">proposedNewTime</span></span>|[<span data-ttu-id="95386-147">timeSlot</span><span class="sxs-lookup"><span data-stu-id="95386-147">timeSlot</span></span>](../resources/timeslot.md)|<span data-ttu-id="95386-148">Uma data/hora alternativa proposta por um convidado para que uma solicitação de reunião seja inicial e final.</span><span class="sxs-lookup"><span data-stu-id="95386-148">An alternate date/time proposed by an invitee for a meeting request to start and end.</span></span> <span data-ttu-id="95386-149">Válido somente para eventos que permitem novas propostas de tempo.</span><span class="sxs-lookup"><span data-stu-id="95386-149">Valid only for events that allow new time proposals.</span></span> <span data-ttu-id="95386-150">A configuração desse parâmetro requer **a definição de sendResponse** como `true` .</span><span class="sxs-lookup"><span data-stu-id="95386-150">Setting this parameter requires setting **sendResponse** to `true`.</span></span> <span data-ttu-id="95386-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="95386-151">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="95386-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="95386-152">Response</span></span>

<span data-ttu-id="95386-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95386-p108">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="95386-155">Essa ação retornará HTTP 400 se ocorrer um ou ambos os seguintes:</span><span class="sxs-lookup"><span data-stu-id="95386-155">This action returns HTTP 400 if one or both of the following occur:</span></span>

- <span data-ttu-id="95386-156">O **parâmetro proposedNewTime** está incluído, **mas a propriedade allowNewTimeProposals** do **evento** é `false` .</span><span class="sxs-lookup"><span data-stu-id="95386-156">The **proposedNewTime** parameter is included but the **allowNewTimeProposals** property of the **event** is `false`.</span></span> 
- <span data-ttu-id="95386-157">O **parâmetro proposedNewTime** está incluído, mas o **parâmetro sendResponse** é definido como `false` .</span><span class="sxs-lookup"><span data-stu-id="95386-157">The **proposedNewTime** parameter is included but the **sendResponse** parameter is set to `false`.</span></span>

## <a name="example"></a><span data-ttu-id="95386-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95386-158">Example</span></span>

<span data-ttu-id="95386-159">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="95386-159">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="95386-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95386-160">Request</span></span>

<span data-ttu-id="95386-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95386-161">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="95386-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="95386-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="95386-163">C#</span><span class="sxs-lookup"><span data-stu-id="95386-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95386-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95386-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95386-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95386-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95386-166">Java</span><span class="sxs-lookup"><span data-stu-id="95386-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="95386-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="95386-167">Response</span></span>

<span data-ttu-id="95386-168">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95386-168">Here is an example of the response.</span></span>

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


