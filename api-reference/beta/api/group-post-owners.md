---
title: Adicionar proprietário do grupo
description: Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 0f46ec957a74aa8619a9c4e2a29fde182b012c01
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857993"
---
# <a name="add-group-owner"></a><span data-ttu-id="8b503-104">Adicionar proprietário do grupo</span><span class="sxs-lookup"><span data-stu-id="8b503-104">Add group owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b503-p102">Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="8b503-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="8b503-107">**Importante:** se você atualizar os proprietários do grupo, e você criou uma equipe para o grupo, poderá levar até duas horas para que os proprietários sejam sincronizados com o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8b503-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="8b503-108">Além disso, se você quiser que o proprietário seja capaz de fazer alterações em uma equipe - por exemplo, criando um plano Planner - o proprietário também precisará ser adicionado como um membro do grupo/equipe.</span><span class="sxs-lookup"><span data-stu-id="8b503-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8b503-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b503-109">Permissions</span></span>
<span data-ttu-id="8b503-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b503-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b503-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b503-112">Permission type</span></span>      | <span data-ttu-id="8b503-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b503-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b503-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b503-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8b503-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b503-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8b503-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b503-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b503-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b503-117">Not supported.</span></span>    |
|<span data-ttu-id="8b503-118">Application</span><span class="sxs-lookup"><span data-stu-id="8b503-118">Application</span></span> | <span data-ttu-id="8b503-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b503-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b503-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b503-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8b503-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b503-121">Request headers</span></span>
| <span data-ttu-id="8b503-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8b503-122">Name</span></span>       | <span data-ttu-id="8b503-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b503-123">Type</span></span> | <span data-ttu-id="8b503-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b503-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8b503-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b503-125">Authorization</span></span>  | <span data-ttu-id="8b503-126">string</span><span class="sxs-lookup"><span data-stu-id="8b503-126">string</span></span>  | <span data-ttu-id="8b503-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b503-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b503-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b503-129">Request body</span></span>
<span data-ttu-id="8b503-130">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="8b503-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="8b503-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b503-131">Response</span></span>
<span data-ttu-id="8b503-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b503-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b503-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b503-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8b503-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b503-135">Request</span></span>
<span data-ttu-id="8b503-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b503-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8b503-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b503-137">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8b503-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="8b503-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8b503-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8b503-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="8b503-140">C#</span><span class="sxs-lookup"><span data-stu-id="8b503-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8b503-141">Java</span><span class="sxs-lookup"><span data-stu-id="8b503-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8b503-142">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="8b503-142">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="8b503-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b503-143">Response</span></span>
<span data-ttu-id="8b503-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8b503-144">The following is an example of the response.</span></span>
><span data-ttu-id="8b503-145">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b503-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8b503-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b503-146">All the properties will be returned from an actual call.</span></span>
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
