---
title: 'evento: dismissReminder'
description: Descarte um lembrete que tiver sido disparado para um evento em um calendário do usuário.
ms.openlocfilehash: d3ac1d09eb52991d9fcdc6c2f499d1415ac11141
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006669"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="c7c9b-103">evento: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="c7c9b-103">event: dismissReminder</span></span>

<span data-ttu-id="c7c9b-104">Descarte um lembrete que tiver sido disparado para um [evento](../resources/event.md) em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7c9b-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="c7c9b-105">Permissions</span></span>
<span data-ttu-id="c7c9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7c9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c9b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7c9b-108">Permission type</span></span>      | <span data-ttu-id="c7c9b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7c9b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7c9b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7c9b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c7c9b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7c9b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c7c9b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7c9b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7c9b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7c9b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c7c9b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7c9b-114">Application</span></span> | <span data-ttu-id="c7c9b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7c9b-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7c9b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7c9b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="c7c9b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7c9b-117">Request headers</span></span>
| <span data-ttu-id="c7c9b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c7c9b-118">Name</span></span>       | <span data-ttu-id="c7c9b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7c9b-119">Type</span></span> | <span data-ttu-id="c7c9b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7c9b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c7c9b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7c9b-121">Authorization</span></span>  | <span data-ttu-id="c7c9b-122">string</span><span class="sxs-lookup"><span data-stu-id="c7c9b-122">string</span></span>  | <span data-ttu-id="c7c9b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="c7c9b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7c9b-125">Response</span></span>

<span data-ttu-id="c7c9b-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7c9b-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7c9b-128">Example</span></span>

<span data-ttu-id="c7c9b-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c7c9b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7c9b-130">Request</span></span>
<span data-ttu-id="c7c9b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

<br/>

### <a name="response"></a><span data-ttu-id="c7c9b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7c9b-132">Response</span></span>
<span data-ttu-id="c7c9b-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
