---
title: Excluir calendarPermission
description: Exclua calendarPermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3004f53cbe37c9f3891f350d1cb7946280ed859e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987509"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="cfc2e-103">Excluir calendarPermission</span><span class="sxs-lookup"><span data-stu-id="cfc2e-103">Delete calendarPermission</span></span>

<span data-ttu-id="cfc2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfc2e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cfc2e-105">Exclua calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="cfc2e-105">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfc2e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cfc2e-106">Permissions</span></span>

<span data-ttu-id="cfc2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfc2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfc2e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfc2e-109">Permission type</span></span>      | <span data-ttu-id="cfc2e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cfc2e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfc2e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfc2e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cfc2e-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfc2e-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cfc2e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfc2e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfc2e-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfc2e-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cfc2e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfc2e-115">Application</span></span> | <span data-ttu-id="cfc2e-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfc2e-116">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="cfc2e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfc2e-117">HTTP request</span></span>

<span data-ttu-id="cfc2e-118">Excluir as permissões especificadas do calendário principal de um usuário:</span><span class="sxs-lookup"><span data-stu-id="cfc2e-118">Delete the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="cfc2e-119">Excluir as permissões especificadas de um calendário de Grupo:</span><span class="sxs-lookup"><span data-stu-id="cfc2e-119">Delete the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="cfc2e-120">Exclua as permissões especificadas do calendário do usuário que contém o evento identificado:</span><span class="sxs-lookup"><span data-stu-id="cfc2e-120">Delete the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cfc2e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc2e-121">Request headers</span></span>

| <span data-ttu-id="cfc2e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="cfc2e-122">Name</span></span>          | <span data-ttu-id="cfc2e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfc2e-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cfc2e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfc2e-124">Authorization</span></span> | <span data-ttu-id="cfc2e-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="cfc2e-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfc2e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc2e-126">Request body</span></span>

<span data-ttu-id="cfc2e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cfc2e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfc2e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc2e-128">Response</span></span>

<span data-ttu-id="cfc2e-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc2e-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfc2e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cfc2e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cfc2e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfc2e-132">Request</span></span>

<span data-ttu-id="cfc2e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfc2e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfc2e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfc2e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="cfc2e-135">C#</span><span class="sxs-lookup"><span data-stu-id="cfc2e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfc2e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfc2e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfc2e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfc2e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cfc2e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfc2e-138">Response</span></span>

<span data-ttu-id="cfc2e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfc2e-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarPermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


