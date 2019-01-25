---
title: 'evento: encaminhar'
description: 'Essa ação permite que o organizador ou o participante de um evento de reunião para encaminhar o '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6f1b3e1f089d927aeb21ca80ff77edda63121c60
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510383"
---
# <a name="event-forward"></a><span data-ttu-id="49f21-103">evento: encaminhar</span><span class="sxs-lookup"><span data-stu-id="49f21-103">event: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49f21-104">Esta ação permite que o organizador ou o participante de um evento de reunião encaminhe a solicitação de reunião ao novo destinatário.</span><span class="sxs-lookup"><span data-stu-id="49f21-104">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="49f21-105">Se o evento de reunião é encaminhado de caixa de correio do de um participante Office 365 para outro destinatário, essa ação também envia uma mensagem para notificar o organizador do encaminhamento e adiciona o destinatário para a cópia do organizador do evento reunião.</span><span class="sxs-lookup"><span data-stu-id="49f21-105">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="49f21-106">Essa conveniência não está disponível no encaminhamento de uma conta do Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="49f21-106">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="49f21-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="49f21-107">Permissions</span></span>
<span data-ttu-id="49f21-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49f21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49f21-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49f21-110">Permission type</span></span>      | <span data-ttu-id="49f21-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49f21-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49f21-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49f21-112">Delegated (work or school account)</span></span> | <span data-ttu-id="49f21-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="49f21-113">Calendars.Read</span></span>    |
|<span data-ttu-id="49f21-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49f21-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49f21-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="49f21-115">Calendars.Read</span></span>    |
|<span data-ttu-id="49f21-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49f21-116">Application</span></span> | <span data-ttu-id="49f21-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="49f21-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="49f21-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49f21-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="49f21-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49f21-119">Request headers</span></span>
| <span data-ttu-id="49f21-120">Nome</span><span class="sxs-lookup"><span data-stu-id="49f21-120">Name</span></span>       | <span data-ttu-id="49f21-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="49f21-121">Type</span></span> | <span data-ttu-id="49f21-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="49f21-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="49f21-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="49f21-123">Authorization</span></span>  | <span data-ttu-id="49f21-124">string</span><span class="sxs-lookup"><span data-stu-id="49f21-124">string</span></span>  | <span data-ttu-id="49f21-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49f21-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49f21-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49f21-127">Content-Type</span></span> | <span data-ttu-id="49f21-128">string</span><span class="sxs-lookup"><span data-stu-id="49f21-128">string</span></span>  | <span data-ttu-id="49f21-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49f21-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49f21-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49f21-131">Request body</span></span>
<span data-ttu-id="49f21-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49f21-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49f21-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="49f21-133">Parameter</span></span>    | <span data-ttu-id="49f21-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="49f21-134">Type</span></span>   |<span data-ttu-id="49f21-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="49f21-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49f21-136">Comentário</span><span class="sxs-lookup"><span data-stu-id="49f21-136">Comment</span></span>|<span data-ttu-id="49f21-137">String</span><span class="sxs-lookup"><span data-stu-id="49f21-137">String</span></span>|<span data-ttu-id="49f21-p105">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="49f21-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="49f21-140">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="49f21-140">ToRecipients</span></span>|<span data-ttu-id="49f21-141">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="49f21-141">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="49f21-142">A lista de destinatários para os quais o evento será encaminhado.</span><span class="sxs-lookup"><span data-stu-id="49f21-142">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="49f21-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="49f21-143">Response</span></span>

<span data-ttu-id="49f21-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49f21-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49f21-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49f21-146">Example</span></span>
<span data-ttu-id="49f21-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="49f21-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="49f21-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49f21-148">Request</span></span>
<span data-ttu-id="49f21-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49f21-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="49f21-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="49f21-150">Response</span></span>
<span data-ttu-id="49f21-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49f21-151">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/event-forward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
