---
title: 'evento: cancelar'
description: 'Esta ação permite que o organizador de uma reunião envie uma mensagem de cancelamento e cancele o evento. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7c73fe6df009188244b68fb9c844457ac902fd2d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323721"
---
# <a name="event-cancel"></a><span data-ttu-id="fc1d4-103">evento: cancelar</span><span class="sxs-lookup"><span data-stu-id="fc1d4-103">event: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc1d4-104">Esta ação permite que o organizador de uma reunião envie uma mensagem de cancelamento e cancele o evento.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-104">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="fc1d4-105">A ação move o evento para a pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-105">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="fc1d4-106">O organizador também pode cancelar uma ocorrência de uma reunião recorrente fornecendo a ID do evento de ocorrência.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-106">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="fc1d4-107">Um participante que chama essa ação recebe um erro (HTTP 400 Solicitação incorreta), com a seguinte mensagem de erro:</span><span class="sxs-lookup"><span data-stu-id="fc1d4-107">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="fc1d4-108">"Não é possível concluir sua solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-108">"Your request can't be completed.</span></span> <span data-ttu-id="fc1d4-109">Você precisa ser um organizador para cancelar uma reunião. "</span><span class="sxs-lookup"><span data-stu-id="fc1d4-109">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="fc1d4-110">Esta ação é diferente de [Excluir](event-delete.md), sendo que **Cancelar** está disponível apenas para o organizador e permite que o organizador envie uma mensagem personalizada aos participantes sobre o cancelamento.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-110">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc1d4-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc1d4-111">Permissions</span></span>
<span data-ttu-id="fc1d4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc1d4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc1d4-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc1d4-114">Permission type</span></span>      | <span data-ttu-id="fc1d4-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc1d4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc1d4-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc1d4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="fc1d4-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc1d4-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fc1d4-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc1d4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc1d4-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc1d4-119">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fc1d4-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc1d4-120">Application</span></span> | <span data-ttu-id="fc1d4-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc1d4-121">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc1d4-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc1d4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/cancel
POST /users/{id | userPrincipalName}/events/{id}/cancel
POST /groups/{id}/events/{id}/cancel

POST /me/calendar/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendar/events/{id}/cancel
POST /groups/{id}/calendar/events/{id}/cancel

POST /me/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/cancel

POST /me/calendargroup/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/cancel

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="fc1d4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc1d4-123">Request headers</span></span>
| <span data-ttu-id="fc1d4-124">Nome</span><span class="sxs-lookup"><span data-stu-id="fc1d4-124">Name</span></span>       | <span data-ttu-id="fc1d4-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc1d4-125">Type</span></span> | <span data-ttu-id="fc1d4-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc1d4-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fc1d4-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc1d4-127">Authorization</span></span>  | <span data-ttu-id="fc1d4-128">string</span><span class="sxs-lookup"><span data-stu-id="fc1d4-128">string</span></span>  | <span data-ttu-id="fc1d4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc1d4-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc1d4-131">Content-Type</span></span> | <span data-ttu-id="fc1d4-132">string</span><span class="sxs-lookup"><span data-stu-id="fc1d4-132">string</span></span>  | <span data-ttu-id="fc1d4-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc1d4-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc1d4-135">Request body</span></span>
<span data-ttu-id="fc1d4-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc1d4-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fc1d4-137">Parameter</span></span>    | <span data-ttu-id="fc1d4-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc1d4-138">Type</span></span>   |<span data-ttu-id="fc1d4-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc1d4-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc1d4-140">comment</span><span class="sxs-lookup"><span data-stu-id="fc1d4-140">comment</span></span>|<span data-ttu-id="fc1d4-141">String</span><span class="sxs-lookup"><span data-stu-id="fc1d4-141">String</span></span>|<span data-ttu-id="fc1d4-142">Um comentário sobre o cancelamento enviado a todos os participantes.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-142">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="fc1d4-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-143">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="fc1d4-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc1d4-144">Response</span></span>

<span data-ttu-id="fc1d4-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc1d4-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc1d4-147">Example</span></span>
<span data-ttu-id="fc1d4-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc1d4-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc1d4-149">Request</span></span>
<span data-ttu-id="fc1d4-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-150">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fc1d4-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc1d4-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/cancel
Content-type: application/json

{
  "Comment": "Cancelling for this week due to all hands"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc1d4-152">C#</span><span class="sxs-lookup"><span data-stu-id="fc1d4-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc1d4-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc1d4-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc1d4-154">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fc1d4-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fc1d4-155">Java</span><span class="sxs-lookup"><span data-stu-id="fc1d4-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fc1d4-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc1d4-156">Response</span></span>
<span data-ttu-id="fc1d4-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc1d4-157">Here is an example of the response.</span></span>
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
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
