---
title: Adicionar membro
description: Use esta API para adicionar um membro a um grupo do Office 365, a um grupo de segurança ou a um grupo de segurança habilitado para email através da propriedade de navegação **owners**.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 9ed8ef9f054a9d0c7a69ab21067664b7fd2f6853
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440257"
---
# <a name="add-member"></a><span data-ttu-id="52a2b-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="52a2b-103">Add member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52a2b-104">Use esta API para adicionar um membro a um grupo do Office 365, a um grupo de segurança ou a um grupo de segurança habilitado para email através da propriedade de navegação **owners**.</span><span class="sxs-lookup"><span data-stu-id="52a2b-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="52a2b-105">É possível adicionar usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="52a2b-105">You can add users or other groups.</span></span> <span data-ttu-id="52a2b-106">Importante: só é possível adicionar usuários a grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="52a2b-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="52a2b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="52a2b-107">Permissions</span></span>
<span data-ttu-id="52a2b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52a2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52a2b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52a2b-110">Permission type</span></span>      | <span data-ttu-id="52a2b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52a2b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52a2b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52a2b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="52a2b-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="52a2b-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="52a2b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52a2b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52a2b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52a2b-115">Not supported.</span></span>    |
|<span data-ttu-id="52a2b-116">Application</span><span class="sxs-lookup"><span data-stu-id="52a2b-116">Application</span></span> | <span data-ttu-id="52a2b-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52a2b-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52a2b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52a2b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="52a2b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52a2b-119">Request headers</span></span>
| <span data-ttu-id="52a2b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="52a2b-120">Name</span></span>       | <span data-ttu-id="52a2b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="52a2b-121">Type</span></span> | <span data-ttu-id="52a2b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="52a2b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="52a2b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="52a2b-123">Authorization</span></span>  | <span data-ttu-id="52a2b-124">string</span><span class="sxs-lookup"><span data-stu-id="52a2b-124">string</span></span>  | <span data-ttu-id="52a2b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52a2b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52a2b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52a2b-127">Request body</span></span>
<span data-ttu-id="52a2b-128">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="52a2b-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="52a2b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="52a2b-129">Response</span></span>
<span data-ttu-id="52a2b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52a2b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52a2b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52a2b-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="52a2b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52a2b-133">Request</span></span>
<span data-ttu-id="52a2b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52a2b-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="52a2b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="52a2b-135">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52a2b-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="52a2b-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="52a2b-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="52a2b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="52a2b-138">No corpo da solicitação, forneça uma representação JSON `id` do objeto [directoryobject](../resources/directoryobject.md), [User](../resources/user.md)ou [Group](../resources/group.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="52a2b-138">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="52a2b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="52a2b-139">Response</span></span>
<span data-ttu-id="52a2b-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52a2b-140">The following is an example of the response.</span></span>
><span data-ttu-id="52a2b-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52a2b-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="52a2b-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52a2b-142">All the properties will be returned from an actual call.</span></span>
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
