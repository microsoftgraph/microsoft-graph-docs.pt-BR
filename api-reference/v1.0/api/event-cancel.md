---
title: 'event: cancel'
description: 'Esta ação permite que o organizador de uma reunião envie uma mensagem de cancelamento e cancele o evento. '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e50fe07c186be9099c2a1f34f6a91982e0ee6436
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441946"
---
# <a name="event-cancel"></a><span data-ttu-id="7271b-103">event: cancel</span><span class="sxs-lookup"><span data-stu-id="7271b-103">event: cancel</span></span>

<span data-ttu-id="7271b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7271b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7271b-105">Esta ação permite que o organizador de uma reunião envie uma mensagem de cancelamento e cancele o evento.</span><span class="sxs-lookup"><span data-stu-id="7271b-105">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="7271b-106">A ação move o evento para a pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="7271b-106">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="7271b-107">O organizador também pode cancelar uma ocorrência de uma reunião recorrente fornecendo a ID do evento de ocorrência.</span><span class="sxs-lookup"><span data-stu-id="7271b-107">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="7271b-108">Um participante que chama essa ação recebe um erro (HTTP 400 Solicitação incorreta), com a seguinte mensagem de erro:</span><span class="sxs-lookup"><span data-stu-id="7271b-108">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="7271b-109">"Não é possível concluir sua solicitação.</span><span class="sxs-lookup"><span data-stu-id="7271b-109">"Your request can't be completed.</span></span> <span data-ttu-id="7271b-110">Você precisa ser um organizador para cancelar uma reunião. "</span><span class="sxs-lookup"><span data-stu-id="7271b-110">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="7271b-111">Esta ação é diferente de [Excluir](event-delete.md), sendo que **Cancelar** está disponível apenas para o organizador e permite que o organizador envie uma mensagem personalizada aos participantes sobre o cancelamento.</span><span class="sxs-lookup"><span data-stu-id="7271b-111">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="7271b-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="7271b-112">Permissions</span></span>
<span data-ttu-id="7271b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7271b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7271b-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7271b-115">Permission type</span></span>      | <span data-ttu-id="7271b-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7271b-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7271b-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7271b-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7271b-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7271b-118">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7271b-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7271b-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7271b-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7271b-120">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7271b-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7271b-121">Application</span></span> | <span data-ttu-id="7271b-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7271b-122">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7271b-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7271b-123">HTTP request</span></span>
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

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="7271b-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7271b-124">Request headers</span></span>
| <span data-ttu-id="7271b-125">Nome</span><span class="sxs-lookup"><span data-stu-id="7271b-125">Name</span></span>       | <span data-ttu-id="7271b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="7271b-126">Type</span></span> | <span data-ttu-id="7271b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="7271b-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7271b-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="7271b-128">Authorization</span></span>  | <span data-ttu-id="7271b-129">string</span><span class="sxs-lookup"><span data-stu-id="7271b-129">string</span></span>  | <span data-ttu-id="7271b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7271b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7271b-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7271b-132">Content-Type</span></span> | <span data-ttu-id="7271b-133">string</span><span class="sxs-lookup"><span data-stu-id="7271b-133">string</span></span>  | <span data-ttu-id="7271b-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7271b-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7271b-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7271b-136">Request body</span></span>
<span data-ttu-id="7271b-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7271b-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7271b-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7271b-138">Parameter</span></span>    | <span data-ttu-id="7271b-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="7271b-139">Type</span></span>   |<span data-ttu-id="7271b-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="7271b-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7271b-141">comment</span><span class="sxs-lookup"><span data-stu-id="7271b-141">comment</span></span>|<span data-ttu-id="7271b-142">String</span><span class="sxs-lookup"><span data-stu-id="7271b-142">String</span></span>|<span data-ttu-id="7271b-143">Um comentário sobre o cancelamento enviado a todos os participantes.</span><span class="sxs-lookup"><span data-stu-id="7271b-143">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="7271b-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7271b-144">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="7271b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7271b-145">Response</span></span>

<span data-ttu-id="7271b-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7271b-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7271b-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7271b-148">Example</span></span>
<span data-ttu-id="7271b-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7271b-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7271b-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7271b-150">Request</span></span>
<span data-ttu-id="7271b-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7271b-151">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7271b-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="7271b-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_cancel"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/cancel
Content-type: application/json

{
  "Comment": "Cancelling for this week due to all hands"
}
```
# <a name="c"></a>[<span data-ttu-id="7271b-153">C#</span><span class="sxs-lookup"><span data-stu-id="7271b-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7271b-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7271b-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7271b-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7271b-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7271b-156">Java</span><span class="sxs-lookup"><span data-stu-id="7271b-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="7271b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7271b-157">Response</span></span>
<span data-ttu-id="7271b-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7271b-158">Here is an example of the response.</span></span>
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
