---
title: Adicionar membro da função de diretório
description: Crie um novo membro de função de diretório.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0385ad02b854753e9b88e103a14b68aebd290497
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436719"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="e9f63-103">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="e9f63-103">Add directory role member</span></span>

<span data-ttu-id="e9f63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9f63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9f63-105">Crie um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="e9f63-105">Create a new directory role member.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9f63-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9f63-106">Permissions</span></span>
<span data-ttu-id="e9f63-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9f63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9f63-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9f63-109">Permission type</span></span>      | <span data-ttu-id="e9f63-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9f63-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9f63-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9f63-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e9f63-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e9f63-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e9f63-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9f63-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9f63-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9f63-114">Not supported.</span></span>    |
|<span data-ttu-id="e9f63-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9f63-115">Application</span></span> | <span data-ttu-id="e9f63-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="e9f63-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9f63-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9f63-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e9f63-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9f63-118">Request headers</span></span>
| <span data-ttu-id="e9f63-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e9f63-119">Name</span></span>       | <span data-ttu-id="e9f63-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9f63-120">Type</span></span> | <span data-ttu-id="e9f63-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9f63-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e9f63-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9f63-122">Authorization</span></span>  | <span data-ttu-id="e9f63-123">string</span><span class="sxs-lookup"><span data-stu-id="e9f63-123">string</span></span>  | <span data-ttu-id="e9f63-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9f63-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9f63-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="e9f63-126">Content-type</span></span> | <span data-ttu-id="e9f63-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9f63-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9f63-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9f63-129">Request body</span></span>
<span data-ttu-id="e9f63-130">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e9f63-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e9f63-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9f63-131">Response</span></span>

<span data-ttu-id="e9f63-132">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9f63-132">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9f63-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e9f63-133">Examples</span></span>

### <a name="example-1-assign-a-built-in-role-to-a-user"></a><span data-ttu-id="e9f63-134">Exemplo 1: Atribuir uma função interna a um usuário</span><span class="sxs-lookup"><span data-stu-id="e9f63-134">Example 1: Assign a built-in role to a user</span></span>
#### <a name="request"></a><span data-ttu-id="e9f63-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9f63-135">Request</span></span>
<span data-ttu-id="e9f63-136">O exemplo a seguir atribui uma função interna a um usuário.</span><span class="sxs-lookup"><span data-stu-id="e9f63-136">The following example assigns a built-in role to a user.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9f63-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9f63-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id":"https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2"
}
```
# <a name="javascript"></a>[<span data-ttu-id="e9f63-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9f63-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="e9f63-139">C#</span><span class="sxs-lookup"><span data-stu-id="e9f63-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9f63-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9f63-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9f63-141">Java</span><span class="sxs-lookup"><span data-stu-id="e9f63-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e9f63-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9f63-142">Response</span></span>
<span data-ttu-id="e9f63-143">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9f63-143">The following example shows the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No content
```

### <a name="example-2-assign-a-built-in-role-to-a-group"></a><span data-ttu-id="e9f63-144">Exemplo 2: Atribuir uma função embutida a um grupo</span><span class="sxs-lookup"><span data-stu-id="e9f63-144">Example 2: Assign a built-in role to a group</span></span>
#### <a name="request"></a><span data-ttu-id="e9f63-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9f63-145">Request</span></span>
<span data-ttu-id="e9f63-146">Você pode usar um conjunto de recursos específico como usuários ou grupos no corpo da solicitação ou pode usar **directoryObjects genéricos.**</span><span class="sxs-lookup"><span data-stu-id="e9f63-146">You can use a specific resource set like users or groups in the request body, or you can use generic **directoryObjects**.</span></span> <span data-ttu-id="e9f63-147">Este exemplo mostra como você pode usar **directoryObjects**.</span><span class="sxs-lookup"><span data-stu-id="e9f63-147">This example shows how you can use **directoryObjects**.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id":"https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc"
}
```

#### <a name="response"></a><span data-ttu-id="e9f63-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9f63-148">Response</span></span>
<span data-ttu-id="e9f63-149">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9f63-149">The following example shows the response.</span></span> 

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


