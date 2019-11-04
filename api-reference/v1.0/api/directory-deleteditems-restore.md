---
title: Restaurar item excluído
description: 'Restaura um item recentemente excluído de itens excluídos. '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 11151e543a973b003334ee360c6eebcbc0c27063
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938797"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="47f21-103">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="47f21-103">Restore deleted item</span></span>

<span data-ttu-id="47f21-104">Restaura um item recentemente excluído de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="47f21-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="47f21-105">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](../resources/application.md), [grupo](../resources/group.md) e recursos do [usuário](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="47f21-105">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="47f21-106">Se um item foi excluído acidentalmente, você poderá restaurá-lo totalmente.</span><span class="sxs-lookup"><span data-stu-id="47f21-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="47f21-107">Um item recentemente excluído permanecerá disponível por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="47f21-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="47f21-108">Após 30 dias, esse item será excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="47f21-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="47f21-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="47f21-109">Permissions</span></span>
<span data-ttu-id="47f21-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47f21-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="47f21-112">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="47f21-112">For applications:</span></span>

|<span data-ttu-id="47f21-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47f21-113">Permission type</span></span>      | <span data-ttu-id="47f21-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47f21-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47f21-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47f21-115">Delegated (work or school account)</span></span> | <span data-ttu-id="47f21-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="47f21-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="47f21-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47f21-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47f21-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47f21-118">Not supported.</span></span>    |
|<span data-ttu-id="47f21-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47f21-119">Application</span></span> | <span data-ttu-id="47f21-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47f21-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |


### <a name="for-users"></a><span data-ttu-id="47f21-121">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="47f21-121">For users:</span></span>

|<span data-ttu-id="47f21-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47f21-122">Permission type</span></span>      | <span data-ttu-id="47f21-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47f21-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47f21-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47f21-124">Delegated (work or school account)</span></span> | <span data-ttu-id="47f21-125">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="47f21-125">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="47f21-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47f21-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47f21-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47f21-127">Not supported.</span></span> |
|<span data-ttu-id="47f21-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47f21-128">Application</span></span> | <span data-ttu-id="47f21-129">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47f21-129">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="47f21-130">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="47f21-130">For groups:</span></span>

|<span data-ttu-id="47f21-131">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47f21-131">Permission type</span></span>      | <span data-ttu-id="47f21-132">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47f21-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47f21-133">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47f21-133">Delegated (work or school account)</span></span> | <span data-ttu-id="47f21-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="47f21-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="47f21-135">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47f21-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47f21-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47f21-136">Not supported.</span></span>    |
|<span data-ttu-id="47f21-137">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47f21-137">Application</span></span> | <span data-ttu-id="47f21-138">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47f21-138">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47f21-139">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47f21-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="47f21-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47f21-140">Request headers</span></span>
| <span data-ttu-id="47f21-141">Nome</span><span class="sxs-lookup"><span data-stu-id="47f21-141">Name</span></span>       | <span data-ttu-id="47f21-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="47f21-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="47f21-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="47f21-143">Authorization</span></span>  | <span data-ttu-id="47f21-144">&lt;Token&gt; de portador *necessário*</span><span class="sxs-lookup"><span data-stu-id="47f21-144">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="47f21-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="47f21-145">Content-type</span></span> | <span data-ttu-id="47f21-146">application/json</span><span class="sxs-lookup"><span data-stu-id="47f21-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="47f21-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47f21-147">Request body</span></span>
<span data-ttu-id="47f21-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47f21-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47f21-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="47f21-149">Response</span></span>

<span data-ttu-id="47f21-150">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47f21-150">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47f21-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47f21-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="47f21-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47f21-152">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="47f21-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="47f21-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="47f21-154">C#</span><span class="sxs-lookup"><span data-stu-id="47f21-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47f21-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47f21-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="47f21-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47f21-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="47f21-157">Java</span><span class="sxs-lookup"><span data-stu-id="47f21-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="47f21-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="47f21-158">Response</span></span>
<span data-ttu-id="47f21-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47f21-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
