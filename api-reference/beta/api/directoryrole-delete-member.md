---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1743ee7027d2afd0651b4216975a8acad74e24b0
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991727"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="1fb2a-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="1fb2a-103">Remove directory role member</span></span>

<span data-ttu-id="1fb2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fb2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fb2a-105">Remove um membro de um directoryRole.</span><span class="sxs-lookup"><span data-stu-id="1fb2a-105">Remove a member from a directoryRole.</span></span>

<span data-ttu-id="1fb2a-106">Você pode usar a ID do objeto e a ID do modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="1fb2a-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="1fb2a-107">A ID do modelo de uma função embutida é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="1fb2a-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="1fb2a-108">Para obter detalhes, consulte [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="1fb2a-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="1fb2a-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="1fb2a-109">Permissions</span></span>

<span data-ttu-id="1fb2a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fb2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1fb2a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fb2a-112">Permission type</span></span>      | <span data-ttu-id="1fb2a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fb2a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fb2a-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fb2a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1fb2a-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1fb2a-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1fb2a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fb2a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fb2a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fb2a-117">Not supported.</span></span>    |
|<span data-ttu-id="1fb2a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fb2a-118">Application</span></span> | <span data-ttu-id="1fb2a-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="1fb2a-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fb2a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fb2a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{role-objectId}/members/{id}/$ref
DELETE /directoryRoles/roleTemplateId={role-templateId}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1fb2a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fb2a-121">Request headers</span></span>

| <span data-ttu-id="1fb2a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1fb2a-122">Name</span></span>       | <span data-ttu-id="1fb2a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fb2a-123">Type</span></span> | <span data-ttu-id="1fb2a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fb2a-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1fb2a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fb2a-125">Authorization</span></span>  | <span data-ttu-id="1fb2a-126">string</span><span class="sxs-lookup"><span data-stu-id="1fb2a-126">string</span></span>  | <span data-ttu-id="1fb2a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fb2a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fb2a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fb2a-129">Request body</span></span>

<span data-ttu-id="1fb2a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1fb2a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fb2a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fb2a-131">Response</span></span>

<span data-ttu-id="1fb2a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fb2a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1fb2a-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1fb2a-134">Examples</span></span>

### <a name="example-1-remove-directory-role-member-using-role-objectid"></a><span data-ttu-id="1fb2a-135">Exemplo 1: Remover membro da função de diretório usando objectId de função</span><span class="sxs-lookup"><span data-stu-id="1fb2a-135">Example 1: Remove directory role member using role objectId</span></span>

#### <a name="request"></a><span data-ttu-id="1fb2a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fb2a-136">Request</span></span>

<span data-ttu-id="1fb2a-137">Neste exemplo, substitua pelo valor de id da função de diretório e pelo valor de id do usuário ou objeto de diretório que você deseja `f8e85ed8-f66f-4058-b170-3efae8b9c6e5` desasinalhar da função de  `bb165b45-151c-4cf6-9911-cd7188912848` diretório. </span><span class="sxs-lookup"><span data-stu-id="1fb2a-137">In this example, replace `f8e85ed8-f66f-4058-b170-3efae8b9c6e5` with the **id** value of the directory role and `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of the user or directory object that you wish to unassign from the directory role.</span></span>

# <a name="http"></a>[<span data-ttu-id="1fb2a-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fb2a-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryRoles/f8e85ed8-f66f-4058-b170-3efae8b9c6e5/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref
```
# <a name="c"></a>[<span data-ttu-id="1fb2a-139">C#</span><span class="sxs-lookup"><span data-stu-id="1fb2a-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fb2a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fb2a-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fb2a-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fb2a-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1fb2a-142">Java</span><span class="sxs-lookup"><span data-stu-id="1fb2a-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1fb2a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fb2a-143">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-directory-role-member-using-role-templateid"></a><span data-ttu-id="1fb2a-144">Exemplo 2: Remover membro da função de diretório usando modelo de funçãoId</span><span class="sxs-lookup"><span data-stu-id="1fb2a-144">Example 2: Remove directory role member using role templateId</span></span>

#### <a name="request"></a><span data-ttu-id="1fb2a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fb2a-145">Request</span></span>

<span data-ttu-id="1fb2a-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fb2a-146">Here is an example of the request.</span></span> <span data-ttu-id="1fb2a-147">Substitua pelo valor de sua roleTemplateId e pelo valor `9f06204d-73c1-4d4c-880a-6edb90606fd8` de `bb165b45-151c-4cf6-9911-cd7188912848` **id** do usuário do objeto directory.</span><span class="sxs-lookup"><span data-stu-id="1fb2a-147">Replace `9f06204d-73c1-4d4c-880a-6edb90606fd8` with the value of your roleTemplateId and `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of your user of directory object.</span></span>


# <a name="http"></a>[<span data-ttu-id="1fb2a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fb2a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_templateId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=9f06204d-73c1-4d4c-880a-6edb90606fd8/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref
```
# <a name="c"></a>[<span data-ttu-id="1fb2a-149">C#</span><span class="sxs-lookup"><span data-stu-id="1fb2a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fb2a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fb2a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fb2a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fb2a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1fb2a-152">Java</span><span class="sxs-lookup"><span data-stu-id="1fb2a-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="1fb2a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fb2a-153">Response</span></span>
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


