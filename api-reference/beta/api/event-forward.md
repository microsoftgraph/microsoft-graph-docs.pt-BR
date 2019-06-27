---
title: 'evento: forward'
description: 'Esta ação permite que o organizador ou participante de um evento de reunião encaminhe o '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5da653eab0dd1d3ab97a3df8bf0de0ffd110c0e3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259154"
---
# <a name="event-forward"></a><span data-ttu-id="20ff8-103">evento: forward</span><span class="sxs-lookup"><span data-stu-id="20ff8-103">event: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20ff8-104">Esta ação permite que o organizador ou o participante de um [evento](../resources/event.md) de reunião encaminhe a solicitação de reunião para um novo destinatário.</span><span class="sxs-lookup"><span data-stu-id="20ff8-104">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="20ff8-105">Se o evento de reunião for encaminhado da caixa de correio do Office 365 de um participante para outro destinatário, essa ação também enviará uma mensagem para notificar o organizador sobre o encaminhamento e adiciona o destinatário à cópia do evento de reunião do organizador.</span><span class="sxs-lookup"><span data-stu-id="20ff8-105">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="20ff8-106">Essa conveniência não está disponível no encaminhamento de uma conta do Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="20ff8-106">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="20ff8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="20ff8-107">Permissions</span></span>
<span data-ttu-id="20ff8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20ff8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20ff8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20ff8-110">Permission type</span></span>      | <span data-ttu-id="20ff8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20ff8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20ff8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20ff8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="20ff8-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="20ff8-113">Calendars.Read</span></span>    |
|<span data-ttu-id="20ff8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20ff8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20ff8-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="20ff8-115">Calendars.Read</span></span>    |
|<span data-ttu-id="20ff8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20ff8-116">Application</span></span> | <span data-ttu-id="20ff8-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="20ff8-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="20ff8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20ff8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/forward
POST /users/{id | userPrincipalName}/events/{id}/forward
POST /groups/{id}/events/{id}/forward

POST /me/calendar/events/{id}/forward
POST /users/{id | userPrincipalName}/calendar/events/{id}/forward
POST /groups/{id}/calendar/events/{id}/forward

POST /me/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/forward

POST /me/calendargroup/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/forward

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="20ff8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20ff8-119">Request headers</span></span>
| <span data-ttu-id="20ff8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="20ff8-120">Name</span></span>       | <span data-ttu-id="20ff8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="20ff8-121">Type</span></span> | <span data-ttu-id="20ff8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="20ff8-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="20ff8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="20ff8-123">Authorization</span></span>  | <span data-ttu-id="20ff8-124">string</span><span class="sxs-lookup"><span data-stu-id="20ff8-124">string</span></span>  | <span data-ttu-id="20ff8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20ff8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20ff8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20ff8-127">Content-Type</span></span> | <span data-ttu-id="20ff8-128">string</span><span class="sxs-lookup"><span data-stu-id="20ff8-128">string</span></span>  | <span data-ttu-id="20ff8-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20ff8-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20ff8-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20ff8-131">Request body</span></span>
<span data-ttu-id="20ff8-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20ff8-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20ff8-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="20ff8-133">Parameter</span></span>    | <span data-ttu-id="20ff8-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="20ff8-134">Type</span></span>   |<span data-ttu-id="20ff8-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="20ff8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20ff8-136">Comentário</span><span class="sxs-lookup"><span data-stu-id="20ff8-136">Comment</span></span>|<span data-ttu-id="20ff8-137">String</span><span class="sxs-lookup"><span data-stu-id="20ff8-137">String</span></span>|<span data-ttu-id="20ff8-p105">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="20ff8-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="20ff8-140">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="20ff8-140">ToRecipients</span></span>|<span data-ttu-id="20ff8-141">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="20ff8-141">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="20ff8-142">A lista de destinatários para os quais o evento será encaminhado.</span><span class="sxs-lookup"><span data-stu-id="20ff8-142">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="20ff8-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="20ff8-143">Response</span></span>

<span data-ttu-id="20ff8-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20ff8-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20ff8-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20ff8-146">Example</span></span>
<span data-ttu-id="20ff8-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="20ff8-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="20ff8-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20ff8-148">Request</span></span>
<span data-ttu-id="20ff8-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20ff8-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/forward
Content-type: application/json
Content-length: 56

{
  "ToRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ],
  "Comment": "Dana, hope you can make this meeting." 
}

```

##### <a name="response"></a><span data-ttu-id="20ff8-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="20ff8-150">Response</span></span>
<span data-ttu-id="20ff8-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20ff8-151">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="20ff8-152">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="20ff8-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="20ff8-153">C#</span><span class="sxs-lookup"><span data-stu-id="20ff8-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_forward-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20ff8-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="20ff8-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_forward-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="20ff8-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="20ff8-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/event_forward-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-forward.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/event-forward.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-forward.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
