---
title: Adicionar membro
description: Adicionar um membro a um grupo do Microsoft 365, de um grupo de segurança ou de um grupo de segurança habilitado para email por meio da propriedade de navegação **members**.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d7272266893579d0524423a7bd968ad56ff7e694
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469000"
---
# <a name="add-member"></a><span data-ttu-id="ba87c-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="ba87c-103">Add member</span></span>

<span data-ttu-id="ba87c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba87c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba87c-105">Adicione um membro a um grupo do Microsoft 365 ou a um grupo de segurança através da propriedade de navegação de **membros**.</span><span class="sxs-lookup"><span data-stu-id="ba87c-105">Add a member to a Microsoft 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="ba87c-106">É possível adicionar usuários, contatos organizacionais, entidades de serviço ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="ba87c-106">You can add users, organizational contacts, service principals or other groups.</span></span> 

> [!IMPORTANT]
> + <span data-ttu-id="ba87c-107">Só é possível adicionar usuários aos grupos do Microsoft 365 e segurança gerenciados pela nuvem.</span><span class="sxs-lookup"><span data-stu-id="ba87c-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>
> + <span data-ttu-id="ba87c-108">Não é possível adicionar grupos de segurança a grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ba87c-108">You cannot add security groups to Microsoft 365 groups.</span></span>
> + <span data-ttu-id="ba87c-109">Não é possível adicionar grupos do Microsoft 365 a grupos de segurança ou a outros grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ba87c-109">You cannot add Microsoft 365 groups to security groups or other Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba87c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba87c-110">Permissions</span></span>

<span data-ttu-id="ba87c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba87c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba87c-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba87c-113">Permission type</span></span>      | <span data-ttu-id="ba87c-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba87c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba87c-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba87c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ba87c-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba87c-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba87c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba87c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba87c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba87c-118">Not supported.</span></span>    |
|<span data-ttu-id="ba87c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba87c-119">Application</span></span> | <span data-ttu-id="ba87c-120">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba87c-120">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba87c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba87c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ba87c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba87c-122">Request headers</span></span>

| <span data-ttu-id="ba87c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba87c-123">Header</span></span>       | <span data-ttu-id="ba87c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ba87c-124">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ba87c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba87c-125">Authorization</span></span>  | <span data-ttu-id="ba87c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba87c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba87c-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="ba87c-128">Content-type</span></span>   | <span data-ttu-id="ba87c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba87c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba87c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba87c-131">Request body</span></span>

<span data-ttu-id="ba87c-132">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) ou [organizational contact](../resources/orgcontact.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="ba87c-132">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="ba87c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba87c-133">Response</span></span>

<span data-ttu-id="ba87c-134">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ba87c-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="ba87c-135">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba87c-135">It does not return anything in the response body.</span></span> <span data-ttu-id="ba87c-136">Esse método retorna um `400 Bad Request` código de resposta quando o objeto já é um membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="ba87c-136">This method returns a `400 Bad Request` response code when the object is already a member of the group.</span></span> <span data-ttu-id="ba87c-137">Esse método retorna um `404 Not Found` código de resposta quando o objeto adicionado não existe.</span><span class="sxs-lookup"><span data-stu-id="ba87c-137">This method returns a `404 Not Found` response code when the object being added doesn't exist.</span></span>

## <a name="examples"></a><span data-ttu-id="ba87c-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ba87c-138">Examples</span></span>

### <a name="example-1-add-a-member-to-a-group"></a><span data-ttu-id="ba87c-139">Exemplo 1: adicionar um membro a um grupo</span><span class="sxs-lookup"><span data-stu-id="ba87c-139">Example 1: Add a member to a group</span></span>

#### <a name="request"></a><span data-ttu-id="ba87c-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba87c-140">Request</span></span>

<span data-ttu-id="ba87c-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba87c-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ba87c-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba87c-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_member_to_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{group-id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="ba87c-143">C#</span><span class="sxs-lookup"><span data-stu-id="ba87c-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-member-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba87c-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba87c-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-member-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba87c-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba87c-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-member-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba87c-146">Java</span><span class="sxs-lookup"><span data-stu-id="ba87c-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-member-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ba87c-147">No corpo da solicitação, forneça uma representação JSON da ID do objeto directoryObject, usuário ou grupo que deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="ba87c-147">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="ba87c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba87c-148">Response</span></span>

<span data-ttu-id="ba87c-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba87c-149">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a><span data-ttu-id="ba87c-150">Exemplo 2: adicionar vários membros a um grupo em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="ba87c-150">Example 2: Add multiple members to a group in a single request</span></span>

<span data-ttu-id="ba87c-151">Esse exemplo mostra como adicionar vários membros a um grupo com suporte vinculado OData em uma operação PATCH.</span><span class="sxs-lookup"><span data-stu-id="ba87c-151">This example shows how to add multiple members to a group with OData bind support in a PATCH operation.</span></span> <span data-ttu-id="ba87c-152">Observe que é possível adicionar até 20 membros em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba87c-152">Note that up to 20 members can be added in a single request.</span></span> <span data-ttu-id="ba87c-153">Não há suporte para a operação POST.</span><span class="sxs-lookup"><span data-stu-id="ba87c-153">The POST operation is not supported.</span></span> <span data-ttu-id="ba87c-154">Se houver uma condição de erro no corpo da solicitação, nenhum membro será adicionado e o código de resposta apropriado será retornado.</span><span class="sxs-lookup"><span data-stu-id="ba87c-154">If an error condition exists in the request body, no members are added and the appropriate response code is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="ba87c-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba87c-155">Request</span></span>

<span data-ttu-id="ba87c-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba87c-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ba87c-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba87c-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_multiple_members_to_group"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{group-id}
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
# <a name="c"></a>[<span data-ttu-id="ba87c-158">C#</span><span class="sxs-lookup"><span data-stu-id="ba87c-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-multiple-members-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba87c-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba87c-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-multiple-members-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba87c-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba87c-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-multiple-members-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba87c-161">Java</span><span class="sxs-lookup"><span data-stu-id="ba87c-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-multiple-members-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ba87c-162">No corpo da solicitação, forneça uma representação JSON da ID do objeto directoryObject, usuário ou grupo que deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="ba87c-162">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="ba87c-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba87c-163">Response</span></span>
<span data-ttu-id="ba87c-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba87c-164">The following is an example of the response.</span></span>

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

