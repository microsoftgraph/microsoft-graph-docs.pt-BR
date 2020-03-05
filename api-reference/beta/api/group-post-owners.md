---
title: Adicionar proprietário do grupo
description: Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 06cd29f13bd5ed2a11f7f5f033da64e488f92ead
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418775"
---
# <a name="add-group-owner"></a><span data-ttu-id="c9d60-104">Adicionar proprietário do grupo</span><span class="sxs-lookup"><span data-stu-id="c9d60-104">Add group owner</span></span>

<span data-ttu-id="c9d60-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c9d60-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9d60-106">Adiciona um usuário aos proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="c9d60-106">Add a user to the group's owners.</span></span> <span data-ttu-id="c9d60-107">Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="c9d60-107">The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="c9d60-108">**Importante:** se você atualizar os proprietários do grupo, e você criou uma equipe para o grupo, poderá levar até duas horas para que os proprietários sejam sincronizados com o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c9d60-108">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="c9d60-109">Além disso, se você quiser que o proprietário seja capaz de fazer alterações em uma equipe - por exemplo, criando um plano Planner - o proprietário também precisará ser adicionado como um membro do grupo/equipe.</span><span class="sxs-lookup"><span data-stu-id="c9d60-109">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c9d60-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9d60-110">Permissions</span></span>
<span data-ttu-id="c9d60-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9d60-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9d60-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9d60-113">Permission type</span></span>      | <span data-ttu-id="c9d60-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9d60-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9d60-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9d60-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c9d60-116">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c9d60-116">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c9d60-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9d60-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9d60-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9d60-118">Not supported.</span></span>    |
|<span data-ttu-id="c9d60-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9d60-119">Application</span></span> | <span data-ttu-id="c9d60-120">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9d60-120">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9d60-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9d60-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c9d60-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9d60-122">Request headers</span></span>
| <span data-ttu-id="c9d60-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c9d60-123">Name</span></span>       | <span data-ttu-id="c9d60-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9d60-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c9d60-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9d60-125">Authorization</span></span>  | <span data-ttu-id="c9d60-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9d60-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c9d60-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="c9d60-128">Content-type</span></span> | <span data-ttu-id="c9d60-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9d60-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9d60-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9d60-131">Request body</span></span>
<span data-ttu-id="c9d60-132">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="c9d60-132">In the request body, supply a JSON representation of the [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="c9d60-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9d60-133">Response</span></span>
<span data-ttu-id="c9d60-p107">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9d60-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9d60-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9d60-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c9d60-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9d60-137">Request</span></span>
<span data-ttu-id="c9d60-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9d60-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c9d60-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9d60-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_owner_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="c9d60-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9d60-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9d60-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9d60-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c9d60-142">C#</span><span class="sxs-lookup"><span data-stu-id="c9d60-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c9d60-143">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="c9d60-143">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="c9d60-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9d60-144">Response</span></span>
<span data-ttu-id="c9d60-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c9d60-145">The following is an example of the response.</span></span>
><span data-ttu-id="c9d60-146">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c9d60-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c9d60-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9d60-147">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
