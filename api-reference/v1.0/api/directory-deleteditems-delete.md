---
title: Excluir permanentemente um item de itens excluídos
description: Exclui permanentemente um item de itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d18bd2a20920d17737e3d517ed09d2a06bd5432d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939807"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="07a93-103">Excluir permanentemente item</span><span class="sxs-lookup"><span data-stu-id="07a93-103">Permanently delete item</span></span>

<span data-ttu-id="07a93-104">Exclui permanentemente um item de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="07a93-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="07a93-105">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](../resources/application.md), [grupo](../resources/group.md) e recursos do [usuário](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="07a93-105">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="07a93-106">É possível excluir permanentemente um item de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="07a93-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="07a93-107">Mas, uma vez que um item é excluído permanentemente, ele **não pode** ser restaurado.</span><span class="sxs-lookup"><span data-stu-id="07a93-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="07a93-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="07a93-108">Permissions</span></span>
<span data-ttu-id="07a93-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07a93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="07a93-111">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="07a93-111">For applications:</span></span>

|<span data-ttu-id="07a93-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07a93-112">Permission type</span></span>      | <span data-ttu-id="07a93-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07a93-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07a93-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07a93-114">Delegated (work or school account)</span></span> | <span data-ttu-id="07a93-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07a93-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07a93-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07a93-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07a93-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07a93-117">Not supported.</span></span>    |
|<span data-ttu-id="07a93-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07a93-118">Application</span></span> | <span data-ttu-id="07a93-119">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07a93-119">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="07a93-120">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="07a93-120">For users:</span></span>

|<span data-ttu-id="07a93-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07a93-121">Permission type</span></span>      | <span data-ttu-id="07a93-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07a93-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07a93-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07a93-123">Delegated (work or school account)</span></span> | <span data-ttu-id="07a93-124">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07a93-124">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="07a93-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07a93-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07a93-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07a93-126">Not supported.</span></span> |
|<span data-ttu-id="07a93-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07a93-127">Application</span></span> | <span data-ttu-id="07a93-128">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07a93-128">User.ReadWrite.All</span></span> |

<span data-ttu-id="07a93-129">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="07a93-129">For groups:</span></span>

|<span data-ttu-id="07a93-130">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07a93-130">Permission type</span></span>      | <span data-ttu-id="07a93-131">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07a93-131">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07a93-132">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07a93-132">Delegated (work or school account)</span></span> | <span data-ttu-id="07a93-133">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07a93-133">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="07a93-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07a93-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07a93-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07a93-135">Not supported.</span></span>    |
|<span data-ttu-id="07a93-136">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07a93-136">Application</span></span> | <span data-ttu-id="07a93-137">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07a93-137">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07a93-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07a93-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="07a93-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07a93-139">Request headers</span></span>
| <span data-ttu-id="07a93-140">Nome</span><span class="sxs-lookup"><span data-stu-id="07a93-140">Name</span></span>       | <span data-ttu-id="07a93-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="07a93-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="07a93-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="07a93-142">Authorization</span></span>  | <span data-ttu-id="07a93-143">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="07a93-143">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="07a93-144">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07a93-144">Accept</span></span>  | <span data-ttu-id="07a93-145">application/json</span><span class="sxs-lookup"><span data-stu-id="07a93-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="07a93-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07a93-146">Request body</span></span>
<span data-ttu-id="07a93-147">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07a93-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07a93-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="07a93-148">Response</span></span>

<span data-ttu-id="07a93-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07a93-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07a93-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07a93-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07a93-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07a93-152">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="07a93-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="07a93-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="07a93-154">C#</span><span class="sxs-lookup"><span data-stu-id="07a93-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07a93-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07a93-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="07a93-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07a93-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="07a93-157">Java</span><span class="sxs-lookup"><span data-stu-id="07a93-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="07a93-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="07a93-158">Response</span></span>
<span data-ttu-id="07a93-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07a93-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
