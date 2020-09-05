---
title: Adicionar membro
description: Adicionar um membro a um grupo do Microsoft 365, um grupo de segurança ou um grupo de segurança habilitado para email através da propriedade de navegação **Members** .
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 74d6ba0443cadf236c6f4af8c0194dfa0cae3d53
ms.sourcegitcommit: 0a979eb1f21ec7834d24c268c24383c3139577ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/05/2020
ms.locfileid: "47400486"
---
# <a name="add-member"></a><span data-ttu-id="33271-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="33271-103">Add member</span></span>

<span data-ttu-id="33271-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33271-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33271-105">Adicionar um membro a um grupo do Microsoft 365 ou um grupo de segurança por meio da propriedade de navegação **Members** .</span><span class="sxs-lookup"><span data-stu-id="33271-105">Add a member to a Microsoft 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="33271-106">Você pode adicionar usuários, contatos organizacionais, entidades de serviço ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="33271-106">You can add users, organizational contacts, service principals or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="33271-107">Você só pode adicionar usuários aos grupos segurança e Microsoft 365 gerenciados por meio da nuvem.</span><span class="sxs-lookup"><span data-stu-id="33271-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="33271-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="33271-108">Permissions</span></span>

<span data-ttu-id="33271-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33271-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33271-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33271-111">Permission type</span></span>      | <span data-ttu-id="33271-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33271-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33271-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33271-113">Delegated (work or school account)</span></span> | <span data-ttu-id="33271-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33271-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33271-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33271-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33271-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33271-116">Not supported.</span></span>    |
|<span data-ttu-id="33271-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33271-117">Application</span></span> | <span data-ttu-id="33271-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33271-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33271-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33271-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="33271-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33271-120">Request headers</span></span>

| <span data-ttu-id="33271-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33271-121">Header</span></span>       | <span data-ttu-id="33271-122">Valor</span><span class="sxs-lookup"><span data-stu-id="33271-122">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="33271-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33271-123">Authorization</span></span>  | <span data-ttu-id="33271-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33271-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33271-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="33271-126">Content-type</span></span>   | <span data-ttu-id="33271-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33271-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33271-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33271-129">Request body</span></span>

<span data-ttu-id="33271-130">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) ou [organizational contact](../resources/orgcontact.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="33271-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="33271-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="33271-131">Response</span></span>

<span data-ttu-id="33271-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33271-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33271-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="33271-134">Examples</span></span>

### <a name="example-1-add-a-member-to-a-group"></a><span data-ttu-id="33271-135">Exemplo 1: adicionar um membro a um grupo</span><span class="sxs-lookup"><span data-stu-id="33271-135">Example 1: Add a member to a group</span></span>

#### <a name="request"></a><span data-ttu-id="33271-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33271-136">Request</span></span>

<span data-ttu-id="33271-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="33271-137">The following is an example of the request.</span></span>

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

<span data-ttu-id="33271-138">No corpo da solicitação, forneça uma representação JSON da ID do objeto directoryobject, User ou Group que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="33271-138">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="33271-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="33271-139">Response</span></span>

<span data-ttu-id="33271-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="33271-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a><span data-ttu-id="33271-141">Exemplo 2: adicionar vários membros a um grupo em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="33271-141">Example 2: Add multiple members to a group in a single request</span></span>

<span data-ttu-id="33271-142">Este exemplo mostra como adicionar vários membros a um grupo com suporte a BIND OData em uma operação PATCH.</span><span class="sxs-lookup"><span data-stu-id="33271-142">This example shows how to add multiple members to a group with OData bind support in a PATCH operation.</span></span> <span data-ttu-id="33271-143">Observe que até 20 membros podem ser adicionados em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="33271-143">Note that up to 20 members can be added in a single request.</span></span> <span data-ttu-id="33271-144">A operação POST não é suportada.</span><span class="sxs-lookup"><span data-stu-id="33271-144">The POST operation is not supported.</span></span>

#### <a name="request"></a><span data-ttu-id="33271-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33271-145">Request</span></span>

<span data-ttu-id="33271-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="33271-146">The following is an example of the request.</span></span>

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

<span data-ttu-id="33271-147">No corpo da solicitação, forneça uma representação JSON da ID do objeto directoryobject, User ou Group que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="33271-147">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="33271-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="33271-148">Response</span></span>
<span data-ttu-id="33271-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="33271-149">The following is an example of the response.</span></span>

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
