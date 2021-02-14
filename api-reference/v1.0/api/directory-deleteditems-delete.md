---
title: Excluir permanentemente um item de itens excluídos
description: Exclui permanentemente um item de itens excluídos.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da494a4cb456119e0a0e2f3ac51fa57531394331
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239097"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="737a3-103">Excluir permanentemente item</span><span class="sxs-lookup"><span data-stu-id="737a3-103">Permanently delete item</span></span>

<span data-ttu-id="737a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="737a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="737a3-105">Exclui permanentemente um item de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="737a3-105">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="737a3-106">Atualmente, a funcionalidade de itens excluídos só tem suporte para os recursos [de](../resources/application.md)aplicativo, [grupo](../resources/group.md) [e](../resources/user.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="737a3-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="737a3-107">É possível excluir permanentemente um item de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="737a3-107">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="737a3-108">Mas, uma vez que um item é excluído permanentemente, ele **não pode** ser restaurado.</span><span class="sxs-lookup"><span data-stu-id="737a3-108">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="737a3-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="737a3-109">Permissions</span></span>
<span data-ttu-id="737a3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="737a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="737a3-112">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="737a3-112">For applications:</span></span>

|<span data-ttu-id="737a3-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="737a3-113">Permission type</span></span>      | <span data-ttu-id="737a3-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="737a3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="737a3-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="737a3-115">Delegated (work or school account)</span></span> | <span data-ttu-id="737a3-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="737a3-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="737a3-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="737a3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="737a3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="737a3-118">Not supported.</span></span>    |
|<span data-ttu-id="737a3-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="737a3-119">Application</span></span> | <span data-ttu-id="737a3-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="737a3-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="737a3-121">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="737a3-121">For users:</span></span>

|<span data-ttu-id="737a3-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="737a3-122">Permission type</span></span>      | <span data-ttu-id="737a3-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="737a3-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="737a3-124">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="737a3-124">Delegated (work or school account)</span></span> | <span data-ttu-id="737a3-125">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="737a3-125">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="737a3-126">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="737a3-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="737a3-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="737a3-127">Not supported.</span></span> |
|<span data-ttu-id="737a3-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="737a3-128">Application</span></span> | <span data-ttu-id="737a3-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="737a3-129">Not supported.</span></span> |

<span data-ttu-id="737a3-130">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="737a3-130">For groups:</span></span>

|<span data-ttu-id="737a3-131">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="737a3-131">Permission type</span></span>      | <span data-ttu-id="737a3-132">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="737a3-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="737a3-133">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="737a3-133">Delegated (work or school account)</span></span> | <span data-ttu-id="737a3-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="737a3-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="737a3-135">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="737a3-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="737a3-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="737a3-136">Not supported.</span></span>    |
|<span data-ttu-id="737a3-137">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="737a3-137">Application</span></span> | <span data-ttu-id="737a3-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="737a3-138">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="737a3-139">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="737a3-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="737a3-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="737a3-140">Request headers</span></span>
| <span data-ttu-id="737a3-141">Nome</span><span class="sxs-lookup"><span data-stu-id="737a3-141">Name</span></span>       | <span data-ttu-id="737a3-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="737a3-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="737a3-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="737a3-143">Authorization</span></span>  | <span data-ttu-id="737a3-144">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="737a3-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="737a3-145">Aceitar</span><span class="sxs-lookup"><span data-stu-id="737a3-145">Accept</span></span>  | <span data-ttu-id="737a3-146">application/json</span><span class="sxs-lookup"><span data-stu-id="737a3-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="737a3-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="737a3-147">Request body</span></span>
<span data-ttu-id="737a3-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="737a3-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="737a3-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="737a3-149">Response</span></span>

<span data-ttu-id="737a3-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="737a3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="737a3-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="737a3-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="737a3-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="737a3-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="737a3-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="737a3-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="c"></a>[<span data-ttu-id="737a3-155">C#</span><span class="sxs-lookup"><span data-stu-id="737a3-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="737a3-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="737a3-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="737a3-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="737a3-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="737a3-158">Java</span><span class="sxs-lookup"><span data-stu-id="737a3-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="737a3-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="737a3-159">Response</span></span>
<span data-ttu-id="737a3-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="737a3-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

