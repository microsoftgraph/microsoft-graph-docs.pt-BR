---
title: Excluir calendarPermission
description: Exclua calendarPermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: def57ef9dab0f4c1666ebd9b411d9e05c7a75858
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936808"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="6a68c-103">Excluir calendarPermission</span><span class="sxs-lookup"><span data-stu-id="6a68c-103">Delete calendarPermission</span></span>

<span data-ttu-id="6a68c-104">Exclua calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="6a68c-104">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a68c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a68c-105">Permissions</span></span>

<span data-ttu-id="6a68c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a68c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a68c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a68c-108">Permission type</span></span>      | <span data-ttu-id="6a68c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a68c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a68c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a68c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6a68c-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a68c-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6a68c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a68c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a68c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a68c-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6a68c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a68c-114">Application</span></span> | <span data-ttu-id="6a68c-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a68c-115">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="6a68c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a68c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
DELETE /groups/{id}/calendar/calendarPermissions/{id}
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6a68c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a68c-117">Request headers</span></span>

| <span data-ttu-id="6a68c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6a68c-118">Name</span></span>          | <span data-ttu-id="6a68c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a68c-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6a68c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a68c-120">Authorization</span></span> | <span data-ttu-id="6a68c-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="6a68c-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a68c-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a68c-122">Request body</span></span>

<span data-ttu-id="6a68c-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a68c-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a68c-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a68c-124">Response</span></span>

<span data-ttu-id="6a68c-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a68c-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a68c-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6a68c-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a68c-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a68c-128">Request</span></span>

<span data-ttu-id="6a68c-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a68c-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```

### <a name="response"></a><span data-ttu-id="6a68c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a68c-130">Response</span></span>

<span data-ttu-id="6a68c-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a68c-131">The following is an example of the response.</span></span>

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