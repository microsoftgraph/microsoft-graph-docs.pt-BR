---
title: Excluir evento
description: Exclua um evento.
author: angelgolfer-ms
ms.openlocfilehash: 7f5880c20c6e9f31259910def9529c387c25abe0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350077"
---
# <a name="delete-event"></a><span data-ttu-id="e2229-103">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="e2229-103">Delete event</span></span>

<span data-ttu-id="e2229-104">Exclua um evento.</span><span class="sxs-lookup"><span data-stu-id="e2229-104">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2229-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2229-105">Permissions</span></span>
<span data-ttu-id="e2229-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2229-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2229-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2229-108">Permission type</span></span>      | <span data-ttu-id="e2229-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2229-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2229-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2229-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2229-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2229-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e2229-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2229-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2229-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2229-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e2229-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2229-114">Application</span></span> | <span data-ttu-id="e2229-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2229-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2229-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2229-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e2229-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2229-117">Request headers</span></span>
| <span data-ttu-id="e2229-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e2229-118">Name</span></span>       | <span data-ttu-id="e2229-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2229-119">Type</span></span> | <span data-ttu-id="e2229-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2229-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2229-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2229-121">Authorization</span></span>  | <span data-ttu-id="e2229-122">string</span><span class="sxs-lookup"><span data-stu-id="e2229-122">string</span></span>  | <span data-ttu-id="e2229-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2229-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2229-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2229-125">Request body</span></span>
<span data-ttu-id="e2229-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e2229-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2229-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2229-127">Response</span></span>

<span data-ttu-id="e2229-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2229-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2229-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2229-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2229-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2229-131">Request</span></span>
<span data-ttu-id="e2229-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2229-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="e2229-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2229-133">Response</span></span>
<span data-ttu-id="e2229-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2229-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
