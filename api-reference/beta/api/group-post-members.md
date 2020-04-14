---
title: Adicionar membro
description: Adicionar um membro a um grupo do Office 365 ou grupo de segurança por meio da propriedade de navegação **Members** .
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8e4b209d7b941bc681e63f9f1781072ff501eb1e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396571"
---
# <a name="add-member"></a><span data-ttu-id="b1a3d-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="b1a3d-103">Add member</span></span>

<span data-ttu-id="b1a3d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1a3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1a3d-105">Adicionar um membro a um grupo do Office 365 ou grupo de segurança por meio da propriedade de navegação **Members** .</span><span class="sxs-lookup"><span data-stu-id="b1a3d-105">Add a member to an Office 365 group or security group through the **members** navigation property.</span></span>

<span data-ttu-id="b1a3d-106">É possível adicionar usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="b1a3d-106">You can add users or other groups.</span></span> 

> [!Important]
> <span data-ttu-id="b1a3d-107">Só é possível adicionar usuários aos grupos do Office 365 e segurança gerenciados pela nuvem.</span><span class="sxs-lookup"><span data-stu-id="b1a3d-107">You can only add users to security and Office 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1a3d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1a3d-108">Permissions</span></span>
<span data-ttu-id="b1a3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1a3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1a3d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1a3d-111">Permission type</span></span>      | <span data-ttu-id="b1a3d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1a3d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1a3d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1a3d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b1a3d-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b1a3d-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b1a3d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1a3d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1a3d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1a3d-116">Not supported.</span></span>    |
|<span data-ttu-id="b1a3d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1a3d-117">Application</span></span> | <span data-ttu-id="b1a3d-118">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1a3d-118">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1a3d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1a3d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b1a3d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1a3d-120">Request headers</span></span>
| <span data-ttu-id="b1a3d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b1a3d-121">Name</span></span> | <span data-ttu-id="b1a3d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1a3d-122">Description</span></span>|
|:---- |:-----------|
| <span data-ttu-id="b1a3d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1a3d-123">Authorization</span></span> | <span data-ttu-id="b1a3d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1a3d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1a3d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1a3d-126">Request body</span></span>
<span data-ttu-id="b1a3d-127">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="b1a3d-127">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="b1a3d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1a3d-128">Response</span></span>
<span data-ttu-id="b1a3d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1a3d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1a3d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1a3d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1a3d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1a3d-132">Request</span></span>
<span data-ttu-id="b1a3d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1a3d-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b1a3d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1a3d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="b1a3d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1a3d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1a3d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1a3d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b1a3d-137">C#</span><span class="sxs-lookup"><span data-stu-id="b1a3d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b1a3d-138">No corpo da solicitação, forneça uma representação JSON `id` do objeto [directoryobject](../resources/directoryobject.md), [User](../resources/user.md)ou [Group](../resources/group.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="b1a3d-138">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="b1a3d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1a3d-139">Response</span></span>
<span data-ttu-id="b1a3d-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b1a3d-140">The following is an example of the response.</span></span>
><span data-ttu-id="b1a3d-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b1a3d-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b1a3d-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1a3d-142">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
