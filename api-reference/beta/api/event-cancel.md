---
title: 'evento: Cancelar'
description: 'Esta ação permite que o organizador de uma reunião envie uma mensagem de cancelamento e cancele o evento. '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 482804d58078f148ed321a0c3489954fc9144f8e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864621"
---
# <a name="event-cancel"></a><span data-ttu-id="55d96-103">evento: Cancelar</span><span class="sxs-lookup"><span data-stu-id="55d96-103">event: cancel</span></span>

> <span data-ttu-id="55d96-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="55d96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55d96-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="55d96-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55d96-106">Esta ação permite que o organizador de uma reunião envie uma mensagem de cancelamento e cancele o evento.</span><span class="sxs-lookup"><span data-stu-id="55d96-106">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="55d96-107">A ação move o evento para a pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="55d96-107">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="55d96-108">O organizador também pode cancelar uma ocorrência de uma reunião recorrente fornecendo a ID do evento de ocorrência.</span><span class="sxs-lookup"><span data-stu-id="55d96-108">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="55d96-109">Um participante que chama essa ação recebe um erro (HTTP 400 Solicitação incorreta), com a seguinte mensagem de erro:</span><span class="sxs-lookup"><span data-stu-id="55d96-109">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="55d96-110">"Não é possível concluir sua solicitação.</span><span class="sxs-lookup"><span data-stu-id="55d96-110">"Your request can't be completed.</span></span> <span data-ttu-id="55d96-111">Você precisa ser um organizador para cancelar uma reunião. "</span><span class="sxs-lookup"><span data-stu-id="55d96-111">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="55d96-112">Esta ação é diferente de [Excluir](event-delete.md), sendo que **Cancelar** está disponível apenas para o organizador e permite que o organizador envie uma mensagem personalizada aos participantes sobre o cancelamento.</span><span class="sxs-lookup"><span data-stu-id="55d96-112">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="55d96-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="55d96-113">Permissions</span></span>
<span data-ttu-id="55d96-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55d96-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55d96-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55d96-116">Permission type</span></span>      | <span data-ttu-id="55d96-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55d96-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55d96-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55d96-118">Delegated (work or school account)</span></span> | <span data-ttu-id="55d96-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55d96-119">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="55d96-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55d96-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55d96-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55d96-121">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="55d96-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55d96-122">Application</span></span> | <span data-ttu-id="55d96-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55d96-123">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="55d96-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55d96-124">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="55d96-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55d96-125">Request headers</span></span>
| <span data-ttu-id="55d96-126">Nome</span><span class="sxs-lookup"><span data-stu-id="55d96-126">Name</span></span>       | <span data-ttu-id="55d96-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="55d96-127">Type</span></span> | <span data-ttu-id="55d96-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="55d96-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55d96-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="55d96-129">Authorization</span></span>  | <span data-ttu-id="55d96-130">string</span><span class="sxs-lookup"><span data-stu-id="55d96-130">string</span></span>  | <span data-ttu-id="55d96-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55d96-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="55d96-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55d96-133">Content-Type</span></span> | <span data-ttu-id="55d96-134">string</span><span class="sxs-lookup"><span data-stu-id="55d96-134">string</span></span>  | <span data-ttu-id="55d96-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55d96-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55d96-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55d96-137">Request body</span></span>
<span data-ttu-id="55d96-138">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55d96-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="55d96-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="55d96-139">Parameter</span></span>    | <span data-ttu-id="55d96-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="55d96-140">Type</span></span>   |<span data-ttu-id="55d96-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="55d96-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55d96-142">comment</span><span class="sxs-lookup"><span data-stu-id="55d96-142">comment</span></span>|<span data-ttu-id="55d96-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55d96-143">String</span></span>|<span data-ttu-id="55d96-144">Um comentário sobre o cancelamento enviado a todos os participantes.</span><span class="sxs-lookup"><span data-stu-id="55d96-144">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="55d96-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="55d96-145">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="55d96-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="55d96-146">Response</span></span>

<span data-ttu-id="55d96-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55d96-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55d96-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55d96-149">Example</span></span>
<span data-ttu-id="55d96-150">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="55d96-150">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="55d96-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55d96-151">Request</span></span>
<span data-ttu-id="55d96-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55d96-152">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="55d96-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="55d96-153">Response</span></span>
<span data-ttu-id="55d96-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55d96-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
