---
title: 'evento: encaminhar'
description: 'Essa ação permite que o organizador ou o participante de um evento de reunião para encaminhar o '
ms.openlocfilehash: 09a98f82e72eef7b223dfccb1f4433c3206f0f7f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033017"
---
# <a name="event-forward"></a><span data-ttu-id="ae512-103">evento: encaminhar</span><span class="sxs-lookup"><span data-stu-id="ae512-103">event: forward</span></span>

> <span data-ttu-id="ae512-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ae512-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae512-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ae512-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae512-106">Essa ação permite que o organizador ou o participante de uma reunião de [evento](../resources/event.md) para encaminhar a solicitação de reunião para um novo destinatário.</span><span class="sxs-lookup"><span data-stu-id="ae512-106">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="ae512-107">Se o evento de reunião é encaminhado de caixa de correio do de um participante Office 365 para outro destinatário, essa ação também envia uma mensagem para notificar o organizador do encaminhamento e adiciona o destinatário para a cópia do organizador do evento reunião.</span><span class="sxs-lookup"><span data-stu-id="ae512-107">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="ae512-108">Essa conveniência não está disponível no encaminhamento de uma conta do Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="ae512-108">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="ae512-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="ae512-109">Permissions</span></span>
<span data-ttu-id="ae512-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae512-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae512-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae512-112">Permission type</span></span>      | <span data-ttu-id="ae512-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae512-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae512-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae512-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ae512-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ae512-115">Calendars.Read</span></span>    |
|<span data-ttu-id="ae512-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae512-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae512-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ae512-117">Calendars.Read</span></span>    |
|<span data-ttu-id="ae512-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae512-118">Application</span></span> | <span data-ttu-id="ae512-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ae512-119">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae512-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae512-120">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="ae512-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae512-121">Request headers</span></span>
| <span data-ttu-id="ae512-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ae512-122">Name</span></span>       | <span data-ttu-id="ae512-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae512-123">Type</span></span> | <span data-ttu-id="ae512-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae512-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ae512-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae512-125">Authorization</span></span>  | <span data-ttu-id="ae512-126">string</span><span class="sxs-lookup"><span data-stu-id="ae512-126">string</span></span>  | <span data-ttu-id="ae512-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae512-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae512-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae512-129">Content-Type</span></span> | <span data-ttu-id="ae512-130">string</span><span class="sxs-lookup"><span data-stu-id="ae512-130">string</span></span>  | <span data-ttu-id="ae512-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae512-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae512-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae512-133">Request body</span></span>
<span data-ttu-id="ae512-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae512-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ae512-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ae512-135">Parameter</span></span>    | <span data-ttu-id="ae512-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae512-136">Type</span></span>   |<span data-ttu-id="ae512-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae512-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae512-138">Comentário</span><span class="sxs-lookup"><span data-stu-id="ae512-138">Comment</span></span>|<span data-ttu-id="ae512-139">String</span><span class="sxs-lookup"><span data-stu-id="ae512-139">String</span></span>|<span data-ttu-id="ae512-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="ae512-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="ae512-142">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="ae512-142">ToRecipients</span></span>|<span data-ttu-id="ae512-143">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="ae512-143">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="ae512-144">A lista de destinatários para os quais o evento será encaminhado.</span><span class="sxs-lookup"><span data-stu-id="ae512-144">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="ae512-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae512-145">Response</span></span>

<span data-ttu-id="ae512-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae512-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae512-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae512-148">Example</span></span>
<span data-ttu-id="ae512-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ae512-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ae512-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae512-150">Request</span></span>
<span data-ttu-id="ae512-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae512-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ae512-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae512-152">Response</span></span>
<span data-ttu-id="ae512-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae512-153">Here is an example of the response.</span></span>
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
  "description": "event: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
