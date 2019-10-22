---
title: 'event: tentativelyAccept'
description: Aceitar provisoriamente o evento específico em um calendário de usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b9bdcd71033c1e1c21f7ba3768e357bbe5c70084
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621424"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="ac729-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="ac729-103">event: tentativelyAccept</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac729-104">Aceitar provisoriamente o [evento](../resources/event.md) especificado em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac729-104">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

<span data-ttu-id="ac729-105">Se o evento permitir propostas para novas horas, em resposta provisória ao evento, um convidado poderá optar por sugerir um tempo alternativo, incluindo o parâmetro **proposedNewTime** .</span><span class="sxs-lookup"><span data-stu-id="ac729-105">If the event allows proposals for new times, on responding tentative to the event, an invitee can choose to suggest an alternative time by including the **proposedNewTime** parameter.</span></span> <span data-ttu-id="ac729-106">Para obter mais informações sobre como propor um horário e como receber e aceitar uma nova proposta de tempo, confira [propor novos horários da reunião](/graph/outlook-calendar-meeting-proposals).</span><span class="sxs-lookup"><span data-stu-id="ac729-106">For more information on how to propose a time, and how to receive and accept a new time proposal, see [Propose new meeting times](/graph/outlook-calendar-meeting-proposals).</span></span>

## <a name="permissions"></a><span data-ttu-id="ac729-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac729-107">Permissions</span></span>
<span data-ttu-id="ac729-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac729-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac729-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac729-110">Permission type</span></span>      | <span data-ttu-id="ac729-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac729-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac729-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac729-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ac729-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac729-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ac729-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac729-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac729-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac729-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ac729-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac729-116">Application</span></span> | <span data-ttu-id="ac729-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac729-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac729-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac729-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="ac729-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac729-119">Request headers</span></span>
| <span data-ttu-id="ac729-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ac729-120">Name</span></span>       | <span data-ttu-id="ac729-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac729-121">Type</span></span> | <span data-ttu-id="ac729-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac729-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ac729-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac729-123">Authorization</span></span>  | <span data-ttu-id="ac729-124">string</span><span class="sxs-lookup"><span data-stu-id="ac729-124">string</span></span>  | <span data-ttu-id="ac729-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac729-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ac729-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac729-127">Content-Type</span></span> | <span data-ttu-id="ac729-128">string</span><span class="sxs-lookup"><span data-stu-id="ac729-128">string</span></span>  | <span data-ttu-id="ac729-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac729-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac729-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac729-131">Request body</span></span>
<span data-ttu-id="ac729-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac729-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ac729-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ac729-133">Parameter</span></span>    | <span data-ttu-id="ac729-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac729-134">Type</span></span>   |<span data-ttu-id="ac729-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac729-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac729-136">comment</span><span class="sxs-lookup"><span data-stu-id="ac729-136">comment</span></span>|<span data-ttu-id="ac729-137">String</span><span class="sxs-lookup"><span data-stu-id="ac729-137">String</span></span>|<span data-ttu-id="ac729-p105">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ac729-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="ac729-140">sendResponse</span><span class="sxs-lookup"><span data-stu-id="ac729-140">sendResponse</span></span>|<span data-ttu-id="ac729-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac729-141">Boolean</span></span>|<span data-ttu-id="ac729-p106">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="ac729-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|
|<span data-ttu-id="ac729-145">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="ac729-145">proposedNewTime</span></span>|[<span data-ttu-id="ac729-146">timeSlot</span><span class="sxs-lookup"><span data-stu-id="ac729-146">timeSlot</span></span>](../resources/timeslot.md)|<span data-ttu-id="ac729-147">Uma data/hora alternativa propostas por um convidado para uma solicitação de reunião para iniciar e finalizar.</span><span class="sxs-lookup"><span data-stu-id="ac729-147">An alternate date/time proposed by an invitee for a meeting request to start and end.</span></span> <span data-ttu-id="ac729-148">Válido somente para eventos que permitem novas propostas de horários.</span><span class="sxs-lookup"><span data-stu-id="ac729-148">Valid only for events that allow new time proposals.</span></span> <span data-ttu-id="ac729-149">A definição desse parâmetro requer \*\*\*\* a definição `true`de sendResponse como.</span><span class="sxs-lookup"><span data-stu-id="ac729-149">Setting this parameter requires setting **sendResponse** to `true`.</span></span> <span data-ttu-id="ac729-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ac729-150">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="ac729-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac729-151">Response</span></span>

<span data-ttu-id="ac729-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac729-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="ac729-154">Esta ação retornará HTTP 400 se ocorrer uma das seguintes ações:</span><span class="sxs-lookup"><span data-stu-id="ac729-154">This action returns HTTP 400 if one or both of the following occur:</span></span>

- <span data-ttu-id="ac729-155">O parâmetro **proposedNewTime** está incluído, mas a propriedade **allowNewTimeProposals** do **evento** é `false`.</span><span class="sxs-lookup"><span data-stu-id="ac729-155">The **proposedNewTime** parameter is included but the **allowNewTimeProposals** property of the **event** is `false`.</span></span> 
- <span data-ttu-id="ac729-156">O parâmetro **proposedNewTime** está incluído, mas o parâmetro **sendResponse** está definido `false`como.</span><span class="sxs-lookup"><span data-stu-id="ac729-156">The **proposedNewTime** parameter is included but the **sendResponse** parameter is set to `false`.</span></span>

## <a name="example"></a><span data-ttu-id="ac729-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac729-157">Example</span></span>
<span data-ttu-id="ac729-158">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ac729-158">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="ac729-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac729-159">Request</span></span>
<span data-ttu-id="ac729-160">No exemplo a seguir, o usuário conectado responde provisoriamente ao evento especificado, define o **sendResponse** paremeter como true e inclui um momento alternativo no parâmetro **proposedNewTime** .</span><span class="sxs-lookup"><span data-stu-id="ac729-160">In the following example, the signed-in user responds tentative to the specified event, sets the **sendResponse** paremeter to true, and includes an alternative time in the **proposedNewTime** parameter.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ac729-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac729-161">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ac729-162">C#</span><span class="sxs-lookup"><span data-stu-id="ac729-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac729-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac729-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ac729-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac729-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ac729-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac729-165">Response</span></span>
<span data-ttu-id="ac729-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac729-166">Here is an example of the response.</span></span>
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
