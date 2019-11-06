---
title: Excluir calendarPermission
description: Exclua calendarPermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e9d0483fd37f9b81b1808c1e2c33557fc2a17679
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994887"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="696fa-103">Excluir calendarPermission</span><span class="sxs-lookup"><span data-stu-id="696fa-103">Delete calendarPermission</span></span>

<span data-ttu-id="696fa-104">Exclua calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="696fa-104">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="696fa-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="696fa-105">Permissions</span></span>

<span data-ttu-id="696fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="696fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="696fa-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="696fa-108">Permission type</span></span>      | <span data-ttu-id="696fa-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="696fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="696fa-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="696fa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="696fa-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="696fa-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="696fa-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="696fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="696fa-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="696fa-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="696fa-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="696fa-114">Application</span></span> | <span data-ttu-id="696fa-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="696fa-115">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="696fa-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="696fa-116">HTTP request</span></span>

<span data-ttu-id="696fa-117">Excluir as permissões especificadas do calendário principal de um usuário:</span><span class="sxs-lookup"><span data-stu-id="696fa-117">Delete the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="696fa-118">Excluir as permissões especificadas de um calendário de Grupo:</span><span class="sxs-lookup"><span data-stu-id="696fa-118">Delete the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="696fa-119">Exclua as permissões especificadas do calendário do usuário que contém o evento identificado:</span><span class="sxs-lookup"><span data-stu-id="696fa-119">Delete the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="696fa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="696fa-120">Request headers</span></span>

| <span data-ttu-id="696fa-121">Nome</span><span class="sxs-lookup"><span data-stu-id="696fa-121">Name</span></span>          | <span data-ttu-id="696fa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="696fa-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="696fa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="696fa-123">Authorization</span></span> | <span data-ttu-id="696fa-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="696fa-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="696fa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="696fa-125">Request body</span></span>

<span data-ttu-id="696fa-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="696fa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="696fa-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="696fa-127">Response</span></span>

<span data-ttu-id="696fa-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="696fa-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="696fa-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="696fa-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="696fa-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="696fa-131">Request</span></span>

<span data-ttu-id="696fa-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="696fa-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="696fa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="696fa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="696fa-134">C#</span><span class="sxs-lookup"><span data-stu-id="696fa-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="696fa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="696fa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="696fa-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="696fa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="696fa-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="696fa-137">Response</span></span>

<span data-ttu-id="696fa-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="696fa-138">The following is an example of the response.</span></span>

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
