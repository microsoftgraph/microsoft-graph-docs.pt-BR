---
title: Restaurar item excluído
description: 'Restaura um item recentemente excluído de itens excluídos. '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ee4585fd4465c8457826be84af7ab672d53825b1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518039"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="3dfc2-103">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="3dfc2-103">Restore deleted item</span></span>

<span data-ttu-id="3dfc2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dfc2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3dfc2-105">Restaura um item recentemente excluído de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="3dfc2-105">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="3dfc2-106">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](../resources/application.md), [grupo](../resources/group.md) e recursos do [usuário](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="3dfc2-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="3dfc2-107">Se um item foi excluído acidentalmente, você poderá restaurá-lo totalmente.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-107">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="3dfc2-108">Um item recentemente excluído permanecerá disponível por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-108">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="3dfc2-109">Após 30 dias, esse item será excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-109">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dfc2-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="3dfc2-110">Permissions</span></span>
<span data-ttu-id="3dfc2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dfc2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="3dfc2-113">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="3dfc2-113">For applications:</span></span>

|<span data-ttu-id="3dfc2-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dfc2-114">Permission type</span></span>      | <span data-ttu-id="3dfc2-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3dfc2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dfc2-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dfc2-116">Delegated (work or school account)</span></span> | <span data-ttu-id="3dfc2-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3dfc2-117">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3dfc2-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3dfc2-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dfc2-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-119">Not supported.</span></span>    |
|<span data-ttu-id="3dfc2-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3dfc2-120">Application</span></span> | <span data-ttu-id="3dfc2-121">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dfc2-121">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |


### <a name="for-users"></a><span data-ttu-id="3dfc2-122">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="3dfc2-122">For users:</span></span>

|<span data-ttu-id="3dfc2-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dfc2-123">Permission type</span></span>      | <span data-ttu-id="3dfc2-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3dfc2-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dfc2-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dfc2-125">Delegated (work or school account)</span></span> | <span data-ttu-id="3dfc2-126">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3dfc2-126">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3dfc2-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3dfc2-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dfc2-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-128">Not supported.</span></span> |
|<span data-ttu-id="3dfc2-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3dfc2-129">Application</span></span> | <span data-ttu-id="3dfc2-130">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dfc2-130">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="3dfc2-131">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="3dfc2-131">For groups:</span></span>

|<span data-ttu-id="3dfc2-132">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dfc2-132">Permission type</span></span>      | <span data-ttu-id="3dfc2-133">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3dfc2-133">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dfc2-134">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dfc2-134">Delegated (work or school account)</span></span> | <span data-ttu-id="3dfc2-135">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3dfc2-135">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3dfc2-136">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3dfc2-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dfc2-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-137">Not supported.</span></span>    |
|<span data-ttu-id="3dfc2-138">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3dfc2-138">Application</span></span> | <span data-ttu-id="3dfc2-139">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dfc2-139">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3dfc2-140">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3dfc2-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="3dfc2-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3dfc2-141">Request headers</span></span>
| <span data-ttu-id="3dfc2-142">Nome</span><span class="sxs-lookup"><span data-stu-id="3dfc2-142">Name</span></span>       | <span data-ttu-id="3dfc2-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="3dfc2-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3dfc2-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="3dfc2-144">Authorization</span></span>  | <span data-ttu-id="3dfc2-145">&lt;Token&gt; de portador *necessário*</span><span class="sxs-lookup"><span data-stu-id="3dfc2-145">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="3dfc2-146">Content-type</span><span class="sxs-lookup"><span data-stu-id="3dfc2-146">Content-type</span></span> | <span data-ttu-id="3dfc2-147">application/json</span><span class="sxs-lookup"><span data-stu-id="3dfc2-147">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3dfc2-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3dfc2-148">Request body</span></span>
<span data-ttu-id="3dfc2-149">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dfc2-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dfc2-150">Response</span></span>

<span data-ttu-id="3dfc2-151">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-151">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dfc2-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3dfc2-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="3dfc2-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3dfc2-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3dfc2-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dfc2-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
# <a name="c"></a>[<span data-ttu-id="3dfc2-155">C#</span><span class="sxs-lookup"><span data-stu-id="3dfc2-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dfc2-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dfc2-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dfc2-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dfc2-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3dfc2-158">Java</span><span class="sxs-lookup"><span data-stu-id="3dfc2-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="3dfc2-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dfc2-159">Response</span></span>
<span data-ttu-id="3dfc2-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
