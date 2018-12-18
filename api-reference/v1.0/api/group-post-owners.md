---
title: Adicionar proprietário do grupo
description: Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
ms.openlocfilehash: ac3790ac3a61beb9b5d92916e8dac82f1849cc8a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332246"
---
# <a name="add-group-owner"></a><span data-ttu-id="b2224-104">Adicionar proprietário do grupo</span><span class="sxs-lookup"><span data-stu-id="b2224-104">Add group owner</span></span>
<span data-ttu-id="b2224-p102">Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="b2224-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="b2224-107">**Importante:** Se você atualizar os proprietários do grupo e você criou uma equipe para o grupo, pode demorar até 2 horas para os proprietários ser sincronizado com o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b2224-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="b2224-108">Além disso, se quiser que o proprietário sejam capazes de fazer alterações em uma equipe - por exemplo, ao criar um plano de Planejador - o proprietário também precisa ser adicionado como um membro de equipe/grupo.</span><span class="sxs-lookup"><span data-stu-id="b2224-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b2224-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2224-109">Permissions</span></span>
<span data-ttu-id="b2224-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2224-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2224-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2224-112">Permission type</span></span>      | <span data-ttu-id="b2224-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2224-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2224-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2224-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b2224-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b2224-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b2224-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2224-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2224-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2224-117">Not supported.</span></span>    |
|<span data-ttu-id="b2224-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2224-118">Application</span></span> | <span data-ttu-id="b2224-119">Group.ReadWrite.All e User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2224-119">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2224-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2224-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b2224-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2224-121">Request headers</span></span>
| <span data-ttu-id="b2224-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b2224-122">Name</span></span>       | <span data-ttu-id="b2224-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2224-123">Type</span></span> | <span data-ttu-id="b2224-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2224-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b2224-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2224-125">Authorization</span></span>  | <span data-ttu-id="b2224-126">string</span><span class="sxs-lookup"><span data-stu-id="b2224-126">string</span></span>  | <span data-ttu-id="b2224-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2224-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2224-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2224-129">Request body</span></span>
<span data-ttu-id="b2224-130">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="b2224-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="b2224-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2224-131">Response</span></span>
<span data-ttu-id="b2224-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2224-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2224-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2224-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b2224-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2224-135">Request</span></span>
<span data-ttu-id="b2224-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2224-136">The following is an example of the request.</span></span>
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
<span data-ttu-id="b2224-137">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="b2224-137">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="b2224-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2224-138">Response</span></span>
<span data-ttu-id="b2224-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b2224-139">The following is an example of the response.</span></span>
><span data-ttu-id="b2224-140">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b2224-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b2224-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2224-141">All the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->

