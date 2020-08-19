---
title: Excluir uma atividade
description: Excluir uma atividade de usuário existente para seu aplicativo.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: apiPageType
ms.openlocfilehash: 1ab0d5510ca8cb1a3a7376259904af22f1561014
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807042"
---
# <a name="delete-an-activity"></a><span data-ttu-id="0f056-103">Excluir uma atividade</span><span class="sxs-lookup"><span data-stu-id="0f056-103">Delete an activity</span></span>

<span data-ttu-id="0f056-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f056-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f056-105">Excluir uma atividade de usuário existente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f056-105">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f056-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f056-106">Permissions</span></span>

<span data-ttu-id="0f056-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f056-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0f056-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f056-109">Permission type</span></span>      | <span data-ttu-id="0f056-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f056-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f056-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f056-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0f056-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="0f056-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="0f056-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f056-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f056-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="0f056-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="0f056-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f056-115">Application</span></span> | <span data-ttu-id="0f056-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f056-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f056-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f056-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0f056-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f056-118">Request headers</span></span>

|<span data-ttu-id="0f056-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0f056-119">Name</span></span> | <span data-ttu-id="0f056-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f056-120">Type</span></span> | <span data-ttu-id="0f056-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f056-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="0f056-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f056-122">Authorization</span></span> | <span data-ttu-id="0f056-123">string</span><span class="sxs-lookup"><span data-stu-id="0f056-123">string</span></span> | <span data-ttu-id="0f056-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f056-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f056-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f056-126">Request body</span></span>

<span data-ttu-id="0f056-127">Nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f056-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="0f056-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f056-128">Response</span></span>

<span data-ttu-id="0f056-129">Se tiver êxito, este método retornará o `204 No Content` código de resposta se a atividade tiver sido excluída.</span><span class="sxs-lookup"><span data-stu-id="0f056-129">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="0f056-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f056-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0f056-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f056-131">Request</span></span>

<span data-ttu-id="0f056-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f056-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0f056-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f056-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```
# <a name="c"></a>[<span data-ttu-id="0f056-134">C#</span><span class="sxs-lookup"><span data-stu-id="0f056-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f056-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f056-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f056-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f056-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f056-137">Java</span><span class="sxs-lookup"><span data-stu-id="0f056-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0f056-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f056-138">Response</span></span>

<span data-ttu-id="0f056-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f056-139">Here is an example of the response.</span></span>

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
