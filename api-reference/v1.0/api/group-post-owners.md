---
title: Adicionar proprietário do grupo
description: Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 532ee6eec8e49fd063e9ee3f41c03aa939a3c89a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277676"
---
# <a name="add-group-owner"></a><span data-ttu-id="615f3-104">Adicionar proprietário do grupo</span><span class="sxs-lookup"><span data-stu-id="615f3-104">Add group owner</span></span>
<span data-ttu-id="615f3-p102">Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="615f3-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="615f3-107">**Importante:** se você atualizar os proprietários do grupo, e você criou uma equipe para o grupo, poderá levar até duas horas para que os proprietários sejam sincronizados com o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="615f3-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="615f3-108">Além disso, se você quiser que o proprietário seja capaz de fazer alterações em uma equipe - por exemplo, criando um plano Planner - o proprietário também precisará ser adicionado como um membro do grupo/equipe.</span><span class="sxs-lookup"><span data-stu-id="615f3-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="615f3-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="615f3-109">Permissions</span></span>
<span data-ttu-id="615f3-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="615f3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="615f3-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="615f3-112">Permission type</span></span>      | <span data-ttu-id="615f3-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="615f3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="615f3-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="615f3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="615f3-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="615f3-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="615f3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="615f3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="615f3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="615f3-117">Not supported.</span></span>    |
|<span data-ttu-id="615f3-118">Application</span><span class="sxs-lookup"><span data-stu-id="615f3-118">Application</span></span> | <span data-ttu-id="615f3-119">Group.ReadWrite.All e User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="615f3-119">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="615f3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="615f3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="615f3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="615f3-121">Request headers</span></span>
| <span data-ttu-id="615f3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="615f3-122">Name</span></span>       | <span data-ttu-id="615f3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="615f3-123">Type</span></span> | <span data-ttu-id="615f3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="615f3-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="615f3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="615f3-125">Authorization</span></span>  | <span data-ttu-id="615f3-126">string</span><span class="sxs-lookup"><span data-stu-id="615f3-126">string</span></span>  | <span data-ttu-id="615f3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="615f3-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="615f3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="615f3-129">Request body</span></span>
<span data-ttu-id="615f3-130">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="615f3-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="615f3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="615f3-131">Response</span></span>
<span data-ttu-id="615f3-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="615f3-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="615f3-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="615f3-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="615f3-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="615f3-135">Request</span></span>
<span data-ttu-id="615f3-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="615f3-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="615f3-137">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="615f3-137">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="615f3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="615f3-138">Response</span></span>
<span data-ttu-id="615f3-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="615f3-139">The following is an example of the response.</span></span>
><span data-ttu-id="615f3-140">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="615f3-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="615f3-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="615f3-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="615f3-142">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="615f3-142">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="615f3-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="615f3-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="615f3-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="615f3-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-owners.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-owners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

