---
title: Excluir calendarPermission
description: Exclua calendarPermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 53e6c0cdf4edd1ad492f190bab488ba63d967219
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227764"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="4ffc9-103">Excluir calendarPermission</span><span class="sxs-lookup"><span data-stu-id="4ffc9-103">Delete calendarPermission</span></span>

<span data-ttu-id="4ffc9-104">Exclua calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="4ffc9-104">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ffc9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ffc9-105">Permissions</span></span>

<span data-ttu-id="4ffc9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ffc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ffc9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ffc9-108">Permission type</span></span>      | <span data-ttu-id="4ffc9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ffc9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ffc9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ffc9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4ffc9-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ffc9-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4ffc9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ffc9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ffc9-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ffc9-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4ffc9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ffc9-114">Application</span></span> | <span data-ttu-id="4ffc9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ffc9-115">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="4ffc9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ffc9-116">HTTP request</span></span>

<span data-ttu-id="4ffc9-117">Excluir as permissões especificadas do calendário principal de um usuário:</span><span class="sxs-lookup"><span data-stu-id="4ffc9-117">Delete the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="4ffc9-118">Excluir as permissões especificadas de um calendário de Grupo:</span><span class="sxs-lookup"><span data-stu-id="4ffc9-118">Delete the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="4ffc9-119">Exclua as permissões especificadas do calendário do usuário que contém o evento identificado:</span><span class="sxs-lookup"><span data-stu-id="4ffc9-119">Delete the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4ffc9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ffc9-120">Request headers</span></span>

| <span data-ttu-id="4ffc9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4ffc9-121">Name</span></span>          | <span data-ttu-id="4ffc9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ffc9-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4ffc9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ffc9-123">Authorization</span></span> | <span data-ttu-id="4ffc9-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="4ffc9-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ffc9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ffc9-125">Request body</span></span>

<span data-ttu-id="4ffc9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ffc9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ffc9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ffc9-127">Response</span></span>

<span data-ttu-id="4ffc9-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ffc9-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ffc9-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4ffc9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ffc9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ffc9-131">Request</span></span>

<span data-ttu-id="4ffc9-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ffc9-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/{id}
```

### <a name="response"></a><span data-ttu-id="4ffc9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ffc9-133">Response</span></span>

<span data-ttu-id="4ffc9-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4ffc9-134">The following is an example of the response.</span></span>

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
