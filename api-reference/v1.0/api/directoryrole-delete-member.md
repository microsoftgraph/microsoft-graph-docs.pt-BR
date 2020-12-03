---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 72491fbc37dfbb77411178e9cfdfe2147d5119b7
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522789"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="16052-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="16052-103">Remove directory role member</span></span>

<span data-ttu-id="16052-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16052-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16052-105">Remover um membro de um [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="16052-105">Remove a member from a [directoryRole](../resources/directoryrole.md).</span></span>

> [!Note]
> <span data-ttu-id="16052-106">Você pode usar a ID de objeto e a ID de modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="16052-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="16052-107">A ID de modelo de uma função interna é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="16052-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="16052-108">Para obter detalhes, consulte [role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="16052-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="16052-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="16052-109">Permissions</span></span>

<span data-ttu-id="16052-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16052-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="16052-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16052-112">Permission type</span></span>      | <span data-ttu-id="16052-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16052-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16052-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16052-114">Delegated (work or school account)</span></span> | <span data-ttu-id="16052-115">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="16052-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="16052-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16052-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16052-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16052-117">Not supported.</span></span>    |
|<span data-ttu-id="16052-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16052-118">Application</span></span> | <span data-ttu-id="16052-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="16052-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="16052-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16052-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="16052-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16052-121">Request headers</span></span>

| <span data-ttu-id="16052-122">Nome</span><span class="sxs-lookup"><span data-stu-id="16052-122">Name</span></span>       | <span data-ttu-id="16052-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="16052-123">Type</span></span> | <span data-ttu-id="16052-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="16052-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16052-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="16052-125">Authorization</span></span>  | <span data-ttu-id="16052-126">string</span><span class="sxs-lookup"><span data-stu-id="16052-126">string</span></span>  | <span data-ttu-id="16052-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16052-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16052-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16052-129">Request body</span></span>

<span data-ttu-id="16052-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16052-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16052-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="16052-131">Response</span></span>

<span data-ttu-id="16052-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16052-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16052-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="16052-134">Examples</span></span>

### <a name="example-1-remove-directory-role-member-using-role-objectid"></a><span data-ttu-id="16052-135">Exemplo 1: remover membro da função de diretório usando objectId de função</span><span class="sxs-lookup"><span data-stu-id="16052-135">Example 1: Remove directory role member using role objectId</span></span>

##### <a name="request"></a><span data-ttu-id="16052-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16052-136">Request</span></span>

<span data-ttu-id="16052-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16052-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16052-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="16052-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_objectId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{role-objectId}/members/{user-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="16052-139">C#</span><span class="sxs-lookup"><span data-stu-id="16052-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16052-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16052-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16052-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16052-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16052-142">Java</span><span class="sxs-lookup"><span data-stu-id="16052-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="16052-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="16052-143">Response</span></span>

<span data-ttu-id="16052-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16052-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-directory-role-member-using-role-templateid"></a><span data-ttu-id="16052-145">Exemplo 2: remover o membro de função de diretório usando o TemplateID de função</span><span class="sxs-lookup"><span data-stu-id="16052-145">Example 2: Remove directory role member using role templateId</span></span>

##### <a name="request"></a><span data-ttu-id="16052-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16052-146">Request</span></span>

<span data-ttu-id="16052-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16052-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16052-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="16052-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_templateId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId={role-templateId}/members/{user-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="16052-149">C#</span><span class="sxs-lookup"><span data-stu-id="16052-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16052-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16052-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16052-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16052-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16052-152">Java</span><span class="sxs-lookup"><span data-stu-id="16052-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="16052-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="16052-153">Response</span></span>

<span data-ttu-id="16052-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16052-154">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

