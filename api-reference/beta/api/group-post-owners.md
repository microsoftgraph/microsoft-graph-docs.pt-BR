---
title: Adicionar proprietário do grupo
description: Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
ms.openlocfilehash: 903c659722877263038860c7d2ff47b301b6d5c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308894"
---
# <a name="add-group-owner"></a><span data-ttu-id="6878e-104">Adicionar proprietário do grupo</span><span class="sxs-lookup"><span data-stu-id="6878e-104">Add group owner</span></span>

> <span data-ttu-id="6878e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6878e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6878e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6878e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6878e-p103">Adiciona um usuário aos proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="6878e-p103">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="6878e-109">**Importante:** Se você atualizar os proprietários do grupo e você criou uma equipe para o grupo, pode demorar até 2 horas para os proprietários ser sincronizado com o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6878e-109">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="6878e-110">Além disso, se quiser que o proprietário sejam capazes de fazer alterações em uma equipe - por exemplo, ao criar um plano de Planejador - o proprietário também precisa ser adicionado como um membro de equipe/grupo.</span><span class="sxs-lookup"><span data-stu-id="6878e-110">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6878e-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="6878e-111">Permissions</span></span>
<span data-ttu-id="6878e-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6878e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6878e-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6878e-114">Permission type</span></span>      | <span data-ttu-id="6878e-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6878e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6878e-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6878e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="6878e-117">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6878e-117">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6878e-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6878e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6878e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6878e-119">Not supported.</span></span>    |
|<span data-ttu-id="6878e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6878e-120">Application</span></span> | <span data-ttu-id="6878e-121">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6878e-121">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6878e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6878e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6878e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6878e-123">Request headers</span></span>
| <span data-ttu-id="6878e-124">Nome</span><span class="sxs-lookup"><span data-stu-id="6878e-124">Name</span></span>       | <span data-ttu-id="6878e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="6878e-125">Type</span></span> | <span data-ttu-id="6878e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6878e-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6878e-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="6878e-127">Authorization</span></span>  | <span data-ttu-id="6878e-128">string</span><span class="sxs-lookup"><span data-stu-id="6878e-128">string</span></span>  | <span data-ttu-id="6878e-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6878e-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6878e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6878e-131">Request body</span></span>
<span data-ttu-id="6878e-132">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="6878e-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="6878e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6878e-133">Response</span></span>
<span data-ttu-id="6878e-p107">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6878e-p107">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6878e-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6878e-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6878e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6878e-137">Request</span></span>
<span data-ttu-id="6878e-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6878e-138">The following is an example of the request.</span></span>
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
<span data-ttu-id="6878e-139">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="6878e-139">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="6878e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6878e-140">Response</span></span>
<span data-ttu-id="6878e-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6878e-141">The following is an example of the response.</span></span>
><span data-ttu-id="6878e-142">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6878e-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6878e-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6878e-143">All the properties will be returned from an actual call.</span></span>
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
