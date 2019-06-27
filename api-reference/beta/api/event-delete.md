---
title: Excluir evento
description: Exclua um evento.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 82bcfd5b8db1932f855fd399159824f0d3cf89c8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259168"
---
# <a name="delete-event"></a><span data-ttu-id="8aecf-103">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="8aecf-103">Delete event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aecf-104">Exclua um evento.</span><span class="sxs-lookup"><span data-stu-id="8aecf-104">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="8aecf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8aecf-105">Permissions</span></span>
<span data-ttu-id="8aecf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aecf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aecf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8aecf-108">Permission type</span></span>      | <span data-ttu-id="8aecf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8aecf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8aecf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8aecf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8aecf-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8aecf-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8aecf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8aecf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8aecf-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8aecf-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8aecf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8aecf-114">Application</span></span> | <span data-ttu-id="8aecf-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8aecf-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8aecf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8aecf-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="8aecf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8aecf-117">Request headers</span></span>
| <span data-ttu-id="8aecf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8aecf-118">Name</span></span>       | <span data-ttu-id="8aecf-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8aecf-119">Type</span></span> | <span data-ttu-id="8aecf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aecf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8aecf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8aecf-121">Authorization</span></span>  | <span data-ttu-id="8aecf-122">string</span><span class="sxs-lookup"><span data-stu-id="8aecf-122">string</span></span>  | <span data-ttu-id="8aecf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8aecf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8aecf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8aecf-125">Request body</span></span>
<span data-ttu-id="8aecf-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8aecf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8aecf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aecf-127">Response</span></span>

<span data-ttu-id="8aecf-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8aecf-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8aecf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8aecf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8aecf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8aecf-131">Request</span></span>
<span data-ttu-id="8aecf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8aecf-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="8aecf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aecf-133">Response</span></span>
<span data-ttu-id="8aecf-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8aecf-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8aecf-135">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="8aecf-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8aecf-136">C#</span><span class="sxs-lookup"><span data-stu-id="8aecf-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8aecf-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="8aecf-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_event-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8aecf-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8aecf-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_event-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/event-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
