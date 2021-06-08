---
title: Adicionar membro da função de diretório
description: Use esta API para criar um novo membro de função de diretório.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 350a68a06c94782951163007751819c58e8113b1
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787636"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="77315-103">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="77315-103">Add directory role member</span></span>

<span data-ttu-id="77315-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77315-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77315-105">Use esta API para criar um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="77315-105">Use this API to create a new directory role member.</span></span>

> [!Note]
> <span data-ttu-id="77315-106">Você pode usar a ID do objeto e a ID do modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="77315-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="77315-107">A ID do modelo de uma função embutida é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="77315-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="77315-108">Para obter detalhes, consulte [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="77315-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="77315-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="77315-109">Permissions</span></span>
<span data-ttu-id="77315-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77315-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77315-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77315-112">Permission type</span></span>      | <span data-ttu-id="77315-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77315-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77315-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77315-114">Delegated (work or school account)</span></span> | <span data-ttu-id="77315-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="77315-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="77315-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77315-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77315-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77315-117">Not supported.</span></span>    |
|<span data-ttu-id="77315-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77315-118">Application</span></span> | <span data-ttu-id="77315-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="77315-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="77315-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77315-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="77315-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77315-121">Request headers</span></span>
| <span data-ttu-id="77315-122">Nome</span><span class="sxs-lookup"><span data-stu-id="77315-122">Name</span></span>       | <span data-ttu-id="77315-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="77315-123">Type</span></span> | <span data-ttu-id="77315-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="77315-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="77315-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="77315-125">Authorization</span></span>  | <span data-ttu-id="77315-126">string</span><span class="sxs-lookup"><span data-stu-id="77315-126">string</span></span>  | <span data-ttu-id="77315-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77315-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77315-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="77315-129">Content-Type</span></span>  | <span data-ttu-id="77315-130">string</span><span class="sxs-lookup"><span data-stu-id="77315-130">string</span></span>  | <span data-ttu-id="77315-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77315-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="77315-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77315-133">Request body</span></span>
<span data-ttu-id="77315-134">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="77315-134">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="77315-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="77315-135">Response</span></span>

<span data-ttu-id="77315-136">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="77315-136">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="77315-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="77315-137">Examples</span></span>

### <a name="example-1-add-a-new-member-to-a-directory-role-using-role-objectid"></a><span data-ttu-id="77315-138">Exemplo 1: Adicionar um novo membro a uma função de diretório usando objectId de função</span><span class="sxs-lookup"><span data-stu-id="77315-138">Example 1: Add a new member to a directory role using role objectId</span></span>

##### <a name="request"></a><span data-ttu-id="77315-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77315-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="77315-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="77315-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_objectId"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{role-objectId}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{user-id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="77315-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77315-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77315-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77315-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="77315-143">C#</span><span class="sxs-lookup"><span data-stu-id="77315-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77315-144">Java</span><span class="sxs-lookup"><span data-stu-id="77315-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="77315-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="77315-145">Response</span></span>
><span data-ttu-id="77315-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="77315-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

### <a name="example-2-add-a-new-member-to-a-directory-role-using-role-templateid"></a><span data-ttu-id="77315-147">Exemplo 2: Adicionar um novo membro a uma função de diretório usando role templateId</span><span class="sxs-lookup"><span data-stu-id="77315-147">Example 2: Add a new member to a directory role using role templateId</span></span>

##### <a name="request"></a><span data-ttu-id="77315-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77315-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="77315-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="77315-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_templateId"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId={role-templateId}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{user-id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="77315-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77315-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77315-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77315-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="77315-152">C#</span><span class="sxs-lookup"><span data-stu-id="77315-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77315-153">Java</span><span class="sxs-lookup"><span data-stu-id="77315-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="77315-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="77315-154">Response</span></span>
><span data-ttu-id="77315-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="77315-155">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

