---
title: Adicionar membro
description: Adicione um membro a um grupo ou grupo de segurança do Microsoft 365 por meio da **propriedade de navegação de** membros.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 188f93c82734c9ae9fe0986114e3c4e4d2bd1772
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468867"
---
# <a name="add-member"></a><span data-ttu-id="ba2a6-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="ba2a6-103">Add member</span></span>

<span data-ttu-id="ba2a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba2a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba2a6-105">Adicione um membro a um grupo ou grupo de segurança do Microsoft 365 por meio da **propriedade de navegação de** membros.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-105">Add a member to a Microsoft 365 group or security group through the **members** navigation property.</span></span>

<span data-ttu-id="ba2a6-106">Você pode adicionar usuários, entidades de serviço ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-106">You can add users, service principals or other groups.</span></span> 

> [!Important]
> + <span data-ttu-id="ba2a6-107">Só é possível adicionar usuários aos grupos do Microsoft 365 e segurança gerenciados pela nuvem.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>
> + <span data-ttu-id="ba2a6-108">Não é possível adicionar grupos de segurança aos grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-108">You cannot add security groups to Microsoft 365 groups.</span></span>
> + <span data-ttu-id="ba2a6-109">Não é possível adicionar grupos do Microsoft 365 a grupos de segurança ou outros grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-109">You cannot add Microsoft 365 groups to security groups or other Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba2a6-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba2a6-110">Permissions</span></span>
<span data-ttu-id="ba2a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba2a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba2a6-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba2a6-113">Permission type</span></span>      | <span data-ttu-id="ba2a6-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba2a6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba2a6-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba2a6-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ba2a6-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba2a6-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba2a6-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba2a6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba2a6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-118">Not supported.</span></span>    |
|<span data-ttu-id="ba2a6-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba2a6-119">Application</span></span> | <span data-ttu-id="ba2a6-120">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba2a6-120">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba2a6-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba2a6-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ba2a6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba2a6-122">Request headers</span></span>
| <span data-ttu-id="ba2a6-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ba2a6-123">Name</span></span> | <span data-ttu-id="ba2a6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba2a6-124">Description</span></span>|
|:---- |:-----------|
| <span data-ttu-id="ba2a6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba2a6-125">Authorization</span></span> | <span data-ttu-id="ba2a6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba2a6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba2a6-128">Request body</span></span>
<span data-ttu-id="ba2a6-129">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="ba2a6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba2a6-130">Response</span></span>
<span data-ttu-id="ba2a6-131">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="ba2a6-132">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-132">It does not return anything in the response body.</span></span> <span data-ttu-id="ba2a6-133">Esse método retorna um `400 Bad Request` código de resposta quando o objeto já é um membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-133">This method returns a `400 Bad Request` response code when the object is already a member of the group.</span></span> <span data-ttu-id="ba2a6-134">Esse método retorna um `404 Not Found` código de resposta quando o objeto adicionado não existe.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-134">This method returns a `404 Not Found` response code when the object being added doesn't exist.</span></span> 

## <a name="example"></a><span data-ttu-id="ba2a6-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba2a6-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="ba2a6-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba2a6-136">Request</span></span>
<span data-ttu-id="ba2a6-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ba2a6-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba2a6-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{group-id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="ba2a6-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba2a6-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba2a6-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba2a6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="ba2a6-141">C#</span><span class="sxs-lookup"><span data-stu-id="ba2a6-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba2a6-142">Java</span><span class="sxs-lookup"><span data-stu-id="ba2a6-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-group-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ba2a6-143">No corpo da solicitação, fornece uma representação JSON do `id` [objeto directoryObject](../resources/directoryobject.md), [user](../resources/user.md)ou [group](../resources/group.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-143">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="ba2a6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba2a6-144">Response</span></span>
<span data-ttu-id="ba2a6-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-145">The following is an example of the response.</span></span>

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


