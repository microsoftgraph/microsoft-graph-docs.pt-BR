---
title: Excluir permanentemente item
description: Exclui permanentemente um item de itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 30c5cb4bc5257e4d98cbf2ee19ecfb8542a3d82e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951286"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="549f6-103">Excluir permanentemente item</span><span class="sxs-lookup"><span data-stu-id="549f6-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="549f6-104">Exclui permanentemente um item de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="549f6-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="549f6-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="549f6-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="549f6-106">É possível excluir permanentemente um item de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="549f6-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="549f6-107">Mas, uma vez que um item é excluído permanentemente, ele **não pode** ser restaurado.</span><span class="sxs-lookup"><span data-stu-id="549f6-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="549f6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="549f6-108">Permissions</span></span>
<span data-ttu-id="549f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="549f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="549f6-111">Para usuários: user. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="549f6-111">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="549f6-112">Para grupos: Group. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="549f6-112">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="549f6-113">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="549f6-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="549f6-114">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="549f6-114">Request headers</span></span>
| <span data-ttu-id="549f6-115">Nome</span><span class="sxs-lookup"><span data-stu-id="549f6-115">Name</span></span>       | <span data-ttu-id="549f6-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="549f6-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="549f6-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="549f6-117">Authorization</span></span>  | <span data-ttu-id="549f6-118">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="549f6-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="549f6-119">Aceitar</span><span class="sxs-lookup"><span data-stu-id="549f6-119">Accept</span></span>  | <span data-ttu-id="549f6-120">application/json</span><span class="sxs-lookup"><span data-stu-id="549f6-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="549f6-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="549f6-121">Request body</span></span>
<span data-ttu-id="549f6-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="549f6-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="549f6-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="549f6-123">Response</span></span>

<span data-ttu-id="549f6-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="549f6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="549f6-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="549f6-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="549f6-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="549f6-127">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="549f6-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="549f6-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="549f6-129">C#</span><span class="sxs-lookup"><span data-stu-id="549f6-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="549f6-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="549f6-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="549f6-131">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="549f6-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="549f6-132">Java</span><span class="sxs-lookup"><span data-stu-id="549f6-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="549f6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="549f6-133">Response</span></span>
<span data-ttu-id="549f6-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="549f6-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
