---
title: Excluir permanentemente item
description: Excluir permanentemente um item de itens excluídos.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 91d39f790e49c725c04830f14e879fb7303c4454
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963337"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="94a38-103">Excluir permanentemente item</span><span class="sxs-lookup"><span data-stu-id="94a38-103">Permanently delete item</span></span>

<span data-ttu-id="94a38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94a38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94a38-105">Excluir permanentemente um item de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="94a38-105">Permanently delete an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="94a38-106">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](../resources/application.md), [grupo](../resources/group.md) e recursos do [usuário](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="94a38-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="94a38-107">É possível excluir permanentemente um item de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="94a38-107">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="94a38-108">Mas, uma vez que um item é excluído permanentemente, ele **não pode** ser restaurado.</span><span class="sxs-lookup"><span data-stu-id="94a38-108">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="94a38-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="94a38-109">Permissions</span></span>
<span data-ttu-id="94a38-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94a38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="94a38-112">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="94a38-112">For applications:</span></span>

|<span data-ttu-id="94a38-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94a38-113">Permission type</span></span>      | <span data-ttu-id="94a38-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94a38-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a38-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94a38-115">Delegated (work or school account)</span></span> | <span data-ttu-id="94a38-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94a38-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94a38-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94a38-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a38-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a38-118">Not supported.</span></span>    |
|<span data-ttu-id="94a38-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94a38-119">Application</span></span> | <span data-ttu-id="94a38-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94a38-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="94a38-121">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="94a38-121">For users:</span></span>

|<span data-ttu-id="94a38-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94a38-122">Permission type</span></span>      | <span data-ttu-id="94a38-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94a38-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a38-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94a38-124">Delegated (work or school account)</span></span> | <span data-ttu-id="94a38-125">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94a38-125">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="94a38-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94a38-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a38-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a38-127">Not supported.</span></span> |
|<span data-ttu-id="94a38-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94a38-128">Application</span></span> | <span data-ttu-id="94a38-129">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94a38-129">User.ReadWrite.All</span></span> |

<span data-ttu-id="94a38-130">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="94a38-130">For groups:</span></span>

|<span data-ttu-id="94a38-131">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94a38-131">Permission type</span></span>      | <span data-ttu-id="94a38-132">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94a38-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a38-133">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94a38-133">Delegated (work or school account)</span></span> | <span data-ttu-id="94a38-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94a38-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="94a38-135">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94a38-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a38-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a38-136">Not supported.</span></span>    |
|<span data-ttu-id="94a38-137">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94a38-137">Application</span></span> | <span data-ttu-id="94a38-138">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94a38-138">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94a38-139">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94a38-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="94a38-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94a38-140">Request headers</span></span>
| <span data-ttu-id="94a38-141">Nome</span><span class="sxs-lookup"><span data-stu-id="94a38-141">Name</span></span>       | <span data-ttu-id="94a38-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="94a38-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="94a38-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="94a38-143">Authorization</span></span>  | <span data-ttu-id="94a38-144">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="94a38-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="94a38-145">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94a38-145">Accept</span></span>  | <span data-ttu-id="94a38-146">application/json</span><span class="sxs-lookup"><span data-stu-id="94a38-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="94a38-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94a38-147">Request body</span></span>
<span data-ttu-id="94a38-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94a38-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94a38-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a38-149">Response</span></span>

<span data-ttu-id="94a38-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94a38-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94a38-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94a38-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94a38-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94a38-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="94a38-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="94a38-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="c"></a>[<span data-ttu-id="94a38-155">C#</span><span class="sxs-lookup"><span data-stu-id="94a38-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94a38-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94a38-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94a38-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94a38-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94a38-158">Java</span><span class="sxs-lookup"><span data-stu-id="94a38-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="94a38-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a38-159">Response</span></span>
<span data-ttu-id="94a38-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94a38-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


