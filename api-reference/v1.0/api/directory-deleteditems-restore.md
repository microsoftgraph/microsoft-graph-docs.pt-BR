---
title: Restaurar item excluído
description: 'Restaura um item recentemente excluído de itens excluídos. '
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e1236f50cb637648aa81a64584a60870135a102e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053185"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="b83ae-103">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="b83ae-103">Restore deleted item</span></span>

<span data-ttu-id="b83ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b83ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b83ae-105">Restaura um item recentemente excluído de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="b83ae-105">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="b83ae-106">Atualmente, a funcionalidade de restaurar itens excluídos só é suportada para os recursos [de](../resources/application.md)aplicativo, [grupo](../resources/group.md) [e](../resources/user.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="b83ae-106">Currently, restore deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="b83ae-107">Se um item foi excluído acidentalmente, você poderá restaurá-lo totalmente.</span><span class="sxs-lookup"><span data-stu-id="b83ae-107">If an item was accidentally deleted, you can fully restore the item.</span></span> <span data-ttu-id="b83ae-108">Isso não se aplica a grupos de Segurança, que são excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="b83ae-108">This is not applicable to Security groups, which are deleted permanently.</span></span>

<span data-ttu-id="b83ae-109">Um item recentemente excluído permanecerá disponível por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="b83ae-109">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="b83ae-110">Após 30 dias, esse item será excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="b83ae-110">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="b83ae-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="b83ae-111">Permissions</span></span>
<span data-ttu-id="b83ae-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b83ae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="b83ae-114">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="b83ae-114">For applications:</span></span>

|<span data-ttu-id="b83ae-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b83ae-115">Permission type</span></span>      | <span data-ttu-id="b83ae-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b83ae-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b83ae-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b83ae-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b83ae-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b83ae-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b83ae-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b83ae-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b83ae-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b83ae-120">Not supported.</span></span>    |
|<span data-ttu-id="b83ae-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b83ae-121">Application</span></span> | <span data-ttu-id="b83ae-122">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b83ae-122">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |


### <a name="for-users"></a><span data-ttu-id="b83ae-123">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="b83ae-123">For users:</span></span>

|<span data-ttu-id="b83ae-124">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b83ae-124">Permission type</span></span>      | <span data-ttu-id="b83ae-125">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b83ae-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b83ae-126">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b83ae-126">Delegated (work or school account)</span></span> | <span data-ttu-id="b83ae-127">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b83ae-127">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b83ae-128">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b83ae-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b83ae-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b83ae-129">Not supported.</span></span> |
|<span data-ttu-id="b83ae-130">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b83ae-130">Application</span></span> | <span data-ttu-id="b83ae-131">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b83ae-131">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="b83ae-132">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="b83ae-132">For groups:</span></span>

|<span data-ttu-id="b83ae-133">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b83ae-133">Permission type</span></span>      | <span data-ttu-id="b83ae-134">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b83ae-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b83ae-135">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b83ae-135">Delegated (work or school account)</span></span> | <span data-ttu-id="b83ae-136">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b83ae-136">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b83ae-137">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b83ae-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b83ae-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b83ae-138">Not supported.</span></span>    |
|<span data-ttu-id="b83ae-139">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b83ae-139">Application</span></span> | <span data-ttu-id="b83ae-140">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b83ae-140">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b83ae-141">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b83ae-141">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="b83ae-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b83ae-142">Request headers</span></span>
| <span data-ttu-id="b83ae-143">Nome</span><span class="sxs-lookup"><span data-stu-id="b83ae-143">Name</span></span>       | <span data-ttu-id="b83ae-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="b83ae-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b83ae-145">Autorização</span><span class="sxs-lookup"><span data-stu-id="b83ae-145">Authorization</span></span>  | <span data-ttu-id="b83ae-146">Token de &lt; portador &gt; *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="b83ae-146">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="b83ae-147">Content-type</span><span class="sxs-lookup"><span data-stu-id="b83ae-147">Content-type</span></span> | <span data-ttu-id="b83ae-148">application/json</span><span class="sxs-lookup"><span data-stu-id="b83ae-148">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b83ae-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b83ae-149">Request body</span></span>
<span data-ttu-id="b83ae-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b83ae-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b83ae-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b83ae-151">Response</span></span>

<span data-ttu-id="b83ae-152">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b83ae-152">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b83ae-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b83ae-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="b83ae-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b83ae-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b83ae-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="b83ae-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
# <a name="c"></a>[<span data-ttu-id="b83ae-156">C#</span><span class="sxs-lookup"><span data-stu-id="b83ae-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b83ae-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b83ae-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b83ae-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b83ae-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b83ae-159">Java</span><span class="sxs-lookup"><span data-stu-id="b83ae-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b83ae-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="b83ae-160">Response</span></span>
<span data-ttu-id="b83ae-161">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b83ae-161">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "@odata.type":"#microsoft.graph.group",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

