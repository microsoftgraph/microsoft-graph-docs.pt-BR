---
title: Excluir um historyItem
description: Excluir um item de histórico existente para uma atividade existente do usuário.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 5fc0088b5e8d814e15cb6231956bd8deff266b41
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458604"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="69f43-103">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="69f43-103">Delete a historyItem</span></span>

<span data-ttu-id="69f43-104">Excluir um item de histórico existente para uma atividade existente do usuário.</span><span class="sxs-lookup"><span data-stu-id="69f43-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="69f43-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="69f43-105">Permissions</span></span>

<span data-ttu-id="69f43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69f43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="69f43-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69f43-108">Permission type</span></span>      | <span data-ttu-id="69f43-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69f43-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69f43-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69f43-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69f43-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="69f43-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="69f43-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69f43-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69f43-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="69f43-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="69f43-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69f43-114">Application</span></span> | <span data-ttu-id="69f43-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69f43-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69f43-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69f43-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="69f43-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69f43-117">Request headers</span></span>

|<span data-ttu-id="69f43-118">Nome</span><span class="sxs-lookup"><span data-stu-id="69f43-118">Name</span></span> | <span data-ttu-id="69f43-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="69f43-119">Type</span></span> | <span data-ttu-id="69f43-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="69f43-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="69f43-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="69f43-121">Authorization</span></span> | <span data-ttu-id="69f43-122">string</span><span class="sxs-lookup"><span data-stu-id="69f43-122">string</span></span> | <span data-ttu-id="69f43-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69f43-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f43-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69f43-125">Request body</span></span>

<span data-ttu-id="69f43-126">Nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="69f43-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="69f43-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="69f43-127">Response</span></span>

<span data-ttu-id="69f43-128">Se tiver êxito, este método retornará `204 No Content` o código de resposta se o item do histórico tiver sido excluído.</span><span class="sxs-lookup"><span data-stu-id="69f43-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="69f43-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69f43-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="69f43-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69f43-130">Request</span></span>

<span data-ttu-id="69f43-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69f43-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="69f43-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="69f43-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```
# <a name="objective-ctabobjc"></a>[<span data-ttu-id="69f43-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="69f43-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="69f43-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="69f43-134">Response</span></span>

<span data-ttu-id="69f43-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69f43-135">Here is an example of the response.</span></span>

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
