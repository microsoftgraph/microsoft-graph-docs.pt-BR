---
title: Excluir permanentemente item
description: Exclui permanentemente um item de itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7b65c4f2667e7acdb6a6ca5240df7ab68e66f594
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455991"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="4a415-103">Excluir permanentemente item</span><span class="sxs-lookup"><span data-stu-id="4a415-103">Permanently delete item</span></span>

<span data-ttu-id="4a415-104">Exclui permanentemente um item de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="4a415-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="4a415-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="4a415-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="4a415-106">É possível excluir permanentemente um item de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="4a415-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="4a415-107">Mas, uma vez que um item é excluído permanentemente, ele **não pode** ser restaurado.</span><span class="sxs-lookup"><span data-stu-id="4a415-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a415-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a415-108">Permissions</span></span>
<span data-ttu-id="4a415-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a415-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="4a415-111">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="4a415-111">For users:</span></span>

|<span data-ttu-id="4a415-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a415-112">Permission type</span></span>      | <span data-ttu-id="4a415-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a415-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a415-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a415-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4a415-115">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a415-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="4a415-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a415-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a415-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a415-117">Not supported.</span></span> |
|<span data-ttu-id="4a415-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a415-118">Application</span></span> | <span data-ttu-id="4a415-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a415-119">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="4a415-120">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="4a415-120">For groups:</span></span>

|<span data-ttu-id="4a415-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a415-121">Permission type</span></span>      | <span data-ttu-id="4a415-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a415-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a415-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a415-123">Delegated (work or school account)</span></span> | <span data-ttu-id="4a415-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a415-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="4a415-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a415-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a415-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a415-126">Not supported.</span></span>    |
|<span data-ttu-id="4a415-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a415-127">Application</span></span> | <span data-ttu-id="4a415-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a415-128">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a415-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a415-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4a415-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a415-130">Request headers</span></span>
| <span data-ttu-id="4a415-131">Nome</span><span class="sxs-lookup"><span data-stu-id="4a415-131">Name</span></span>       | <span data-ttu-id="4a415-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a415-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4a415-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a415-133">Authorization</span></span>  | <span data-ttu-id="4a415-134">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="4a415-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="4a415-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a415-135">Accept</span></span>  | <span data-ttu-id="4a415-136">application/json</span><span class="sxs-lookup"><span data-stu-id="4a415-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a415-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a415-137">Request body</span></span>
<span data-ttu-id="4a415-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a415-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a415-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a415-139">Response</span></span>

<span data-ttu-id="4a415-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a415-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a415-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a415-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a415-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a415-143">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4a415-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a415-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a415-145">C#</span><span class="sxs-lookup"><span data-stu-id="4a415-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a415-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="4a415-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a415-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4a415-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4a415-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a415-148">Response</span></span>
<span data-ttu-id="4a415-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a415-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
