---
title: Adicionar proprietário do grupo
description: Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 98d5a0275cd5bbab9ee992774b8c771d9ec12d61
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440292"
---
# <a name="add-group-owner"></a><span data-ttu-id="ba619-104">Adicionar proprietário do grupo</span><span class="sxs-lookup"><span data-stu-id="ba619-104">Add group owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba619-p102">Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="ba619-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="ba619-107">**Importante:** se você atualizar os proprietários do grupo, e você criou uma equipe para o grupo, poderá levar até duas horas para que os proprietários sejam sincronizados com o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ba619-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="ba619-108">Além disso, se você quiser que o proprietário seja capaz de fazer alterações em uma equipe - por exemplo, criando um plano Planner - o proprietário também precisará ser adicionado como um membro do grupo/equipe.</span><span class="sxs-lookup"><span data-stu-id="ba619-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ba619-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba619-109">Permissions</span></span>
<span data-ttu-id="ba619-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba619-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba619-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba619-112">Permission type</span></span>      | <span data-ttu-id="ba619-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba619-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba619-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba619-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ba619-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba619-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba619-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba619-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba619-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba619-117">Not supported.</span></span>    |
|<span data-ttu-id="ba619-118">Application</span><span class="sxs-lookup"><span data-stu-id="ba619-118">Application</span></span> | <span data-ttu-id="ba619-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba619-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba619-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba619-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ba619-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba619-121">Request headers</span></span>
| <span data-ttu-id="ba619-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ba619-122">Name</span></span>       | <span data-ttu-id="ba619-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba619-123">Type</span></span> | <span data-ttu-id="ba619-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba619-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba619-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba619-125">Authorization</span></span>  | <span data-ttu-id="ba619-126">string</span><span class="sxs-lookup"><span data-stu-id="ba619-126">string</span></span>  | <span data-ttu-id="ba619-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba619-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba619-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba619-129">Request body</span></span>
<span data-ttu-id="ba619-130">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="ba619-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="ba619-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba619-131">Response</span></span>
<span data-ttu-id="ba619-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba619-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba619-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba619-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ba619-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba619-135">Request</span></span>
<span data-ttu-id="ba619-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba619-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ba619-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba619-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba619-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="ba619-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ba619-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ba619-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ba619-140">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="ba619-140">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="ba619-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba619-141">Response</span></span>
<span data-ttu-id="ba619-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba619-142">The following is an example of the response.</span></span>
><span data-ttu-id="ba619-143">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ba619-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ba619-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba619-144">All the properties will be returned from an actual call.</span></span>
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
