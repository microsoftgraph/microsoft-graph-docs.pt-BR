---
title: Excluir um historyItem
description: Excluir um item de histórico existente para uma atividade existente do usuário.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: apiPageType
ms.openlocfilehash: 084431ed1ad5ef6ff30986afe7a14037bbb4b5f5
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810287"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="63884-103">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="63884-103">Delete a historyItem</span></span>

<span data-ttu-id="63884-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63884-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63884-105">Excluir um item de histórico existente para uma atividade existente do usuário.</span><span class="sxs-lookup"><span data-stu-id="63884-105">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="63884-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="63884-106">Permissions</span></span>

<span data-ttu-id="63884-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63884-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="63884-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63884-109">Permission type</span></span>      | <span data-ttu-id="63884-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63884-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63884-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63884-111">Delegated (work or school account)</span></span> | <span data-ttu-id="63884-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="63884-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="63884-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63884-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63884-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="63884-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="63884-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63884-115">Application</span></span> | <span data-ttu-id="63884-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63884-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63884-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63884-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="63884-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63884-118">Request headers</span></span>

|<span data-ttu-id="63884-119">Nome</span><span class="sxs-lookup"><span data-stu-id="63884-119">Name</span></span> | <span data-ttu-id="63884-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="63884-120">Type</span></span> | <span data-ttu-id="63884-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="63884-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="63884-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63884-122">Authorization</span></span> | <span data-ttu-id="63884-123">string</span><span class="sxs-lookup"><span data-stu-id="63884-123">string</span></span> | <span data-ttu-id="63884-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63884-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63884-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63884-126">Request body</span></span>

<span data-ttu-id="63884-127">Nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="63884-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="63884-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="63884-128">Response</span></span>

<span data-ttu-id="63884-129">Se tiver êxito, este método retornará o `204 No Content` código de resposta se o item do histórico tiver sido excluído.</span><span class="sxs-lookup"><span data-stu-id="63884-129">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="63884-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63884-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="63884-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63884-131">Request</span></span>

<span data-ttu-id="63884-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63884-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="63884-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="63884-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```
# <a name="objective-c"></a>[<span data-ttu-id="63884-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63884-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="63884-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="63884-135">Response</span></span>

<span data-ttu-id="63884-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63884-136">Here is an example of the response.</span></span>

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
