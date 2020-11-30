---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2c6c8dba462c4514907c4d167810abe1ccfe3cd7
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377065"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="6710f-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="6710f-103">Remove directory role member</span></span>

<span data-ttu-id="6710f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6710f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6710f-105">Remover um membro de um [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="6710f-105">Remove a member from a [directoryRole](../resources/directoryrole.md).</span></span>

> [!Note]
> <span data-ttu-id="6710f-106">Você pode usar a ID de objeto e a ID de modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="6710f-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="6710f-107">A ID de modelo de uma função interna é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6710f-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="6710f-108">Para obter detalhes, consulte [role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="6710f-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="6710f-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="6710f-109">Permissions</span></span>

<span data-ttu-id="6710f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6710f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6710f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6710f-112">Permission type</span></span>      | <span data-ttu-id="6710f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6710f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6710f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6710f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6710f-115">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="6710f-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6710f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6710f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6710f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6710f-117">Not supported.</span></span>    |
|<span data-ttu-id="6710f-118">Application</span><span class="sxs-lookup"><span data-stu-id="6710f-118">Application</span></span> | <span data-ttu-id="6710f-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="6710f-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="6710f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6710f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6710f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6710f-121">Request headers</span></span>

| <span data-ttu-id="6710f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6710f-122">Name</span></span>       | <span data-ttu-id="6710f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="6710f-123">Type</span></span> | <span data-ttu-id="6710f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6710f-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6710f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6710f-125">Authorization</span></span>  | <span data-ttu-id="6710f-126">string</span><span class="sxs-lookup"><span data-stu-id="6710f-126">string</span></span>  | <span data-ttu-id="6710f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6710f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6710f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6710f-129">Request body</span></span>

<span data-ttu-id="6710f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6710f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6710f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6710f-131">Response</span></span>

<span data-ttu-id="6710f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6710f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6710f-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6710f-134">Examples</span></span>

### <a name="example-1-remove-directory-role-member-using-role-objectid"></a><span data-ttu-id="6710f-135">Exemplo 1: remover membro da função de diretório usando objectId de função</span><span class="sxs-lookup"><span data-stu-id="6710f-135">Example 1: Remove directory role member using role objectId</span></span>

##### <a name="request"></a><span data-ttu-id="6710f-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6710f-136">Request</span></span>

<span data-ttu-id="6710f-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6710f-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6710f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6710f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_objectId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{role-objectId}/members/{user-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="6710f-139">C#</span><span class="sxs-lookup"><span data-stu-id="6710f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6710f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6710f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6710f-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6710f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6710f-142">Java</span><span class="sxs-lookup"><span data-stu-id="6710f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6710f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6710f-143">Response</span></span>

<span data-ttu-id="6710f-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6710f-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-directory-role-member-using-role-templateid"></a><span data-ttu-id="6710f-145">Exemplo 2: remover o membro de função de diretório usando o TemplateID de função</span><span class="sxs-lookup"><span data-stu-id="6710f-145">Example 2: Remove directory role member using role templateId</span></span>

##### <a name="request"></a><span data-ttu-id="6710f-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6710f-146">Request</span></span>

<span data-ttu-id="6710f-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6710f-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6710f-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="6710f-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_templateId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId={role-templateId}/members/{user-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="6710f-149">C#</span><span class="sxs-lookup"><span data-stu-id="6710f-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6710f-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6710f-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6710f-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6710f-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6710f-152">Java</span><span class="sxs-lookup"><span data-stu-id="6710f-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6710f-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6710f-153">Response</span></span>

<span data-ttu-id="6710f-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6710f-154">Here is an example of the response.</span></span> 
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

