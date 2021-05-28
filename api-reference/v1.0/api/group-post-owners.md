---
title: Adicionar proprietário do grupo
description: Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
localization_priority: Priority
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fc469ce2594a98e602a53cc7733f3cca902c8f86
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680560"
---
# <a name="add-group-owner"></a><span data-ttu-id="29e4e-104">Adicionar proprietário do grupo</span><span class="sxs-lookup"><span data-stu-id="29e4e-104">Add group owner</span></span>

<span data-ttu-id="29e4e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29e4e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="29e4e-p102">Adicione um usuário ou diretor de serviço aos proprietários do grupo. Os proprietários são um conjunto de usuários ou diretores de serviço que têm permissão para modificar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="29e4e-p102">Add a user or service principal to the group's owners. The owners are a set of users or service principals who are allowed to modify the group object.</span></span>

><span data-ttu-id="29e4e-108">**Importante:** se você atualizar os proprietários do grupo, e você criou uma equipe para o grupo, poderá levar até duas horas para que os proprietários sejam sincronizados com o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="29e4e-108">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="29e4e-109">Além disso, se você quiser que o proprietário seja capaz de fazer alterações em uma equipe - por exemplo, criando um plano Planner - o proprietário também precisará ser adicionado como um membro do grupo/equipe.</span><span class="sxs-lookup"><span data-stu-id="29e4e-109">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="29e4e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="29e4e-110">Permissions</span></span>
<span data-ttu-id="29e4e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29e4e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29e4e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29e4e-113">Permission type</span></span>      | <span data-ttu-id="29e4e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29e4e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29e4e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29e4e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="29e4e-116">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29e4e-116">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29e4e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29e4e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29e4e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29e4e-118">Not supported.</span></span>    |
|<span data-ttu-id="29e4e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29e4e-119">Application</span></span> | <span data-ttu-id="29e4e-120">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29e4e-120">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29e4e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29e4e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="29e4e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29e4e-122">Request headers</span></span>
| <span data-ttu-id="29e4e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="29e4e-123">Name</span></span>       | <span data-ttu-id="29e4e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="29e4e-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="29e4e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="29e4e-125">Authorization</span></span>  | <span data-ttu-id="29e4e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29e4e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29e4e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29e4e-128">Content-Type</span></span> | <span data-ttu-id="29e4e-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29e4e-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29e4e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29e4e-131">Request body</span></span>
<span data-ttu-id="29e4e-132">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="29e4e-132">In the request body, supply a JSON representation of the [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="29e4e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="29e4e-133">Response</span></span>
<span data-ttu-id="29e4e-134">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="29e4e-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="29e4e-135">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29e4e-135">It does not return anything in the response body.</span></span> <span data-ttu-id="29e4e-136">Esse método retorna um `400 Bad Request` código de resposta quando o objeto já é um membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="29e4e-136">This method returns a `400 Bad Request` response code when the object is already a member of the group.</span></span> <span data-ttu-id="29e4e-137">Esse método retorna um `404 Not Found` código de resposta quando o objeto adicionado não existe.</span><span class="sxs-lookup"><span data-stu-id="29e4e-137">This method returns a `404 Not Found` response code when the object being added doesn't exist.</span></span>

## <a name="example"></a><span data-ttu-id="29e4e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29e4e-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="29e4e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29e4e-139">Request</span></span>
<span data-ttu-id="29e4e-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29e4e-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="29e4e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="29e4e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_owner_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="29e4e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29e4e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29e4e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29e4e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="29e4e-144">C#</span><span class="sxs-lookup"><span data-stu-id="29e4e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29e4e-145">Java</span><span class="sxs-lookup"><span data-stu-id="29e4e-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="29e4e-146">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="29e4e-146">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="29e4e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="29e4e-147">Response</span></span>
<span data-ttu-id="29e4e-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29e4e-148">The following is an example of the response.</span></span>
><span data-ttu-id="29e4e-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="29e4e-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


