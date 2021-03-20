---
title: Adicionar membro da função de diretório
description: Crie um novo membro de função de diretório.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 843eb3d27e8765d0d95fb8ee86c11b0f1deae5bb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946566"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="c090d-103">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="c090d-103">Add directory role member</span></span>

<span data-ttu-id="c090d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c090d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c090d-105">Crie um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="c090d-105">Create a new directory role member.</span></span>
## <a name="permissions"></a><span data-ttu-id="c090d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c090d-106">Permissions</span></span>
<span data-ttu-id="c090d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c090d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c090d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c090d-109">Permission type</span></span>      | <span data-ttu-id="c090d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c090d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c090d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c090d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c090d-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c090d-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c090d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c090d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c090d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c090d-114">Not supported.</span></span>    |
|<span data-ttu-id="c090d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c090d-115">Application</span></span> | <span data-ttu-id="c090d-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="c090d-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="c090d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c090d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c090d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c090d-118">Request headers</span></span>
| <span data-ttu-id="c090d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c090d-119">Name</span></span>       | <span data-ttu-id="c090d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c090d-120">Type</span></span> | <span data-ttu-id="c090d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c090d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c090d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c090d-122">Authorization</span></span>  | <span data-ttu-id="c090d-123">string</span><span class="sxs-lookup"><span data-stu-id="c090d-123">string</span></span>  | <span data-ttu-id="c090d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c090d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c090d-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="c090d-126">Content-type</span></span> | <span data-ttu-id="c090d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c090d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c090d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c090d-129">Request body</span></span>
<span data-ttu-id="c090d-130">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="c090d-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c090d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c090d-131">Response</span></span>

<span data-ttu-id="c090d-132">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c090d-132">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c090d-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c090d-133">Examples</span></span>

### <a name="example-1-assign-a-built-in-role-to-a-user"></a><span data-ttu-id="c090d-134">Exemplo 1: Atribuir uma função interna a um usuário</span><span class="sxs-lookup"><span data-stu-id="c090d-134">Example 1: Assign a built-in role to a user</span></span>
#### <a name="request"></a><span data-ttu-id="c090d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c090d-135">Request</span></span>
<span data-ttu-id="c090d-136">O exemplo a seguir atribui uma função interna a um usuário.</span><span class="sxs-lookup"><span data-stu-id="c090d-136">The following example assigns a built-in role to a user.</span></span>

# <a name="http"></a>[<span data-ttu-id="c090d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c090d-137">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="c090d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c090d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c090d-139">C#</span><span class="sxs-lookup"><span data-stu-id="c090d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c090d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c090d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c090d-141">Java</span><span class="sxs-lookup"><span data-stu-id="c090d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c090d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c090d-142">Response</span></span>
<span data-ttu-id="c090d-143">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="c090d-143">The following example shows the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No content
```

### <a name="example-2-assign-a-built-in-role-to-a-group"></a><span data-ttu-id="c090d-144">Exemplo 2: Atribuir uma função embutida a um grupo</span><span class="sxs-lookup"><span data-stu-id="c090d-144">Example 2: Assign a built-in role to a group</span></span>
#### <a name="request"></a><span data-ttu-id="c090d-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c090d-145">Request</span></span>
<span data-ttu-id="c090d-146">Você pode usar um conjunto de recursos específico como usuários ou grupos no corpo da solicitação ou pode usar **directoryObjects genéricos.**</span><span class="sxs-lookup"><span data-stu-id="c090d-146">You can use a specific resource set like users or groups in the request body, or you can use generic **directoryObjects**.</span></span> <span data-ttu-id="c090d-147">Este exemplo mostra como você pode usar **directoryObjects**.</span><span class="sxs-lookup"><span data-stu-id="c090d-147">This example shows how you can use **directoryObjects**.</span></span>


# <a name="http"></a>[<span data-ttu-id="c090d-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="c090d-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c090d-149">C#</span><span class="sxs-lookup"><span data-stu-id="c090d-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c090d-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c090d-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c090d-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c090d-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c090d-152">Java</span><span class="sxs-lookup"><span data-stu-id="c090d-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c090d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c090d-153">Response</span></span>
<span data-ttu-id="c090d-154">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="c090d-154">The following example shows the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
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


