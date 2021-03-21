---
title: Excluir permanentemente um item de itens excluídos
description: Exclui permanentemente um item de itens excluídos.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e673ffebf6bfae9c7d4271ef117d9a8c388ab58a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956755"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="c91ed-103">Excluir permanentemente item</span><span class="sxs-lookup"><span data-stu-id="c91ed-103">Permanently delete item</span></span>

<span data-ttu-id="c91ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c91ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c91ed-105">Exclui permanentemente um item de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="c91ed-105">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="c91ed-106">Atualmente, a funcionalidade de itens excluídos só tem suporte para os recursos [de](../resources/application.md)aplicativo, [grupo](../resources/group.md) [e](../resources/user.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="c91ed-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="c91ed-107">É possível excluir permanentemente um item de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="c91ed-107">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="c91ed-108">Mas, uma vez que um item é excluído permanentemente, ele **não pode** ser restaurado.</span><span class="sxs-lookup"><span data-stu-id="c91ed-108">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="c91ed-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c91ed-109">Permissions</span></span>
<span data-ttu-id="c91ed-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c91ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c91ed-112">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="c91ed-112">For applications:</span></span>

|<span data-ttu-id="c91ed-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c91ed-113">Permission type</span></span>      | <span data-ttu-id="c91ed-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c91ed-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c91ed-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c91ed-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c91ed-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c91ed-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c91ed-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c91ed-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c91ed-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c91ed-118">Not supported.</span></span>    |
|<span data-ttu-id="c91ed-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c91ed-119">Application</span></span> | <span data-ttu-id="c91ed-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c91ed-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="c91ed-121">O solicitante precisa ter uma das seguintes funções: *Administrador Global* ou Administrador *de Aplicativos.*</span><span class="sxs-lookup"><span data-stu-id="c91ed-121">The requestor needs to have one of the following roles: *Global Administrator* or *Application Administrator*.</span></span>

<span data-ttu-id="c91ed-122">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="c91ed-122">For users:</span></span>

|<span data-ttu-id="c91ed-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c91ed-123">Permission type</span></span>      | <span data-ttu-id="c91ed-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c91ed-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c91ed-125">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c91ed-125">Delegated (work or school account)</span></span> | <span data-ttu-id="c91ed-126">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c91ed-126">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c91ed-127">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c91ed-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c91ed-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c91ed-128">Not supported.</span></span> |
|<span data-ttu-id="c91ed-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c91ed-129">Application</span></span> | <span data-ttu-id="c91ed-130">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c91ed-130">Not supported.</span></span> |

<span data-ttu-id="c91ed-131">O usuário inscreveu precisa ter uma das seguintes funções: *Administrador Global* ou Administrador *de Usuário.*</span><span class="sxs-lookup"><span data-stu-id="c91ed-131">The signed-in user needs to have one of the following roles: *Global Administrator* or *User Administrator*.</span></span>

<span data-ttu-id="c91ed-132">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="c91ed-132">For groups:</span></span>

|<span data-ttu-id="c91ed-133">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c91ed-133">Permission type</span></span>      | <span data-ttu-id="c91ed-134">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c91ed-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c91ed-135">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c91ed-135">Delegated (work or school account)</span></span> | <span data-ttu-id="c91ed-136">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c91ed-136">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c91ed-137">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c91ed-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c91ed-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c91ed-138">Not supported.</span></span>    |
|<span data-ttu-id="c91ed-139">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c91ed-139">Application</span></span> | <span data-ttu-id="c91ed-140">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c91ed-140">Not supported.</span></span> |

<span data-ttu-id="c91ed-141">O solicitante precisa ter uma das seguintes funções: *Administrador Global* ou Administrador *de Grupos.*</span><span class="sxs-lookup"><span data-stu-id="c91ed-141">The requestor needs to have one of the following roles: *Global Administrator* or *Groups Administrator*.</span></span>

## <a name="http-request"></a><span data-ttu-id="c91ed-142">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c91ed-142">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c91ed-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c91ed-143">Request headers</span></span>
| <span data-ttu-id="c91ed-144">Nome</span><span class="sxs-lookup"><span data-stu-id="c91ed-144">Name</span></span>       | <span data-ttu-id="c91ed-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="c91ed-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c91ed-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="c91ed-146">Authorization</span></span>  | <span data-ttu-id="c91ed-147">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="c91ed-147">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="c91ed-148">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c91ed-148">Accept</span></span>  | <span data-ttu-id="c91ed-149">application/json</span><span class="sxs-lookup"><span data-stu-id="c91ed-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c91ed-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c91ed-150">Request body</span></span>
<span data-ttu-id="c91ed-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c91ed-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c91ed-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="c91ed-152">Response</span></span>

<span data-ttu-id="c91ed-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c91ed-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c91ed-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c91ed-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c91ed-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c91ed-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c91ed-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="c91ed-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="c"></a>[<span data-ttu-id="c91ed-158">C#</span><span class="sxs-lookup"><span data-stu-id="c91ed-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c91ed-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c91ed-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c91ed-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c91ed-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c91ed-161">Java</span><span class="sxs-lookup"><span data-stu-id="c91ed-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c91ed-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c91ed-162">Response</span></span>
<span data-ttu-id="c91ed-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c91ed-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

