---
title: Adicionar membro
description: Adicionar um membro a um grupo do Microsoft 365, um grupo de segurança ou um grupo de segurança habilitado para email através da propriedade de navegação **Members** .
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0388d13d0e50c6ffcc415503a75afb8af56fa14f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897145"
---
# <a name="add-member"></a><span data-ttu-id="9d8e2-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="9d8e2-103">Add member</span></span>

<span data-ttu-id="9d8e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d8e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d8e2-105">Adicionar um membro a um grupo do Microsoft 365 ou um grupo de segurança por meio da propriedade de navegação **Members** .</span><span class="sxs-lookup"><span data-stu-id="9d8e2-105">Add a member to a Microsoft 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="9d8e2-106">Você pode adicionar usuários, contatos organizacionais, entidades de serviço ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-106">You can add users, organizational contacts, service principals or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="9d8e2-107">Você só pode adicionar usuários aos grupos segurança e Microsoft 365 gerenciados por meio da nuvem.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d8e2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d8e2-108">Permissions</span></span>
<span data-ttu-id="9d8e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d8e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d8e2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d8e2-111">Permission type</span></span>      | <span data-ttu-id="9d8e2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d8e2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d8e2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d8e2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9d8e2-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d8e2-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d8e2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d8e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d8e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-116">Not supported.</span></span>    |
|<span data-ttu-id="9d8e2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d8e2-117">Application</span></span> | <span data-ttu-id="9d8e2-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d8e2-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d8e2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d8e2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9d8e2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d8e2-120">Request headers</span></span>
| <span data-ttu-id="9d8e2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9d8e2-121">Header</span></span>       | <span data-ttu-id="9d8e2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9d8e2-122">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="9d8e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d8e2-123">Authorization</span></span>  | <span data-ttu-id="9d8e2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9d8e2-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="9d8e2-126">Content-type</span></span>   | <span data-ttu-id="9d8e2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d8e2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d8e2-129">Request body</span></span>
<span data-ttu-id="9d8e2-130">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) ou [organizational contact](../resources/orgcontact.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="9d8e2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d8e2-131">Response</span></span>
<span data-ttu-id="9d8e2-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d8e2-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9d8e2-134">Examples</span></span>
### <a name="example-1-add-a-member-to-a-group"></a><span data-ttu-id="9d8e2-135">Exemplo 1: adicionar um membro a um grupo</span><span class="sxs-lookup"><span data-stu-id="9d8e2-135">Example 1: Add a member to a group</span></span>
#### <a name="request"></a><span data-ttu-id="9d8e2-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d8e2-136">Request</span></span>
<span data-ttu-id="9d8e2-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d8e2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d8e2-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_member_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="9d8e2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d8e2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d8e2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d8e2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="9d8e2-141">C#</span><span class="sxs-lookup"><span data-stu-id="9d8e2-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d8e2-142">Java</span><span class="sxs-lookup"><span data-stu-id="9d8e2-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9d8e2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d8e2-143">Response</span></span>
<span data-ttu-id="9d8e2-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a><span data-ttu-id="9d8e2-145">Exemplo 2: adicionar vários membros a um grupo em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="9d8e2-145">Example 2: Add multiple members to a group in a single request</span></span>
<span data-ttu-id="9d8e2-146">Este exemplo mostra como adicionar vários membros a um grupo com suporte a BIND OData em uma operação PATCH.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-146">This example shows how to add multiple members to a group with OData bind support in a PATCH operation.</span></span> <span data-ttu-id="9d8e2-147">Observe que até 20 membros podem ser adicionados em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-147">Note that up to 20 members can be added in a single request.</span></span> <span data-ttu-id="9d8e2-148">A operação POST não é suportada.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-148">The POST operation is not supported.</span></span>
#### <a name="request"></a><span data-ttu-id="9d8e2-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d8e2-149">Request</span></span>
<span data-ttu-id="9d8e2-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d8e2-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d8e2-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_member_from_group"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
Content-type: application/json
Content-length: 30

{
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="9d8e2-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d8e2-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d8e2-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d8e2-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="9d8e2-154">C#</span><span class="sxs-lookup"><span data-stu-id="9d8e2-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d8e2-155">Java</span><span class="sxs-lookup"><span data-stu-id="9d8e2-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9d8e2-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d8e2-156">Response</span></span>
<span data-ttu-id="9d8e2-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d8e2-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
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
