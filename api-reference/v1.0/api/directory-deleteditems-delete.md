---
title: Excluir permanentemente um item de itens excluídos
description: Exclui permanentemente um item de itens excluídos.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 090f41ed4f6bc1410dccede72fe432e38320de0a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053206"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="e5b02-103">Excluir permanentemente item</span><span class="sxs-lookup"><span data-stu-id="e5b02-103">Permanently delete item</span></span>

<span data-ttu-id="e5b02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5b02-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5b02-105">Exclui permanentemente um item de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="e5b02-105">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="e5b02-106">Atualmente, a funcionalidade de itens excluídos só tem suporte para os recursos [de](../resources/application.md)aplicativo, [grupo](../resources/group.md) [e](../resources/user.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="e5b02-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="e5b02-107">É possível excluir permanentemente um item de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="e5b02-107">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="e5b02-108">Mas, uma vez que um item é excluído permanentemente, ele **não pode** ser restaurado.</span><span class="sxs-lookup"><span data-stu-id="e5b02-108">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5b02-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5b02-109">Permissions</span></span>
<span data-ttu-id="e5b02-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5b02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e5b02-112">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="e5b02-112">For applications:</span></span>

|<span data-ttu-id="e5b02-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5b02-113">Permission type</span></span>      | <span data-ttu-id="e5b02-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5b02-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5b02-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5b02-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e5b02-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5b02-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5b02-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5b02-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5b02-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5b02-118">Not supported.</span></span>    |
|<span data-ttu-id="e5b02-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5b02-119">Application</span></span> | <span data-ttu-id="e5b02-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5b02-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="e5b02-121">O solicitante precisa ter uma das seguintes funções: *Administrador Global* ou Administrador *de Aplicativos.*</span><span class="sxs-lookup"><span data-stu-id="e5b02-121">The requestor needs to have one of the following roles: *Global Administrator* or *Application Administrator*.</span></span>

<span data-ttu-id="e5b02-122">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="e5b02-122">For users:</span></span>

|<span data-ttu-id="e5b02-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5b02-123">Permission type</span></span>      | <span data-ttu-id="e5b02-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5b02-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5b02-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5b02-125">Delegated (work or school account)</span></span> | <span data-ttu-id="e5b02-126">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5b02-126">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e5b02-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5b02-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5b02-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5b02-128">Not supported.</span></span> |
|<span data-ttu-id="e5b02-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5b02-129">Application</span></span> | <span data-ttu-id="e5b02-130">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5b02-130">Not supported.</span></span> |

<span data-ttu-id="e5b02-131">O usuário inscreveu precisa ter uma das seguintes funções: *Administrador Global* ou Administrador *de Usuário.*</span><span class="sxs-lookup"><span data-stu-id="e5b02-131">The signed-in user needs to have one of the following roles: *Global Administrator* or *User Administrator*.</span></span>

<span data-ttu-id="e5b02-132">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="e5b02-132">For groups:</span></span>

|<span data-ttu-id="e5b02-133">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5b02-133">Permission type</span></span>      | <span data-ttu-id="e5b02-134">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5b02-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5b02-135">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5b02-135">Delegated (work or school account)</span></span> | <span data-ttu-id="e5b02-136">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5b02-136">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e5b02-137">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5b02-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5b02-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5b02-138">Not supported.</span></span>    |
|<span data-ttu-id="e5b02-139">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5b02-139">Application</span></span> | <span data-ttu-id="e5b02-140">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5b02-140">Not supported.</span></span> |

<span data-ttu-id="e5b02-141">O solicitante precisa ter uma das seguintes funções: *Administrador Global* ou Administrador *de Grupos.*</span><span class="sxs-lookup"><span data-stu-id="e5b02-141">The requestor needs to have one of the following roles: *Global Administrator* or *Groups Administrator*.</span></span>

## <a name="http-request"></a><span data-ttu-id="e5b02-142">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5b02-142">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e5b02-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5b02-143">Request headers</span></span>
| <span data-ttu-id="e5b02-144">Nome</span><span class="sxs-lookup"><span data-stu-id="e5b02-144">Name</span></span>       | <span data-ttu-id="e5b02-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5b02-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e5b02-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5b02-146">Authorization</span></span>  | <span data-ttu-id="e5b02-147">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="e5b02-147">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="e5b02-148">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e5b02-148">Accept</span></span>  | <span data-ttu-id="e5b02-149">application/json</span><span class="sxs-lookup"><span data-stu-id="e5b02-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5b02-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5b02-150">Request body</span></span>
<span data-ttu-id="e5b02-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5b02-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5b02-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5b02-152">Response</span></span>

<span data-ttu-id="e5b02-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5b02-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5b02-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5b02-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5b02-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5b02-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e5b02-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5b02-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="c"></a>[<span data-ttu-id="e5b02-158">C#</span><span class="sxs-lookup"><span data-stu-id="e5b02-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5b02-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5b02-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5b02-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5b02-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5b02-161">Java</span><span class="sxs-lookup"><span data-stu-id="e5b02-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e5b02-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5b02-162">Response</span></span>
<span data-ttu-id="e5b02-163">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e5b02-163">Note: The response object shown here might be shortened for readability.</span></span>
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

