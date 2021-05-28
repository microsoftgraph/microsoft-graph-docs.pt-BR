---
title: Adicionar membro
description: Adicionar um membro a um grupo do Microsoft 365, de um grupo de segurança ou de um grupo de segurança habilitado para email por meio da propriedade de navegação **members**.
localization_priority: Priority
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a9337c18b25e37711e9e7d9ec14d9ee65eccac39
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681974"
---
# <a name="add-member"></a><span data-ttu-id="df4fb-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="df4fb-103">Add member</span></span>

<span data-ttu-id="df4fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df4fb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df4fb-105">Adicione um membro a um grupo do Microsoft 365 ou a um grupo de segurança através da propriedade de navegação de **membros**.</span><span class="sxs-lookup"><span data-stu-id="df4fb-105">Add a member to a Microsoft 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="df4fb-106">É possível adicionar usuários, contatos organizacionais, entidades de serviço ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="df4fb-106">You can add users, organizational contacts, service principals or other groups.</span></span> 

> [!IMPORTANT]
> + <span data-ttu-id="df4fb-107">Só é possível adicionar usuários aos grupos do Microsoft 365 e segurança gerenciados pela nuvem.</span><span class="sxs-lookup"><span data-stu-id="df4fb-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>
> + <span data-ttu-id="df4fb-108">Não é possível adicionar grupos de segurança a grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="df4fb-108">You cannot add security groups to Microsoft 365 groups.</span></span>
> + <span data-ttu-id="df4fb-109">Não é possível adicionar grupos do Microsoft 365 a grupos de segurança ou a outros grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="df4fb-109">You cannot add Microsoft 365 groups to security groups or other Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="df4fb-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="df4fb-110">Permissions</span></span>

<span data-ttu-id="df4fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df4fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df4fb-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df4fb-113">Permission type</span></span>      | <span data-ttu-id="df4fb-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df4fb-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df4fb-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df4fb-115">Delegated (work or school account)</span></span> | <span data-ttu-id="df4fb-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="df4fb-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="df4fb-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df4fb-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df4fb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df4fb-118">Not supported.</span></span>    |
|<span data-ttu-id="df4fb-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df4fb-119">Application</span></span> | <span data-ttu-id="df4fb-120">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df4fb-120">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df4fb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df4fb-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="df4fb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df4fb-122">Request headers</span></span>

| <span data-ttu-id="df4fb-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df4fb-123">Header</span></span>       | <span data-ttu-id="df4fb-124">Valor</span><span class="sxs-lookup"><span data-stu-id="df4fb-124">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="df4fb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="df4fb-125">Authorization</span></span>  | <span data-ttu-id="df4fb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df4fb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="df4fb-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="df4fb-128">Content-type</span></span>   | <span data-ttu-id="df4fb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df4fb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df4fb-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df4fb-131">Request body</span></span>

<span data-ttu-id="df4fb-132">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) ou [organizational contact](../resources/orgcontact.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="df4fb-132">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="df4fb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="df4fb-133">Response</span></span>

<span data-ttu-id="df4fb-134">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="df4fb-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="df4fb-135">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df4fb-135">It does not return anything in the response body.</span></span> <span data-ttu-id="df4fb-136">Esse método retorna um `400 Bad Request` código de resposta quando o objeto já é um membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="df4fb-136">This method returns a `400 Bad Request` response code when the object is already a member of the group.</span></span> <span data-ttu-id="df4fb-137">Esse método retorna um `404 Not Found` código de resposta quando o objeto adicionado não existe.</span><span class="sxs-lookup"><span data-stu-id="df4fb-137">This method returns a `404 Not Found` response code when the object being added doesn't exist.</span></span>

## <a name="examples"></a><span data-ttu-id="df4fb-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="df4fb-138">Examples</span></span>

### <a name="example-1-add-a-member-to-a-group"></a><span data-ttu-id="df4fb-139">Exemplo 1: adicionar um membro a um grupo</span><span class="sxs-lookup"><span data-stu-id="df4fb-139">Example 1: Add a member to a group</span></span>

#### <a name="request"></a><span data-ttu-id="df4fb-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df4fb-140">Request</span></span>

<span data-ttu-id="df4fb-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df4fb-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="df4fb-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="df4fb-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="df4fb-143">C#</span><span class="sxs-lookup"><span data-stu-id="df4fb-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-member-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df4fb-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df4fb-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-member-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df4fb-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df4fb-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-member-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df4fb-146">Java</span><span class="sxs-lookup"><span data-stu-id="df4fb-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-member-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="df4fb-147">No corpo da solicitação, forneça uma representação JSON da ID do objeto directoryObject, usuário ou grupo que deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="df4fb-147">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="df4fb-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="df4fb-148">Response</span></span>

<span data-ttu-id="df4fb-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df4fb-149">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a><span data-ttu-id="df4fb-150">Exemplo 2: adicionar vários membros a um grupo em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="df4fb-150">Example 2: Add multiple members to a group in a single request</span></span>

<span data-ttu-id="df4fb-151">Esse exemplo mostra como adicionar vários membros a um grupo com suporte vinculado OData em uma operação PATCH.</span><span class="sxs-lookup"><span data-stu-id="df4fb-151">This example shows how to add multiple members to a group with OData bind support in a PATCH operation.</span></span> <span data-ttu-id="df4fb-152">Observe que é possível adicionar até 20 membros em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="df4fb-152">Note that up to 20 members can be added in a single request.</span></span> <span data-ttu-id="df4fb-153">Não há suporte para a operação POST.</span><span class="sxs-lookup"><span data-stu-id="df4fb-153">The POST operation is not supported.</span></span> <span data-ttu-id="df4fb-154">Se houver uma condição de erro no corpo da solicitação, nenhum membro será adicionado e o código de resposta apropriado será retornado.</span><span class="sxs-lookup"><span data-stu-id="df4fb-154">If an error condition exists in the request body, no members are added and the appropriate response code is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="df4fb-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df4fb-155">Request</span></span>

<span data-ttu-id="df4fb-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df4fb-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="df4fb-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="df4fb-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="df4fb-158">C#</span><span class="sxs-lookup"><span data-stu-id="df4fb-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-multiple-members-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df4fb-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df4fb-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-multiple-members-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df4fb-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df4fb-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-multiple-members-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df4fb-161">Java</span><span class="sxs-lookup"><span data-stu-id="df4fb-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-multiple-members-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="df4fb-162">No corpo da solicitação, forneça uma representação JSON da ID do objeto directoryObject, usuário ou grupo que deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="df4fb-162">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="df4fb-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="df4fb-163">Response</span></span>
<span data-ttu-id="df4fb-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df4fb-164">The following is an example of the response.</span></span>

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

