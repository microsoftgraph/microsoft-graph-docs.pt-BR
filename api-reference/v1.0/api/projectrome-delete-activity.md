---
title: Excluir uma atividade
description: Exclua uma atividade de usuário existente para seu aplicativo.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: apiPageType
ms.openlocfilehash: 860400939228b913c5c7a8a134827e2a02d893c2
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401579"
---
# <a name="delete-an-activity"></a><span data-ttu-id="6b671-103">Excluir uma atividade</span><span class="sxs-lookup"><span data-stu-id="6b671-103">Delete an activity</span></span>

<span data-ttu-id="6b671-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b671-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b671-105">Exclua uma atividade de usuário existente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6b671-105">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b671-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b671-106">Permissions</span></span>

<span data-ttu-id="6b671-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b671-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6b671-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b671-109">Permission type</span></span>      | <span data-ttu-id="6b671-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b671-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b671-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b671-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b671-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="6b671-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="6b671-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b671-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b671-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="6b671-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="6b671-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b671-115">Application</span></span> | <span data-ttu-id="6b671-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b671-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b671-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b671-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6b671-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b671-118">Request headers</span></span>

|<span data-ttu-id="6b671-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6b671-119">Name</span></span> | <span data-ttu-id="6b671-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b671-120">Type</span></span> | <span data-ttu-id="6b671-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b671-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="6b671-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b671-122">Authorization</span></span> | <span data-ttu-id="6b671-123">string</span><span class="sxs-lookup"><span data-stu-id="6b671-123">string</span></span> | <span data-ttu-id="6b671-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b671-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b671-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b671-126">Request body</span></span>

<span data-ttu-id="6b671-127">Nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b671-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="6b671-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b671-128">Response</span></span>

<span data-ttu-id="6b671-129">Se tiver êxito, este método retornará `204 No Content` o código de resposta se a atividade tiver sido excluída.</span><span class="sxs-lookup"><span data-stu-id="6b671-129">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="6b671-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b671-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b671-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b671-131">Request</span></span>

<span data-ttu-id="6b671-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b671-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6b671-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b671-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```
# <a name="c"></a>[<span data-ttu-id="6b671-134">C#</span><span class="sxs-lookup"><span data-stu-id="6b671-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b671-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b671-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b671-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b671-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b671-137">Java</span><span class="sxs-lookup"><span data-stu-id="6b671-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6b671-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b671-138">Response</span></span>

<span data-ttu-id="6b671-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6b671-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

