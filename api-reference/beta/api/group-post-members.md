---
title: Adicionar membro
description: Adicione um membro a um grupo Microsoft 365 ou grupo de segurança por meio da **propriedade de navegação de** membros.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5e7c4b6d2f4547a57783307f5da2c1ea0af88b20
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681386"
---
# <a name="add-member"></a><span data-ttu-id="907f7-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="907f7-103">Add member</span></span>

<span data-ttu-id="907f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="907f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="907f7-105">Adicione um membro a um grupo Microsoft 365 ou grupo de segurança por meio da **propriedade de navegação de** membros.</span><span class="sxs-lookup"><span data-stu-id="907f7-105">Add a member to a Microsoft 365 group or security group through the **members** navigation property.</span></span>

<span data-ttu-id="907f7-106">Você pode adicionar usuários, entidades de serviço ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="907f7-106">You can add users, service principals or other groups.</span></span> 

> [!Important]
> + <span data-ttu-id="907f7-107">Só é possível adicionar usuários aos grupos do Microsoft 365 e segurança gerenciados pela nuvem.</span><span class="sxs-lookup"><span data-stu-id="907f7-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>
> + <span data-ttu-id="907f7-108">Não é possível adicionar grupos de segurança a grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="907f7-108">You cannot add security groups to Microsoft 365 groups.</span></span>
> + <span data-ttu-id="907f7-109">Não é possível adicionar grupos do Microsoft 365 a grupos de segurança ou a outros grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="907f7-109">You cannot add Microsoft 365 groups to security groups or other Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="907f7-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="907f7-110">Permissions</span></span>
<span data-ttu-id="907f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="907f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="907f7-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="907f7-113">Permission type</span></span>      | <span data-ttu-id="907f7-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="907f7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="907f7-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="907f7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="907f7-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="907f7-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="907f7-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="907f7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="907f7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="907f7-118">Not supported.</span></span>    |
|<span data-ttu-id="907f7-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="907f7-119">Application</span></span> | <span data-ttu-id="907f7-120">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="907f7-120">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="907f7-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="907f7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="907f7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="907f7-122">Request headers</span></span>
| <span data-ttu-id="907f7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="907f7-123">Name</span></span> | <span data-ttu-id="907f7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="907f7-124">Description</span></span>|
|:---- |:-----------|
| <span data-ttu-id="907f7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="907f7-125">Authorization</span></span> | <span data-ttu-id="907f7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="907f7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="907f7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="907f7-128">Request body</span></span>
<span data-ttu-id="907f7-129">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="907f7-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="907f7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="907f7-130">Response</span></span>
<span data-ttu-id="907f7-131">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="907f7-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="907f7-132">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="907f7-132">It does not return anything in the response body.</span></span> <span data-ttu-id="907f7-133">Esse método retorna um `400 Bad Request` código de resposta quando o objeto já é um membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="907f7-133">This method returns a `400 Bad Request` response code when the object is already a member of the group.</span></span> <span data-ttu-id="907f7-134">Esse método retorna um `404 Not Found` código de resposta quando o objeto adicionado não existe.</span><span class="sxs-lookup"><span data-stu-id="907f7-134">This method returns a `404 Not Found` response code when the object being added doesn't exist.</span></span> 

## <a name="example"></a><span data-ttu-id="907f7-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="907f7-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="907f7-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="907f7-136">Request</span></span>
<span data-ttu-id="907f7-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="907f7-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="907f7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="907f7-138">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="907f7-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="907f7-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="907f7-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="907f7-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="907f7-141">C#</span><span class="sxs-lookup"><span data-stu-id="907f7-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="907f7-142">Java</span><span class="sxs-lookup"><span data-stu-id="907f7-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-group-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="907f7-143">No corpo da solicitação, fornece uma representação JSON do `id` [objeto directoryObject](../resources/directoryobject.md), [user](../resources/user.md)ou [group](../resources/group.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="907f7-143">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="907f7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="907f7-144">Response</span></span>
<span data-ttu-id="907f7-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="907f7-145">The following is an example of the response.</span></span>

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


