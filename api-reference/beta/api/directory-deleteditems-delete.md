---
title: Excluir permanentemente item
description: Exclua permanentemente um item de itens excluídos.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5fe36d8a129a42dcd139b36577f0ae7fab45a6f6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437055"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="1073f-103">Excluir permanentemente item</span><span class="sxs-lookup"><span data-stu-id="1073f-103">Permanently delete item</span></span>

<span data-ttu-id="1073f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1073f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1073f-105">Exclua permanentemente um item [de itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="1073f-105">Permanently delete an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="1073f-106">Atualmente, a funcionalidade de itens excluídos só tem suporte para os recursos [de](../resources/application.md)aplicativo, [grupo](../resources/group.md) [e](../resources/user.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="1073f-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="1073f-107">É possível excluir permanentemente um item de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="1073f-107">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="1073f-108">Mas, uma vez que um item é excluído permanentemente, ele **não pode** ser restaurado.</span><span class="sxs-lookup"><span data-stu-id="1073f-108">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="1073f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1073f-109">Permissions</span></span>
<span data-ttu-id="1073f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1073f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1073f-112">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="1073f-112">For applications:</span></span>

|<span data-ttu-id="1073f-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1073f-113">Permission type</span></span>      | <span data-ttu-id="1073f-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1073f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1073f-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1073f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="1073f-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1073f-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1073f-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1073f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1073f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1073f-118">Not supported.</span></span>    |
|<span data-ttu-id="1073f-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1073f-119">Application</span></span> | <span data-ttu-id="1073f-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1073f-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="1073f-121">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="1073f-121">For users:</span></span>

|<span data-ttu-id="1073f-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1073f-122">Permission type</span></span>      | <span data-ttu-id="1073f-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1073f-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1073f-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1073f-124">Delegated (work or school account)</span></span> | <span data-ttu-id="1073f-125">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1073f-125">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1073f-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1073f-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1073f-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1073f-127">Not supported.</span></span> |
|<span data-ttu-id="1073f-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1073f-128">Application</span></span> | <span data-ttu-id="1073f-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1073f-129">Not supported.</span></span> |

<span data-ttu-id="1073f-130">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="1073f-130">For groups:</span></span>

|<span data-ttu-id="1073f-131">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1073f-131">Permission type</span></span>      | <span data-ttu-id="1073f-132">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1073f-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1073f-133">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1073f-133">Delegated (work or school account)</span></span> | <span data-ttu-id="1073f-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1073f-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1073f-135">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1073f-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1073f-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1073f-136">Not supported.</span></span>    |
|<span data-ttu-id="1073f-137">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1073f-137">Application</span></span> | <span data-ttu-id="1073f-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1073f-138">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1073f-139">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1073f-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1073f-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1073f-140">Request headers</span></span>
| <span data-ttu-id="1073f-141">Nome</span><span class="sxs-lookup"><span data-stu-id="1073f-141">Name</span></span>       | <span data-ttu-id="1073f-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="1073f-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1073f-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="1073f-143">Authorization</span></span>  | <span data-ttu-id="1073f-144">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="1073f-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="1073f-145">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1073f-145">Accept</span></span>  | <span data-ttu-id="1073f-146">application/json</span><span class="sxs-lookup"><span data-stu-id="1073f-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1073f-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1073f-147">Request body</span></span>
<span data-ttu-id="1073f-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1073f-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1073f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1073f-149">Response</span></span>

<span data-ttu-id="1073f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1073f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1073f-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1073f-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1073f-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1073f-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1073f-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="1073f-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="c"></a>[<span data-ttu-id="1073f-155">C#</span><span class="sxs-lookup"><span data-stu-id="1073f-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1073f-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1073f-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1073f-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1073f-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1073f-158">Java</span><span class="sxs-lookup"><span data-stu-id="1073f-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1073f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="1073f-159">Response</span></span>
<span data-ttu-id="1073f-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1073f-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


