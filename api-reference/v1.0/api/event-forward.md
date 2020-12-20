---
title: 'evento: forward'
description: 'Esta ação permite que o organizador ou participante de um evento de reunião encaminhe o '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 624312256cbca37529eb55eececa136df04d69fe
ms.sourcegitcommit: 0cde389d4d6dbec1568dab14490f0fd6297d5aa4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720736"
---
# <a name="event-forward"></a><span data-ttu-id="e9e19-103">evento: forward</span><span class="sxs-lookup"><span data-stu-id="e9e19-103">event: forward</span></span>

<span data-ttu-id="e9e19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9e19-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e9e19-105">Esta ação permite que o organizador ou o participante de um [evento](../resources/event.md) de reunião encaminhe a solicitação de reunião para um novo destinatário.</span><span class="sxs-lookup"><span data-stu-id="e9e19-105">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="e9e19-106">Se o evento de reunião for encaminhado da caixa de correio do Microsoft 365 de um participante para outro destinatário, essa ação também enviará uma mensagem para notificar o organizador sobre o encaminhamento e adiciona o destinatário à cópia do evento de reunião do organizador.</span><span class="sxs-lookup"><span data-stu-id="e9e19-106">If the meeting event is forwarded from an attendee's Microsoft 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="e9e19-107">Essa conveniência não está disponível no encaminhamento de uma conta do Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="e9e19-107">This convenience is not available when forwarding from an Outlook.com account.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9e19-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9e19-108">Permissions</span></span>
<span data-ttu-id="e9e19-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9e19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9e19-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9e19-111">Permission type</span></span>      | <span data-ttu-id="e9e19-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9e19-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9e19-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9e19-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e9e19-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e9e19-114">Calendars.Read</span></span>    |
|<span data-ttu-id="e9e19-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9e19-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9e19-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e9e19-116">Calendars.Read</span></span>    |
|<span data-ttu-id="e9e19-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9e19-117">Application</span></span> | <span data-ttu-id="e9e19-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e9e19-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9e19-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9e19-119">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="e9e19-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9e19-120">Request headers</span></span>
| <span data-ttu-id="e9e19-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e9e19-121">Name</span></span>       | <span data-ttu-id="e9e19-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9e19-122">Type</span></span> | <span data-ttu-id="e9e19-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9e19-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e9e19-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9e19-124">Authorization</span></span>  | <span data-ttu-id="e9e19-125">string</span><span class="sxs-lookup"><span data-stu-id="e9e19-125">string</span></span>  | <span data-ttu-id="e9e19-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9e19-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9e19-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9e19-128">Content-Type</span></span> | <span data-ttu-id="e9e19-129">string</span><span class="sxs-lookup"><span data-stu-id="e9e19-129">string</span></span>  | <span data-ttu-id="e9e19-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9e19-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9e19-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9e19-132">Request body</span></span>
<span data-ttu-id="e9e19-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9e19-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e9e19-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e9e19-134">Parameter</span></span>    | <span data-ttu-id="e9e19-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9e19-135">Type</span></span>   |<span data-ttu-id="e9e19-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9e19-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9e19-137">Comentário</span><span class="sxs-lookup"><span data-stu-id="e9e19-137">Comment</span></span>|<span data-ttu-id="e9e19-138">String</span><span class="sxs-lookup"><span data-stu-id="e9e19-138">String</span></span>|<span data-ttu-id="e9e19-p105">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="e9e19-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="e9e19-141">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="e9e19-141">ToRecipients</span></span>|<span data-ttu-id="e9e19-142">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="e9e19-142">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="e9e19-143">A lista de destinatários para os quais o evento será encaminhado.</span><span class="sxs-lookup"><span data-stu-id="e9e19-143">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="e9e19-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9e19-144">Response</span></span>

<span data-ttu-id="e9e19-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9e19-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9e19-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9e19-147">Example</span></span>
<span data-ttu-id="e9e19-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e9e19-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e9e19-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9e19-149">Request</span></span>
<span data-ttu-id="e9e19-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9e19-150">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/forward
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


##### <a name="response"></a><span data-ttu-id="e9e19-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9e19-151">Response</span></span>
<span data-ttu-id="e9e19-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9e19-152">Here is an example of the response.</span></span>
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
