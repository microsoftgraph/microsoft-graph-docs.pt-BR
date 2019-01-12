---
title: Excluir evento
description: Exclua um evento.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 830568c5abbd02f0083cf45d5172266c2bf20e41
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956560"
---
# <a name="delete-event"></a><span data-ttu-id="6fde4-103">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="6fde4-103">Delete event</span></span>

> <span data-ttu-id="6fde4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6fde4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fde4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6fde4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6fde4-106">Exclua um evento.</span><span class="sxs-lookup"><span data-stu-id="6fde4-106">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="6fde4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6fde4-107">Permissions</span></span>
<span data-ttu-id="6fde4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fde4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fde4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fde4-110">Permission type</span></span>      | <span data-ttu-id="6fde4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fde4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fde4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fde4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6fde4-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fde4-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6fde4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fde4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fde4-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fde4-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6fde4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fde4-116">Application</span></span> | <span data-ttu-id="6fde4-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fde4-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fde4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fde4-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="6fde4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fde4-119">Request headers</span></span>
| <span data-ttu-id="6fde4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6fde4-120">Name</span></span>       | <span data-ttu-id="6fde4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fde4-121">Type</span></span> | <span data-ttu-id="6fde4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fde4-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6fde4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fde4-123">Authorization</span></span>  | <span data-ttu-id="6fde4-124">string</span><span class="sxs-lookup"><span data-stu-id="6fde4-124">string</span></span>  | <span data-ttu-id="6fde4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fde4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fde4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fde4-127">Request body</span></span>
<span data-ttu-id="6fde4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6fde4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fde4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fde4-129">Response</span></span>

<span data-ttu-id="6fde4-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fde4-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fde4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fde4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6fde4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fde4-133">Request</span></span>
<span data-ttu-id="6fde4-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fde4-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="6fde4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fde4-135">Response</span></span>
<span data-ttu-id="6fde4-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fde4-136">Here is an example of the response.</span></span> 
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
