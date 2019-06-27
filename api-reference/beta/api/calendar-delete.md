---
title: Excluir calendário
description: Exclua um calendário que não o calendário padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9325308eb348c92a6352da3205c4bed230b02455
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262430"
---
# <a name="delete-calendar"></a><span data-ttu-id="4cf1f-103">Excluir calendário</span><span class="sxs-lookup"><span data-stu-id="4cf1f-103">Delete calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cf1f-104">Exclua um calendário que não o calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="4cf1f-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="4cf1f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4cf1f-105">Permissions</span></span>
<span data-ttu-id="4cf1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cf1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cf1f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4cf1f-108">Permission type</span></span>      | <span data-ttu-id="4cf1f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4cf1f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cf1f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4cf1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4cf1f-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cf1f-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4cf1f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4cf1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cf1f-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cf1f-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4cf1f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4cf1f-114">Application</span></span> | <span data-ttu-id="4cf1f-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cf1f-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cf1f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4cf1f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="4cf1f-117">Um [calendar](../resources/calendar.md) de usuário, que não seja o padrão, no [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="4cf1f-117">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="4cf1f-118">Um [calendar](../resources/calendar.md), que não seja o padrão, em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="4cf1f-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4cf1f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4cf1f-119">Request headers</span></span>
| <span data-ttu-id="4cf1f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4cf1f-120">Name</span></span>           |  <span data-ttu-id="4cf1f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cf1f-121">Type</span></span>    | <span data-ttu-id="4cf1f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cf1f-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="4cf1f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4cf1f-123">Authorization</span></span>  |  <span data-ttu-id="4cf1f-124">string</span><span class="sxs-lookup"><span data-stu-id="4cf1f-124">string</span></span>  | <span data-ttu-id="4cf1f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4cf1f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4cf1f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4cf1f-127">Request body</span></span>
<span data-ttu-id="4cf1f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4cf1f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cf1f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cf1f-129">Response</span></span>

<span data-ttu-id="4cf1f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4cf1f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cf1f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4cf1f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cf1f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cf1f-133">Request</span></span>
<span data-ttu-id="4cf1f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cf1f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
##### <a name="response"></a><span data-ttu-id="4cf1f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cf1f-135">Response</span></span>
<span data-ttu-id="4cf1f-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4cf1f-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4cf1f-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4cf1f-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4cf1f-138">C#</span><span class="sxs-lookup"><span data-stu-id="4cf1f-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_calendar-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4cf1f-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="4cf1f-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_calendar-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4cf1f-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4cf1f-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_calendar-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/calendar-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/calendar-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
