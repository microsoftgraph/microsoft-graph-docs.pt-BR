---
title: 'evento: dismissReminder'
description: Descarte um lembrete que tiver sido disparado para um evento em um calendário do usuário.
author: angelgolfer-ms
ms.openlocfilehash: 1075ee86ee174bab23bd0436c69da37f1f001d66
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357775"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="68e3e-103">evento: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="68e3e-103">event: dismissReminder</span></span>

<span data-ttu-id="68e3e-104">Descarte um lembrete que tiver sido disparado para um [evento](../resources/event.md) em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="68e3e-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="68e3e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="68e3e-105">Permissions</span></span>
<span data-ttu-id="68e3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68e3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68e3e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68e3e-108">Permission type</span></span>      | <span data-ttu-id="68e3e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68e3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68e3e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68e3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="68e3e-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68e3e-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="68e3e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68e3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68e3e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68e3e-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="68e3e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68e3e-114">Application</span></span> | <span data-ttu-id="68e3e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68e3e-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="68e3e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68e3e-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="68e3e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68e3e-117">Request headers</span></span>
| <span data-ttu-id="68e3e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="68e3e-118">Name</span></span>       | <span data-ttu-id="68e3e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="68e3e-119">Type</span></span> | <span data-ttu-id="68e3e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="68e3e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="68e3e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="68e3e-121">Authorization</span></span>  | <span data-ttu-id="68e3e-122">string</span><span class="sxs-lookup"><span data-stu-id="68e3e-122">string</span></span>  | <span data-ttu-id="68e3e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68e3e-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="68e3e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="68e3e-125">Response</span></span>

<span data-ttu-id="68e3e-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68e3e-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68e3e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68e3e-128">Example</span></span>

<span data-ttu-id="68e3e-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="68e3e-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="68e3e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68e3e-130">Request</span></span>
<span data-ttu-id="68e3e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68e3e-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

<br/>

### <a name="response"></a><span data-ttu-id="68e3e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="68e3e-132">Response</span></span>
<span data-ttu-id="68e3e-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68e3e-133">Here is an example of the response.</span></span>

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
