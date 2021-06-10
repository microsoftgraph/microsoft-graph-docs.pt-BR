---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 42932d1d058fa7970d444376553a0ae683dc9e2e
ms.sourcegitcommit: 9eeb056f311044aaa40654cdb3ae5ae61f1c4d04
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2021
ms.locfileid: "52854254"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="066e2-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="066e2-103">Remove directory role member</span></span>

<span data-ttu-id="066e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="066e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="066e2-105">Remover um membro de um [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="066e2-105">Remove a member from a [directoryRole](../resources/directoryrole.md).</span></span>

<span data-ttu-id="066e2-106">Você pode usar a ID do objeto e a ID do modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="066e2-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="066e2-107">A ID do modelo de uma função embutida é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="066e2-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="066e2-108">Para obter detalhes, consulte [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="066e2-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="066e2-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="066e2-109">Permissions</span></span>

<span data-ttu-id="066e2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="066e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="066e2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="066e2-112">Permission type</span></span>      | <span data-ttu-id="066e2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="066e2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="066e2-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="066e2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="066e2-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="066e2-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="066e2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="066e2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="066e2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="066e2-117">Not supported.</span></span>    |
|<span data-ttu-id="066e2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="066e2-118">Application</span></span> | <span data-ttu-id="066e2-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="066e2-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="066e2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="066e2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{role-objectId}/members/{id}/$ref
DELETE /directoryRoles/roleTemplateId={role-templateId}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="066e2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="066e2-121">Request headers</span></span>

| <span data-ttu-id="066e2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="066e2-122">Name</span></span>       | <span data-ttu-id="066e2-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="066e2-123">Type</span></span> | <span data-ttu-id="066e2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="066e2-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="066e2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="066e2-125">Authorization</span></span>  | <span data-ttu-id="066e2-126">string</span><span class="sxs-lookup"><span data-stu-id="066e2-126">string</span></span>  | <span data-ttu-id="066e2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="066e2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="066e2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="066e2-129">Request body</span></span>

<span data-ttu-id="066e2-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="066e2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="066e2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="066e2-131">Response</span></span>

<span data-ttu-id="066e2-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="066e2-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="066e2-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="066e2-134">Examples</span></span>

### <a name="example-1-remove-directory-role-member-using-role-objectid"></a><span data-ttu-id="066e2-135">Exemplo 1: Remover membro da função de diretório usando objectId de função</span><span class="sxs-lookup"><span data-stu-id="066e2-135">Example 1: Remove directory role member using role objectId</span></span>

#### <a name="request"></a><span data-ttu-id="066e2-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="066e2-136">Request</span></span>

<span data-ttu-id="066e2-137">Neste exemplo, substitua pelo valor de id da função de diretório e pelo valor de id do usuário ou objeto de diretório que você deseja `f8e85ed8-f66f-4058-b170-3efae8b9c6e5` desasinalhar da função de  `bb165b45-151c-4cf6-9911-cd7188912848` diretório. </span><span class="sxs-lookup"><span data-stu-id="066e2-137">In this example, replace `f8e85ed8-f66f-4058-b170-3efae8b9c6e5` with the **id** value of the directory role and `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of the user or directory object that you wish to unassign from the directory role.</span></span>

# <a name="http"></a>[<span data-ttu-id="066e2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="066e2-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_objectId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/f8e85ed8-f66f-4058-b170-3efae8b9c6e5/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref
```
# <a name="c"></a>[<span data-ttu-id="066e2-139">C#</span><span class="sxs-lookup"><span data-stu-id="066e2-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="066e2-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="066e2-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="066e2-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="066e2-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="066e2-142">Java</span><span class="sxs-lookup"><span data-stu-id="066e2-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="066e2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="066e2-143">Response</span></span>

<span data-ttu-id="066e2-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="066e2-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-directory-role-member-using-role-templateid"></a><span data-ttu-id="066e2-145">Exemplo 2: Remover membro da função de diretório usando modelo de funçãoId</span><span class="sxs-lookup"><span data-stu-id="066e2-145">Example 2: Remove directory role member using role templateId</span></span>

#### <a name="request"></a><span data-ttu-id="066e2-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="066e2-146">Request</span></span>

<span data-ttu-id="066e2-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="066e2-147">Here is an example of the request.</span></span> <span data-ttu-id="066e2-148">Substitua pelo valor de sua roleTemplateId e pelo valor `9f06204d-73c1-4d4c-880a-6edb90606fd8` de `bb165b45-151c-4cf6-9911-cd7188912848` **id** do usuário do objeto directory.</span><span class="sxs-lookup"><span data-stu-id="066e2-148">Replace `9f06204d-73c1-4d4c-880a-6edb90606fd8` with the value of your roleTemplateId and `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of your user of directory object.</span></span>

# <a name="http"></a>[<span data-ttu-id="066e2-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="066e2-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_templateId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=9f06204d-73c1-4d4c-880a-6edb90606fd8/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref
```
# <a name="c"></a>[<span data-ttu-id="066e2-150">C#</span><span class="sxs-lookup"><span data-stu-id="066e2-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="066e2-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="066e2-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="066e2-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="066e2-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="066e2-153">Java</span><span class="sxs-lookup"><span data-stu-id="066e2-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="066e2-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="066e2-154">Response</span></span>

<span data-ttu-id="066e2-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="066e2-155">Here is an example of the response.</span></span> 
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

