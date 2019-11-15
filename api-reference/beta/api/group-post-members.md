---
title: Adicionar membro
description: Adicionar um membro a um grupo do Office 365 ou grupo de segurança por meio da propriedade de navegação **Members** .
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5169d2b2c54fc8055effcf1984c6279168a84072
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38657869"
---
# <a name="add-member"></a><span data-ttu-id="57095-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="57095-103">Add member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57095-104">Adicionar um membro a um grupo do Office 365 ou grupo de segurança por meio da propriedade de navegação **Members** .</span><span class="sxs-lookup"><span data-stu-id="57095-104">Add a member to an Office 365 group or security group through the **members** navigation property.</span></span>

<span data-ttu-id="57095-105">É possível adicionar usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="57095-105">You can add users or other groups.</span></span> 

> [!Important]
> <span data-ttu-id="57095-106">Só é possível adicionar usuários aos grupos do Office 365 e segurança gerenciados pela nuvem.</span><span class="sxs-lookup"><span data-stu-id="57095-106">You can only add users to security and Office 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="57095-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="57095-107">Permissions</span></span>
<span data-ttu-id="57095-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57095-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57095-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57095-110">Permission type</span></span>      | <span data-ttu-id="57095-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57095-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57095-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57095-112">Delegated (work or school account)</span></span> | <span data-ttu-id="57095-113">GroupMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="57095-113">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="57095-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57095-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57095-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57095-115">Not supported.</span></span>    |
|<span data-ttu-id="57095-116">Application</span><span class="sxs-lookup"><span data-stu-id="57095-116">Application</span></span> | <span data-ttu-id="57095-117">GroupMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="57095-117">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57095-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57095-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="57095-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57095-119">Request headers</span></span>
| <span data-ttu-id="57095-120">Nome</span><span class="sxs-lookup"><span data-stu-id="57095-120">Name</span></span> | <span data-ttu-id="57095-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="57095-121">Description</span></span>|
|:---- |:-----------|
| <span data-ttu-id="57095-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="57095-122">Authorization</span></span> | <span data-ttu-id="57095-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57095-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57095-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57095-125">Request body</span></span>
<span data-ttu-id="57095-126">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="57095-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="57095-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="57095-127">Response</span></span>
<span data-ttu-id="57095-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57095-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57095-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57095-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="57095-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57095-131">Request</span></span>
<span data-ttu-id="57095-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="57095-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="57095-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="57095-133">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57095-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57095-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="57095-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57095-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="57095-136">C#</span><span class="sxs-lookup"><span data-stu-id="57095-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="57095-137">No corpo da solicitação, forneça uma representação JSON `id` do objeto [directoryobject](../resources/directoryobject.md), [User](../resources/user.md)ou [Group](../resources/group.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="57095-137">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="57095-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="57095-138">Response</span></span>
<span data-ttu-id="57095-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="57095-139">The following is an example of the response.</span></span>
><span data-ttu-id="57095-140">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="57095-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="57095-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57095-141">All the properties will be returned from an actual call.</span></span>
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
