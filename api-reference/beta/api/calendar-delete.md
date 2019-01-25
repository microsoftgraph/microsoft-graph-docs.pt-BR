---
title: Excluir calendário
description: Exclua um calendário que não o calendário padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1bdba9bb9da0ad0277ba73c4f2c28eec13072913
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511566"
---
# <a name="delete-calendar"></a><span data-ttu-id="cb00e-103">Excluir calendário</span><span class="sxs-lookup"><span data-stu-id="cb00e-103">Delete calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb00e-104">Exclua um calendário que não o calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="cb00e-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="cb00e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb00e-105">Permissions</span></span>
<span data-ttu-id="cb00e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb00e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb00e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb00e-108">Permission type</span></span>      | <span data-ttu-id="cb00e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb00e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb00e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb00e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb00e-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb00e-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cb00e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb00e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb00e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb00e-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cb00e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb00e-114">Application</span></span> | <span data-ttu-id="cb00e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb00e-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb00e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb00e-116">HTTP request</span></span>
<span data-ttu-id="cb00e-117"><!-- { "blockType": "ignored" } -->De um usuário [calendário](../resources/calendar.md) que não seja o calendário padrão em que o padrão [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="cb00e-117"><!-- { "blockType": "ignored" } --> A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="cb00e-118">Um [calendar](../resources/calendar.md), que não seja o padrão, em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="cb00e-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cb00e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb00e-119">Request headers</span></span>
| <span data-ttu-id="cb00e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="cb00e-120">Name</span></span>           |  <span data-ttu-id="cb00e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb00e-121">Type</span></span>    | <span data-ttu-id="cb00e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb00e-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="cb00e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb00e-123">Authorization</span></span>  |  <span data-ttu-id="cb00e-124">string</span><span class="sxs-lookup"><span data-stu-id="cb00e-124">string</span></span>  | <span data-ttu-id="cb00e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb00e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb00e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb00e-127">Request body</span></span>
<span data-ttu-id="cb00e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb00e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb00e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb00e-129">Response</span></span>

<span data-ttu-id="cb00e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb00e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb00e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb00e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb00e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb00e-133">Request</span></span>
<span data-ttu-id="cb00e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb00e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
##### <a name="response"></a><span data-ttu-id="cb00e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb00e-135">Response</span></span>
<span data-ttu-id="cb00e-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb00e-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
    "Error: /api-reference/beta/api/calendar-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
