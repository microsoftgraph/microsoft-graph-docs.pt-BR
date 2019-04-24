---
title: Excluir calendário
description: Exclua um calendário que não o calendário padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1bdba9bb9da0ad0277ba73c4f2c28eec13072913
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461637"
---
# <a name="delete-calendar"></a><span data-ttu-id="614dc-103">Excluir calendário</span><span class="sxs-lookup"><span data-stu-id="614dc-103">Delete calendar</span></span>

<span data-ttu-id="614dc-104">Exclua um calendário que não o calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="614dc-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="614dc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="614dc-105">Permissions</span></span>
<span data-ttu-id="614dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="614dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="614dc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="614dc-108">Permission type</span></span>      | <span data-ttu-id="614dc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="614dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="614dc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="614dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="614dc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="614dc-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="614dc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="614dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="614dc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="614dc-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="614dc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="614dc-114">Application</span></span> | <span data-ttu-id="614dc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="614dc-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="614dc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="614dc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="614dc-117">Um [calendar](../resources/calendar.md) de usuário, que não seja o padrão, no [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="614dc-117">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="614dc-118">Um [calendar](../resources/calendar.md), que não seja o padrão, em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="614dc-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="614dc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="614dc-119">Request headers</span></span>
| <span data-ttu-id="614dc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="614dc-120">Name</span></span>           |  <span data-ttu-id="614dc-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="614dc-121">Type</span></span>    | <span data-ttu-id="614dc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="614dc-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="614dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="614dc-123">Authorization</span></span>  |  <span data-ttu-id="614dc-124">string</span><span class="sxs-lookup"><span data-stu-id="614dc-124">string</span></span>  | <span data-ttu-id="614dc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="614dc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="614dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="614dc-127">Request body</span></span>
<span data-ttu-id="614dc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="614dc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="614dc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="614dc-129">Response</span></span>

<span data-ttu-id="614dc-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="614dc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="614dc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="614dc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="614dc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="614dc-133">Request</span></span>
<span data-ttu-id="614dc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="614dc-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="614dc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="614dc-135">Response</span></span>
<span data-ttu-id="614dc-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="614dc-136">Here is an example of the response.</span></span> 
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
