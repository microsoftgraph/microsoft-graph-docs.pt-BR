---
title: Excluir calendário
description: Exclua um calendário que não o calendário padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af1fe9a0b13aeb20a269b39bac8966bcc31508b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937415"
---
# <a name="delete-calendar"></a><span data-ttu-id="61a29-103">Excluir calendário</span><span class="sxs-lookup"><span data-stu-id="61a29-103">Delete calendar</span></span>

<span data-ttu-id="61a29-104">Exclua um calendário que não o calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="61a29-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="61a29-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="61a29-105">Permissions</span></span>
<span data-ttu-id="61a29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61a29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61a29-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61a29-108">Permission type</span></span>      | <span data-ttu-id="61a29-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61a29-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61a29-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61a29-110">Delegated (work or school account)</span></span> | <span data-ttu-id="61a29-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61a29-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="61a29-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61a29-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61a29-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61a29-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="61a29-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61a29-114">Application</span></span> | <span data-ttu-id="61a29-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61a29-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="61a29-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61a29-116">HTTP request</span></span>
<span data-ttu-id="61a29-117"><!-- { "blockType": "ignored" } -->De um usuário [calendário](../resources/calendar.md) que não seja o calendário padrão em que o padrão [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="61a29-117"><!-- { "blockType": "ignored" } --> A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="61a29-118">Um [calendar](../resources/calendar.md), que não seja o padrão, em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="61a29-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="61a29-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61a29-119">Request headers</span></span>
| <span data-ttu-id="61a29-120">Nome</span><span class="sxs-lookup"><span data-stu-id="61a29-120">Name</span></span>           |  <span data-ttu-id="61a29-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="61a29-121">Type</span></span>    | <span data-ttu-id="61a29-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="61a29-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="61a29-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="61a29-123">Authorization</span></span>  |  <span data-ttu-id="61a29-124">string</span><span class="sxs-lookup"><span data-stu-id="61a29-124">string</span></span>  | <span data-ttu-id="61a29-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61a29-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61a29-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61a29-127">Request body</span></span>
<span data-ttu-id="61a29-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61a29-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61a29-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="61a29-129">Response</span></span>

<span data-ttu-id="61a29-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61a29-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61a29-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61a29-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61a29-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61a29-133">Request</span></span>
<span data-ttu-id="61a29-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61a29-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="61a29-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="61a29-135">Response</span></span>
<span data-ttu-id="61a29-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61a29-136">Here is an example of the response.</span></span> 
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
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
