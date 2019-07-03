---
title: 'evento: forward'
description: 'Esta ação permite que o organizador ou participante de um evento de reunião encaminhe o '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5ad26f76ff9d71bf453f967ad00f3018f6ce4361
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441069"
---
# <a name="event-forward"></a><span data-ttu-id="08a38-103">evento: forward</span><span class="sxs-lookup"><span data-stu-id="08a38-103">event: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08a38-104">Esta ação permite que o organizador ou o participante de um [evento](../resources/event.md) de reunião encaminhe a solicitação de reunião para um novo destinatário.</span><span class="sxs-lookup"><span data-stu-id="08a38-104">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="08a38-105">Se o evento de reunião for encaminhado da caixa de correio do Office 365 de um participante para outro destinatário, essa ação também enviará uma mensagem para notificar o organizador sobre o encaminhamento e adiciona o destinatário à cópia do evento de reunião do organizador.</span><span class="sxs-lookup"><span data-stu-id="08a38-105">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="08a38-106">Essa conveniência não está disponível no encaminhamento de uma conta do Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="08a38-106">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="08a38-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="08a38-107">Permissions</span></span>
<span data-ttu-id="08a38-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08a38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08a38-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08a38-110">Permission type</span></span>      | <span data-ttu-id="08a38-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08a38-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08a38-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08a38-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08a38-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="08a38-113">Calendars.Read</span></span>    |
|<span data-ttu-id="08a38-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08a38-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08a38-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="08a38-115">Calendars.Read</span></span>    |
|<span data-ttu-id="08a38-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08a38-116">Application</span></span> | <span data-ttu-id="08a38-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="08a38-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="08a38-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08a38-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="08a38-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08a38-119">Request headers</span></span>
| <span data-ttu-id="08a38-120">Nome</span><span class="sxs-lookup"><span data-stu-id="08a38-120">Name</span></span>       | <span data-ttu-id="08a38-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="08a38-121">Type</span></span> | <span data-ttu-id="08a38-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="08a38-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08a38-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="08a38-123">Authorization</span></span>  | <span data-ttu-id="08a38-124">string</span><span class="sxs-lookup"><span data-stu-id="08a38-124">string</span></span>  | <span data-ttu-id="08a38-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08a38-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08a38-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08a38-127">Content-Type</span></span> | <span data-ttu-id="08a38-128">string</span><span class="sxs-lookup"><span data-stu-id="08a38-128">string</span></span>  | <span data-ttu-id="08a38-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08a38-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08a38-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08a38-131">Request body</span></span>
<span data-ttu-id="08a38-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08a38-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="08a38-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="08a38-133">Parameter</span></span>    | <span data-ttu-id="08a38-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="08a38-134">Type</span></span>   |<span data-ttu-id="08a38-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="08a38-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08a38-136">Comentário</span><span class="sxs-lookup"><span data-stu-id="08a38-136">Comment</span></span>|<span data-ttu-id="08a38-137">String</span><span class="sxs-lookup"><span data-stu-id="08a38-137">String</span></span>|<span data-ttu-id="08a38-p105">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="08a38-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="08a38-140">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="08a38-140">ToRecipients</span></span>|<span data-ttu-id="08a38-141">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="08a38-141">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="08a38-142">A lista de destinatários para os quais o evento será encaminhado.</span><span class="sxs-lookup"><span data-stu-id="08a38-142">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="08a38-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="08a38-143">Response</span></span>

<span data-ttu-id="08a38-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08a38-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08a38-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08a38-146">Example</span></span>
<span data-ttu-id="08a38-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="08a38-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="08a38-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08a38-148">Request</span></span>
<span data-ttu-id="08a38-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08a38-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="08a38-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="08a38-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="08a38-151">C#</span><span class="sxs-lookup"><span data-stu-id="08a38-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08a38-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="08a38-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08a38-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="08a38-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="08a38-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="08a38-154">Response</span></span>
<span data-ttu-id="08a38-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08a38-155">Here is an example of the response.</span></span>
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
