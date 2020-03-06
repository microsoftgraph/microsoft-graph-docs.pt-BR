---
title: Excluir um historyItem
description: Excluir um item de histórico existente para uma atividade existente do usuário.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: apiPageType
ms.openlocfilehash: fc6ed6a6a2f01667c32b9f2497a93e05e0f275ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510736"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="dc8cd-103">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="dc8cd-103">Delete a historyItem</span></span>

<span data-ttu-id="dc8cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc8cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dc8cd-105">Excluir um item de histórico existente para uma atividade existente do usuário.</span><span class="sxs-lookup"><span data-stu-id="dc8cd-105">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc8cd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc8cd-106">Permissions</span></span>

<span data-ttu-id="dc8cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc8cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dc8cd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc8cd-109">Permission type</span></span>      | <span data-ttu-id="dc8cd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc8cd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc8cd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc8cd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc8cd-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="dc8cd-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="dc8cd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc8cd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc8cd-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="dc8cd-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="dc8cd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc8cd-115">Application</span></span> | <span data-ttu-id="dc8cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc8cd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc8cd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc8cd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dc8cd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc8cd-118">Request headers</span></span>

|<span data-ttu-id="dc8cd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dc8cd-119">Name</span></span> | <span data-ttu-id="dc8cd-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc8cd-120">Type</span></span> | <span data-ttu-id="dc8cd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc8cd-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="dc8cd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc8cd-122">Authorization</span></span> | <span data-ttu-id="dc8cd-123">string</span><span class="sxs-lookup"><span data-stu-id="dc8cd-123">string</span></span> | <span data-ttu-id="dc8cd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc8cd-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc8cd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc8cd-126">Request body</span></span>

<span data-ttu-id="dc8cd-127">Nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc8cd-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="dc8cd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc8cd-128">Response</span></span>

<span data-ttu-id="dc8cd-129">Se tiver êxito, este método retornará `204 No Content` o código de resposta se o item do histórico tiver sido excluído.</span><span class="sxs-lookup"><span data-stu-id="dc8cd-129">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="dc8cd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc8cd-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dc8cd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc8cd-131">Request</span></span>

<span data-ttu-id="dc8cd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc8cd-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dc8cd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc8cd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```
# <a name="objective-c"></a>[<span data-ttu-id="dc8cd-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc8cd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dc8cd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc8cd-135">Response</span></span>

<span data-ttu-id="dc8cd-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc8cd-136">Here is an example of the response.</span></span>

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
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
