---
title: 'event: tentativelyAccept'
description: Aceitar provisoriamente o evento específico em um calendário de usuário.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2d4060489167c438077e85800e04c2973adf6a58
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436138"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="bdd80-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="bdd80-103">event: tentativelyAccept</span></span>

<span data-ttu-id="bdd80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdd80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdd80-105">Aceite provisamente o evento [especificado](../resources/event.md) em um calendário do [usuário.](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="bdd80-105">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

<span data-ttu-id="bdd80-106">Se o evento permitir propostas para novos horários, ao responder provisão ao evento, um convidado pode optar por sugerir uma hora alternativa incluindo o parâmetro **proposedNewTime.**</span><span class="sxs-lookup"><span data-stu-id="bdd80-106">If the event allows proposals for new times, on responding tentative to the event, an invitee can choose to suggest an alternative time by including the **proposedNewTime** parameter.</span></span> <span data-ttu-id="bdd80-107">Para obter mais informações sobre como propor uma hora e como receber e aceitar uma nova proposta de hora, consulte [Propor novos horários de reunião.](/graph/outlook-calendar-meeting-proposals)</span><span class="sxs-lookup"><span data-stu-id="bdd80-107">For more information on how to propose a time, and how to receive and accept a new time proposal, see [Propose new meeting times](/graph/outlook-calendar-meeting-proposals).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdd80-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdd80-108">Permissions</span></span>
<span data-ttu-id="bdd80-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdd80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdd80-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdd80-111">Permission type</span></span>      | <span data-ttu-id="bdd80-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdd80-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdd80-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdd80-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bdd80-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdd80-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bdd80-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdd80-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdd80-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdd80-116">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bdd80-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdd80-117">Application</span></span> | <span data-ttu-id="bdd80-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdd80-118">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdd80-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdd80-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="bdd80-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdd80-120">Request headers</span></span>
| <span data-ttu-id="bdd80-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bdd80-121">Name</span></span>       | <span data-ttu-id="bdd80-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdd80-122">Type</span></span> | <span data-ttu-id="bdd80-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdd80-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bdd80-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdd80-124">Authorization</span></span>  | <span data-ttu-id="bdd80-125">string</span><span class="sxs-lookup"><span data-stu-id="bdd80-125">string</span></span>  | <span data-ttu-id="bdd80-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdd80-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bdd80-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bdd80-128">Content-Type</span></span> | <span data-ttu-id="bdd80-129">string</span><span class="sxs-lookup"><span data-stu-id="bdd80-129">string</span></span>  | <span data-ttu-id="bdd80-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdd80-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdd80-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdd80-132">Request body</span></span>
<span data-ttu-id="bdd80-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdd80-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bdd80-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bdd80-134">Parameter</span></span>    | <span data-ttu-id="bdd80-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdd80-135">Type</span></span>   |<span data-ttu-id="bdd80-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdd80-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdd80-137">comment</span><span class="sxs-lookup"><span data-stu-id="bdd80-137">comment</span></span>|<span data-ttu-id="bdd80-138">String</span><span class="sxs-lookup"><span data-stu-id="bdd80-138">String</span></span>|<span data-ttu-id="bdd80-p105">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bdd80-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="bdd80-141">sendResponse</span><span class="sxs-lookup"><span data-stu-id="bdd80-141">sendResponse</span></span>|<span data-ttu-id="bdd80-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="bdd80-142">Boolean</span></span>|<span data-ttu-id="bdd80-p106">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="bdd80-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|
|<span data-ttu-id="bdd80-146">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="bdd80-146">proposedNewTime</span></span>|[<span data-ttu-id="bdd80-147">timeSlot</span><span class="sxs-lookup"><span data-stu-id="bdd80-147">timeSlot</span></span>](../resources/timeslot.md)|<span data-ttu-id="bdd80-148">Uma data/hora alternativa proposta por um convidado para que uma solicitação de reunião seja inicial e final.</span><span class="sxs-lookup"><span data-stu-id="bdd80-148">An alternate date/time proposed by an invitee for a meeting request to start and end.</span></span> <span data-ttu-id="bdd80-149">Válido somente para eventos que permitem novas propostas de tempo.</span><span class="sxs-lookup"><span data-stu-id="bdd80-149">Valid only for events that allow new time proposals.</span></span> <span data-ttu-id="bdd80-150">A configuração desse parâmetro requer **a definição de sendResponse** como `true` .</span><span class="sxs-lookup"><span data-stu-id="bdd80-150">Setting this parameter requires setting **sendResponse** to `true`.</span></span> <span data-ttu-id="bdd80-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bdd80-151">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="bdd80-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdd80-152">Response</span></span>

<span data-ttu-id="bdd80-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdd80-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="bdd80-155">Essa ação retornará HTTP 400 se ocorrer um ou ambos os seguintes:</span><span class="sxs-lookup"><span data-stu-id="bdd80-155">This action returns HTTP 400 if one or both of the following occur:</span></span>

- <span data-ttu-id="bdd80-156">O **parâmetro proposedNewTime** está incluído, **mas a propriedade allowNewTimeProposals** do **evento** é `false` .</span><span class="sxs-lookup"><span data-stu-id="bdd80-156">The **proposedNewTime** parameter is included but the **allowNewTimeProposals** property of the **event** is `false`.</span></span> 
- <span data-ttu-id="bdd80-157">O **parâmetro proposedNewTime** está incluído, mas o **parâmetro sendResponse** é definido como `false` .</span><span class="sxs-lookup"><span data-stu-id="bdd80-157">The **proposedNewTime** parameter is included but the **sendResponse** parameter is set to `false`.</span></span>

## <a name="example"></a><span data-ttu-id="bdd80-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdd80-158">Example</span></span>
<span data-ttu-id="bdd80-159">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="bdd80-159">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="bdd80-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdd80-160">Request</span></span>
<span data-ttu-id="bdd80-161">No exemplo a seguir, o usuário in-loco responde provisivo ao evento especificado, define o parâmetro **sendResponse** como true e inclui uma hora alternativa no parâmetro **proposedNewTime.**</span><span class="sxs-lookup"><span data-stu-id="bdd80-161">In the following example, the signed-in user responds tentative to the specified event, sets the **sendResponse** parameter to true, and includes an alternative time in the **proposedNewTime** parameter.</span></span>

# <a name="http"></a>[<span data-ttu-id="bdd80-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdd80-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/tentativelyAccept
Content-type: application/json

{
  "comment": "I may not be able to make this week. How about next week?",
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
# <a name="c"></a>[<span data-ttu-id="bdd80-163">C#</span><span class="sxs-lookup"><span data-stu-id="bdd80-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bdd80-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdd80-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bdd80-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdd80-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="bdd80-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdd80-166">Response</span></span>
<span data-ttu-id="bdd80-167">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdd80-167">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "event_tentativelyaccept",
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
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


