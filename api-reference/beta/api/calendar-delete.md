---
title: Excluir calendário
description: Exclua um calendário que não o calendário padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 4621314f179ddc1eac47b5f178ff50af670972db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809489"
---
# <a name="delete-calendar"></a><span data-ttu-id="c64df-103">Excluir calendário</span><span class="sxs-lookup"><span data-stu-id="c64df-103">Delete calendar</span></span>

> <span data-ttu-id="c64df-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c64df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c64df-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c64df-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c64df-106">Exclua um calendário que não o calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="c64df-106">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="c64df-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c64df-107">Permissions</span></span>
<span data-ttu-id="c64df-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c64df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c64df-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c64df-110">Permission type</span></span>      | <span data-ttu-id="c64df-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c64df-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c64df-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c64df-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c64df-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c64df-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c64df-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c64df-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c64df-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c64df-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c64df-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c64df-116">Application</span></span> | <span data-ttu-id="c64df-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c64df-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c64df-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c64df-118">HTTP request</span></span>
<span data-ttu-id="c64df-119"><!-- { "blockType": "ignored" } -->De um usuário [calendário](../resources/calendar.md) que não seja o calendário padrão em que o padrão [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="c64df-119"><!-- { "blockType": "ignored" } --> A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="c64df-120">Um [calendar](../resources/calendar.md), que não seja o padrão, em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="c64df-120">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c64df-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c64df-121">Request headers</span></span>
| <span data-ttu-id="c64df-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c64df-122">Name</span></span>           |  <span data-ttu-id="c64df-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c64df-123">Type</span></span>    | <span data-ttu-id="c64df-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c64df-124">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="c64df-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c64df-125">Authorization</span></span>  |  <span data-ttu-id="c64df-126">string</span><span class="sxs-lookup"><span data-stu-id="c64df-126">string</span></span>  | <span data-ttu-id="c64df-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c64df-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c64df-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c64df-129">Request body</span></span>
<span data-ttu-id="c64df-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c64df-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c64df-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c64df-131">Response</span></span>

<span data-ttu-id="c64df-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c64df-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c64df-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c64df-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c64df-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c64df-135">Request</span></span>
<span data-ttu-id="c64df-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c64df-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
##### <a name="response"></a><span data-ttu-id="c64df-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c64df-137">Response</span></span>
<span data-ttu-id="c64df-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c64df-138">Here is an example of the response.</span></span> 
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
