---
title: 'evento: forward'
description: 'Esta ação permite que o organizador ou participante de um evento de reunião encaminhe o '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f4fe8a200f1f86dd44eb5d0d2ed291c60ba10e73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006948"
---
# <a name="event-forward"></a><span data-ttu-id="76895-103">evento: forward</span><span class="sxs-lookup"><span data-stu-id="76895-103">event: forward</span></span>

<span data-ttu-id="76895-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="76895-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76895-105">Esta ação permite que o organizador ou o participante de um [evento](../resources/event.md) de reunião encaminhe a solicitação de reunião para um novo destinatário.</span><span class="sxs-lookup"><span data-stu-id="76895-105">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="76895-106">Se o evento de reunião for encaminhado da caixa de correio do Microsoft 365 de um participante para outro destinatário, essa ação também enviará uma mensagem para notificar o organizador sobre o encaminhamento e adiciona o destinatário à cópia do evento de reunião do organizador.</span><span class="sxs-lookup"><span data-stu-id="76895-106">If the meeting event is forwarded from an attendee's Microsoft 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="76895-107">Essa conveniência não está disponível no encaminhamento de uma conta do Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="76895-107">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="76895-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="76895-108">Permissions</span></span>
<span data-ttu-id="76895-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76895-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76895-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76895-111">Permission type</span></span>      | <span data-ttu-id="76895-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76895-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76895-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76895-113">Delegated (work or school account)</span></span> | <span data-ttu-id="76895-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="76895-114">Calendars.Read</span></span>    |
|<span data-ttu-id="76895-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76895-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76895-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="76895-116">Calendars.Read</span></span>    |
|<span data-ttu-id="76895-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76895-117">Application</span></span> | <span data-ttu-id="76895-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="76895-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="76895-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76895-119">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="76895-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76895-120">Request headers</span></span>
| <span data-ttu-id="76895-121">Nome</span><span class="sxs-lookup"><span data-stu-id="76895-121">Name</span></span>       | <span data-ttu-id="76895-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="76895-122">Type</span></span> | <span data-ttu-id="76895-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="76895-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="76895-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="76895-124">Authorization</span></span>  | <span data-ttu-id="76895-125">string</span><span class="sxs-lookup"><span data-stu-id="76895-125">string</span></span>  | <span data-ttu-id="76895-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76895-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76895-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76895-128">Content-Type</span></span> | <span data-ttu-id="76895-129">string</span><span class="sxs-lookup"><span data-stu-id="76895-129">string</span></span>  | <span data-ttu-id="76895-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76895-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76895-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76895-132">Request body</span></span>
<span data-ttu-id="76895-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76895-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="76895-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="76895-134">Parameter</span></span>    | <span data-ttu-id="76895-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="76895-135">Type</span></span>   |<span data-ttu-id="76895-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="76895-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76895-137">Comentário</span><span class="sxs-lookup"><span data-stu-id="76895-137">Comment</span></span>|<span data-ttu-id="76895-138">String</span><span class="sxs-lookup"><span data-stu-id="76895-138">String</span></span>|<span data-ttu-id="76895-p105">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="76895-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="76895-141">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="76895-141">ToRecipients</span></span>|<span data-ttu-id="76895-142">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="76895-142">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="76895-143">A lista de destinatários para os quais o evento será encaminhado.</span><span class="sxs-lookup"><span data-stu-id="76895-143">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="76895-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="76895-144">Response</span></span>

<span data-ttu-id="76895-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76895-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76895-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76895-147">Example</span></span>
<span data-ttu-id="76895-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="76895-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="76895-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76895-149">Request</span></span>
<span data-ttu-id="76895-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76895-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="76895-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="76895-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="76895-152">C#</span><span class="sxs-lookup"><span data-stu-id="76895-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76895-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76895-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76895-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76895-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="76895-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="76895-155">Response</span></span>
<span data-ttu-id="76895-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76895-156">Here is an example of the response.</span></span>
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
  "description": "event: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


