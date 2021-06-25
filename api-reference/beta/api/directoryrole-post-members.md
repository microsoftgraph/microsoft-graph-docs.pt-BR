---
title: Adicionar membro da função de diretório
description: Crie um novo membro de função de diretório.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 135640887f43952a83f93b1b4267645a228383c4
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118494"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="5c0c9-103">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="5c0c9-103">Add directory role member</span></span>

<span data-ttu-id="5c0c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c0c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c0c9-105">Crie um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="5c0c9-105">Create a new directory role member.</span></span>

<span data-ttu-id="5c0c9-106">Você pode usar a ID do objeto e a ID do modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="5c0c9-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="5c0c9-107">A ID do modelo de uma função embutida é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5c0c9-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="5c0c9-108">Para obter detalhes, consulte [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="5c0c9-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="5c0c9-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c0c9-109">Permissions</span></span>
<span data-ttu-id="5c0c9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c0c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c0c9-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c0c9-112">Permission type</span></span>      | <span data-ttu-id="5c0c9-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c0c9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c0c9-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c0c9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5c0c9-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5c0c9-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5c0c9-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c0c9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c0c9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c0c9-117">Not supported.</span></span>    |
|<span data-ttu-id="5c0c9-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c0c9-118">Application</span></span> | <span data-ttu-id="5c0c9-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="5c0c9-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c0c9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c0c9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{role-id}/members/$ref
POST /directoryRoles/roleTemplateId={roleTemplateId}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5c0c9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c0c9-121">Request headers</span></span>
| <span data-ttu-id="5c0c9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5c0c9-122">Name</span></span>       | <span data-ttu-id="5c0c9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c0c9-123">Type</span></span> | <span data-ttu-id="5c0c9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c0c9-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5c0c9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c0c9-125">Authorization</span></span>  | <span data-ttu-id="5c0c9-126">string</span><span class="sxs-lookup"><span data-stu-id="5c0c9-126">string</span></span>  | <span data-ttu-id="5c0c9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c0c9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c0c9-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="5c0c9-129">Content-type</span></span> | <span data-ttu-id="5c0c9-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c0c9-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c0c9-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c0c9-132">Request body</span></span>
<span data-ttu-id="5c0c9-133">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="5c0c9-133">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5c0c9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c0c9-134">Response</span></span>

<span data-ttu-id="5c0c9-135">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c0c9-135">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c0c9-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5c0c9-136">Examples</span></span>

### <a name="example-1-assign-a-built-in-role-to-a-user"></a><span data-ttu-id="5c0c9-137">Exemplo 1: Atribuir uma função interna a um usuário</span><span class="sxs-lookup"><span data-stu-id="5c0c9-137">Example 1: Assign a built-in role to a user</span></span>
#### <a name="request"></a><span data-ttu-id="5c0c9-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c0c9-138">Request</span></span>
<span data-ttu-id="5c0c9-139">O exemplo a seguir atribui uma função interna a um usuário.</span><span class="sxs-lookup"><span data-stu-id="5c0c9-139">The following example assigns a built-in role to a user.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c0c9-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c0c9-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_1"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id":"https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2"
}
```
# <a name="javascript"></a>[<span data-ttu-id="5c0c9-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c0c9-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="5c0c9-142">C#</span><span class="sxs-lookup"><span data-stu-id="5c0c9-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c0c9-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c0c9-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c0c9-144">Java</span><span class="sxs-lookup"><span data-stu-id="5c0c9-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5c0c9-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c0c9-145">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No content
```

### <a name="example-2-assign-a-built-in-role-to-a-group"></a><span data-ttu-id="5c0c9-146">Exemplo 2: Atribuir uma função embutida a um grupo</span><span class="sxs-lookup"><span data-stu-id="5c0c9-146">Example 2: Assign a built-in role to a group</span></span>
#### <a name="request"></a><span data-ttu-id="5c0c9-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c0c9-147">Request</span></span>
<span data-ttu-id="5c0c9-148">Você pode usar um conjunto de recursos específico como usuários ou grupos no corpo da solicitação ou pode usar **directoryObjects genéricos.**</span><span class="sxs-lookup"><span data-stu-id="5c0c9-148">You can use a specific resource set like users or groups in the request body, or you can use generic **directoryObjects**.</span></span> <span data-ttu-id="5c0c9-149">Este exemplo mostra como você pode usar **directoryObjects**.</span><span class="sxs-lookup"><span data-stu-id="5c0c9-149">This example shows how you can use **directoryObjects**.</span></span>


# <a name="http"></a>[<span data-ttu-id="5c0c9-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c0c9-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_2"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id":"https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc"
}
```
# <a name="c"></a>[<span data-ttu-id="5c0c9-151">C#</span><span class="sxs-lookup"><span data-stu-id="5c0c9-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c0c9-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c0c9-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c0c9-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c0c9-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c0c9-154">Java</span><span class="sxs-lookup"><span data-stu-id="5c0c9-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5c0c9-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c0c9-155">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No content
```

### <a name="example-3-add-a-new-member-to-a-directory-role-using-roletemplateid"></a><span data-ttu-id="5c0c9-156">Exemplo 3: Adicionar um novo membro a uma função de diretório usando roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="5c0c9-156">Example 3: Add a new member to a directory role using roleTemplateId</span></span>
#### <a name="request"></a><span data-ttu-id="5c0c9-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c0c9-157">Request</span></span>
<span data-ttu-id="5c0c9-158">Nesta solicitação, substitua pelo valor da `88d8e3e3-8f55-4a1e-953a-9b9898b8876b` **funçãoTemplateId** para a função de diretório que você deseja atribuir ao usuário ou objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="5c0c9-158">In this request, replace `88d8e3e3-8f55-4a1e-953a-9b9898b8876b` with the value of the **roleTemplateId** for the directory role you wish to assign to the user or directory object.</span></span> <span data-ttu-id="5c0c9-159">Substitua `bb165b45-151c-4cf6-9911-cd7188912848` pelo valor de **id** do seu objeto de diretório ou usuário.</span><span class="sxs-lookup"><span data-stu-id="5c0c9-159">Replace `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of your user or directory object.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5c0c9-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c0c9-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_2_templateId"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/bb165b45-151c-4cf6-9911-cd7188912848"
}
```
# <a name="c"></a>[<span data-ttu-id="5c0c9-161">C#</span><span class="sxs-lookup"><span data-stu-id="5c0c9-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-2-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c0c9-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c0c9-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-2-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c0c9-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c0c9-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-2-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c0c9-164">Java</span><span class="sxs-lookup"><span data-stu-id="5c0c9-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-2-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5c0c9-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c0c9-165">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


