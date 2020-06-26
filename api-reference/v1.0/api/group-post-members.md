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
# <a name="add-member"></a><span data-ttu-id="62440-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="62440-103">Add member</span></span>

<span data-ttu-id="62440-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62440-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62440-105">Adicionar um membro a um grupo do Microsoft 365 ou um grupo de segurança por meio da propriedade de navegação **Members** .</span><span class="sxs-lookup"><span data-stu-id="62440-105">Add a member to a Microsoft 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="62440-106">Você pode adicionar usuários, contatos organizacionais, entidades de serviço ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="62440-106">You can add users, organizational contacts, service principals or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="62440-107">Você só pode adicionar usuários aos grupos segurança e Microsoft 365 gerenciados por meio da nuvem.</span><span class="sxs-lookup"><span data-stu-id="62440-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="62440-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="62440-108">Permissions</span></span>
<span data-ttu-id="62440-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="62440-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="62440-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62440-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62440-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62440-111">Permission type</span></span>      | <span data-ttu-id="62440-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62440-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62440-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62440-113">Delegated (work or school account)</span></span> | <span data-ttu-id="62440-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62440-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="62440-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62440-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62440-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62440-116">Not supported.</span></span>    |
|<span data-ttu-id="62440-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62440-117">Application</span></span> | <span data-ttu-id="62440-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62440-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62440-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62440-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="62440-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62440-120">Request headers</span></span>
| <span data-ttu-id="62440-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62440-121">Header</span></span>       | <span data-ttu-id="62440-122">Valor</span><span class="sxs-lookup"><span data-stu-id="62440-122">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="62440-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="62440-123">Authorization</span></span>  | <span data-ttu-id="62440-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="62440-124">Bearer {token}.</span></span> <span data-ttu-id="62440-125">Required.</span><span class="sxs-lookup"><span data-stu-id="62440-125">Required.</span></span> |
| <span data-ttu-id="62440-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="62440-126">Content-type</span></span>   | <span data-ttu-id="62440-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="62440-127">application/json.</span></span> <span data-ttu-id="62440-128">Required.</span><span class="sxs-lookup"><span data-stu-id="62440-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62440-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62440-129">Request body</span></span>
<span data-ttu-id="62440-130">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) ou [organizational contact](../resources/orgcontact.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="62440-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="62440-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="62440-131">Response</span></span>
<span data-ttu-id="62440-132">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="62440-132">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="62440-133">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="62440-133">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62440-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="62440-134">Examples</span></span>
### <a name="example-1-add-a-member-to-a-group"></a><span data-ttu-id="62440-135">Exemplo 1: adicionar um membro a um grupo</span><span class="sxs-lookup"><span data-stu-id="62440-135">Example 1: Add a member to a group</span></span>
#### <a name="request"></a><span data-ttu-id="62440-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62440-136">Request</span></span>
<span data-ttu-id="62440-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="62440-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="62440-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="62440-138">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="62440-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62440-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62440-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62440-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="62440-141">C#</span><span class="sxs-lookup"><span data-stu-id="62440-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62440-142">Java</span><span class="sxs-lookup"><span data-stu-id="62440-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="62440-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="62440-143">Response</span></span>
<span data-ttu-id="62440-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="62440-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a><span data-ttu-id="62440-145">Exemplo 2: adicionar vários membros a um grupo em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="62440-145">Example 2: Add multiple members to a group in a single request</span></span>
<span data-ttu-id="62440-146">Este exemplo mostra como adicionar vários membros a um grupo com suporte a BIND OData em uma operação PATCH.</span><span class="sxs-lookup"><span data-stu-id="62440-146">This example shows how to add multiple members to a group with OData bind support in a PATCH operation.</span></span> <span data-ttu-id="62440-147">Observe que até 20 membros podem ser adicionados em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="62440-147">Note that up to 20 members can be added in a single request.</span></span> <span data-ttu-id="62440-148">A operação POST não é suportada.</span><span class="sxs-lookup"><span data-stu-id="62440-148">The POST operation is not supported.</span></span>
#### <a name="request"></a><span data-ttu-id="62440-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62440-149">Request</span></span>
<span data-ttu-id="62440-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="62440-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="62440-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="62440-151">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="62440-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62440-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62440-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62440-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="62440-154">C#</span><span class="sxs-lookup"><span data-stu-id="62440-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62440-155">Java</span><span class="sxs-lookup"><span data-stu-id="62440-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="62440-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="62440-156">Response</span></span>
<span data-ttu-id="62440-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="62440-157">The following is an example of the response.</span></span>

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
