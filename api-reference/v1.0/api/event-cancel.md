---
title: 'evento: cancelar'
description: 'Esta ação permite que o organizador de uma reunião envie uma mensagem de cancelamento e cancele o evento. '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a0d9c8dae2998d38bb9bde56fcf2cd0d49e691b9
ms.sourcegitcommit: 0cde389d4d6dbec1568dab14490f0fd6297d5aa4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720732"
---
# <a name="event-cancel"></a><span data-ttu-id="e619f-103">evento: cancelar</span><span class="sxs-lookup"><span data-stu-id="e619f-103">event: cancel</span></span>

<span data-ttu-id="e619f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e619f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e619f-105">Esta ação permite que o organizador de uma reunião envie uma mensagem de cancelamento e cancele o evento.</span><span class="sxs-lookup"><span data-stu-id="e619f-105">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="e619f-106">A ação move o evento para a pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="e619f-106">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="e619f-107">O organizador também pode cancelar uma ocorrência de uma reunião recorrente fornecendo a ID do evento de ocorrência.</span><span class="sxs-lookup"><span data-stu-id="e619f-107">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="e619f-108">Um participante que chama essa ação recebe um erro (HTTP 400 Solicitação incorreta), com a seguinte mensagem de erro:</span><span class="sxs-lookup"><span data-stu-id="e619f-108">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="e619f-109">"Não é possível concluir sua solicitação.</span><span class="sxs-lookup"><span data-stu-id="e619f-109">"Your request can't be completed.</span></span> <span data-ttu-id="e619f-110">Você precisa ser um organizador para cancelar uma reunião. "</span><span class="sxs-lookup"><span data-stu-id="e619f-110">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="e619f-111">Esta ação é diferente de [Excluir](event-delete.md), sendo que **Cancelar** está disponível apenas para o organizador e permite que o organizador envie uma mensagem personalizada aos participantes sobre o cancelamento.</span><span class="sxs-lookup"><span data-stu-id="e619f-111">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="e619f-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="e619f-112">Permissions</span></span>
<span data-ttu-id="e619f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e619f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e619f-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e619f-115">Permission type</span></span>      | <span data-ttu-id="e619f-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e619f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e619f-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e619f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e619f-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e619f-118">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e619f-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e619f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e619f-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e619f-120">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e619f-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e619f-121">Application</span></span> | <span data-ttu-id="e619f-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e619f-122">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e619f-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e619f-123">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="e619f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e619f-124">Request headers</span></span>
| <span data-ttu-id="e619f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="e619f-125">Name</span></span>       | <span data-ttu-id="e619f-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e619f-126">Type</span></span> | <span data-ttu-id="e619f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e619f-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e619f-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="e619f-128">Authorization</span></span>  | <span data-ttu-id="e619f-129">string</span><span class="sxs-lookup"><span data-stu-id="e619f-129">string</span></span>  | <span data-ttu-id="e619f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e619f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e619f-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e619f-132">Content-Type</span></span> | <span data-ttu-id="e619f-133">string</span><span class="sxs-lookup"><span data-stu-id="e619f-133">string</span></span>  | <span data-ttu-id="e619f-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e619f-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e619f-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e619f-136">Request body</span></span>
<span data-ttu-id="e619f-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e619f-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e619f-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e619f-138">Parameter</span></span>    | <span data-ttu-id="e619f-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="e619f-139">Type</span></span>   |<span data-ttu-id="e619f-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="e619f-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e619f-141">comment</span><span class="sxs-lookup"><span data-stu-id="e619f-141">comment</span></span>|<span data-ttu-id="e619f-142">String</span><span class="sxs-lookup"><span data-stu-id="e619f-142">String</span></span>|<span data-ttu-id="e619f-143">Um comentário sobre o cancelamento enviado a todos os participantes.</span><span class="sxs-lookup"><span data-stu-id="e619f-143">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="e619f-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e619f-144">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="e619f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e619f-145">Response</span></span>

<span data-ttu-id="e619f-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e619f-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e619f-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e619f-148">Example</span></span>
<span data-ttu-id="e619f-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e619f-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e619f-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e619f-150">Request</span></span>
<span data-ttu-id="e619f-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e619f-151">Here is an example of the request.</span></span>

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


##### <a name="response"></a><span data-ttu-id="e619f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e619f-152">Response</span></span>
<span data-ttu-id="e619f-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e619f-153">Here is an example of the response.</span></span>
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
