---
title: Excluir uma atividade
description: Excluir uma atividade de usuário existente para seu aplicativo.
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ''
ms.openlocfilehash: e2e5b23ca9786af7e08a4cf0281ec519274b09a7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342212"
---
# <a name="delete-an-activity"></a><span data-ttu-id="8ad09-103">Excluir uma atividade</span><span class="sxs-lookup"><span data-stu-id="8ad09-103">Delete an activity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ad09-104">Excluir uma atividade de usuário existente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8ad09-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ad09-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ad09-105">Permissions</span></span>

<span data-ttu-id="8ad09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ad09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8ad09-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ad09-108">Permission type</span></span>      | <span data-ttu-id="8ad09-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ad09-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ad09-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ad09-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ad09-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="8ad09-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="8ad09-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ad09-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ad09-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="8ad09-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="8ad09-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ad09-114">Application</span></span> | <span data-ttu-id="8ad09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ad09-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ad09-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ad09-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8ad09-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ad09-117">Request headers</span></span>

|<span data-ttu-id="8ad09-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8ad09-118">Name</span></span> | <span data-ttu-id="8ad09-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ad09-119">Type</span></span> | <span data-ttu-id="8ad09-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ad09-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="8ad09-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ad09-121">Authorization</span></span> | <span data-ttu-id="8ad09-122">string</span><span class="sxs-lookup"><span data-stu-id="8ad09-122">string</span></span> | <span data-ttu-id="8ad09-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ad09-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ad09-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ad09-125">Request body</span></span>

<span data-ttu-id="8ad09-126">Nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ad09-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="8ad09-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ad09-127">Response</span></span>

<span data-ttu-id="8ad09-128">Se tiver êxito, este método retornará `204 No Content` o código de resposta se a atividade tiver sido excluída.</span><span class="sxs-lookup"><span data-stu-id="8ad09-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="8ad09-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ad09-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8ad09-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ad09-130">Request</span></span>

<span data-ttu-id="8ad09-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ad09-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8ad09-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ad09-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ad09-133">C#</span><span class="sxs-lookup"><span data-stu-id="8ad09-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ad09-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ad09-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ad09-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8ad09-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8ad09-136">Java</span><span class="sxs-lookup"><span data-stu-id="8ad09-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8ad09-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ad09-137">Response</span></span>

<span data-ttu-id="8ad09-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ad09-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
