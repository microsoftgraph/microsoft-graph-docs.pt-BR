---
title: Adicionar proprietário do grupo
description: Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3ba3f85193921fe7b77e6640200ec0a82b610997
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516974"
---
# <a name="add-group-owner"></a><span data-ttu-id="8cc1e-104">Adicionar proprietário do grupo</span><span class="sxs-lookup"><span data-stu-id="8cc1e-104">Add group owner</span></span>

<span data-ttu-id="8cc1e-p102">Namespace: microsoft.graph Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-p102">Namespace: microsoft.graph Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="8cc1e-107">**Importante:** se você atualizar os proprietários do grupo, e você criou uma equipe para o grupo, poderá levar até duas horas para que os proprietários sejam sincronizados com o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="8cc1e-108">Além disso, se você quiser que o proprietário seja capaz de fazer alterações em uma equipe - por exemplo, criando um plano Planner - o proprietário também precisará ser adicionado como um membro do grupo/equipe.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8cc1e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8cc1e-109">Permissions</span></span>
<span data-ttu-id="8cc1e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc1e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc1e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc1e-112">Permission type</span></span>      | <span data-ttu-id="8cc1e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cc1e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cc1e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc1e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8cc1e-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8cc1e-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8cc1e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc1e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cc1e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-117">Not supported.</span></span>    |
|<span data-ttu-id="8cc1e-118">Application</span><span class="sxs-lookup"><span data-stu-id="8cc1e-118">Application</span></span> | <span data-ttu-id="8cc1e-119">Group.ReadWrite.All e User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc1e-119">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cc1e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc1e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8cc1e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc1e-121">Request headers</span></span>
| <span data-ttu-id="8cc1e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8cc1e-122">Name</span></span>       | <span data-ttu-id="8cc1e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc1e-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8cc1e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cc1e-124">Authorization</span></span>  | <span data-ttu-id="8cc1e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8cc1e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cc1e-127">Content-Type</span></span> | <span data-ttu-id="8cc1e-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cc1e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc1e-130">Request body</span></span>
<span data-ttu-id="8cc1e-131">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-131">In the request body, supply a JSON representation of the [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="8cc1e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc1e-132">Response</span></span>
<span data-ttu-id="8cc1e-p107">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc1e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc1e-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8cc1e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc1e-136">Request</span></span>
<span data-ttu-id="8cc1e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8cc1e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc1e-138">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="8cc1e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cc1e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cc1e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cc1e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8cc1e-141">C#</span><span class="sxs-lookup"><span data-stu-id="8cc1e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8cc1e-142">Java</span><span class="sxs-lookup"><span data-stu-id="8cc1e-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8cc1e-143">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-143">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="8cc1e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc1e-144">Response</span></span>
<span data-ttu-id="8cc1e-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-145">The following is an example of the response.</span></span>
><span data-ttu-id="8cc1e-146">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8cc1e-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cc1e-147">All the properties will be returned from an actual call.</span></span>
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

