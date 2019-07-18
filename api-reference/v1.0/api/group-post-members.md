---
title: Adicionar membro
description: Adicione um membro a um grupo do Office 365, a um grupo de segurança ou a um grupo de segurança habilitado para email através da propriedade de navegação de **membros**.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: a3ccacd1ebb1985cd09de31f9568df86660451af
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778425"
---
# <a name="add-member"></a><span data-ttu-id="bfb41-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="bfb41-103">Add member</span></span>
<span data-ttu-id="bfb41-104">Adicione um membro a um grupo do Office 365 ou a um grupo de segurança através da propriedade de navegação de **membros**.</span><span class="sxs-lookup"><span data-stu-id="bfb41-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="bfb41-105">É possível adicionar usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="bfb41-105">You can add users or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="bfb41-106">É possível adicionar somente usuários a grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="bfb41-106">Important: You can add only users to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfb41-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bfb41-107">Permissions</span></span>
<span data-ttu-id="bfb41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfb41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfb41-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfb41-110">Permission type</span></span>      | <span data-ttu-id="bfb41-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfb41-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfb41-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfb41-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bfb41-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bfb41-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bfb41-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfb41-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfb41-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfb41-115">Not supported.</span></span>    |
|<span data-ttu-id="bfb41-116">Application</span><span class="sxs-lookup"><span data-stu-id="bfb41-116">Application</span></span> | <span data-ttu-id="bfb41-117">Group.ReadWrite.All e Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfb41-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfb41-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfb41-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="bfb41-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfb41-119">Request headers</span></span>
| <span data-ttu-id="bfb41-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bfb41-120">Name</span></span>       | <span data-ttu-id="bfb41-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfb41-121">Type</span></span> | <span data-ttu-id="bfb41-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfb41-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bfb41-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfb41-123">Authorization</span></span>  | <span data-ttu-id="bfb41-124">string</span><span class="sxs-lookup"><span data-stu-id="bfb41-124">string</span></span>  | <span data-ttu-id="bfb41-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfb41-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfb41-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfb41-127">Request body</span></span>
<span data-ttu-id="bfb41-128">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="bfb41-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="bfb41-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfb41-129">Response</span></span>
<span data-ttu-id="bfb41-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfb41-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfb41-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfb41-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bfb41-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfb41-133">Request</span></span>
<span data-ttu-id="bfb41-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfb41-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bfb41-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfb41-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bfb41-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="bfb41-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bfb41-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfb41-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="bfb41-138">No corpo da solicitação, forneça uma representação JSON da `id` do objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) que deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="bfb41-138">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="bfb41-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfb41-139">Response</span></span>
<span data-ttu-id="bfb41-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfb41-140">The following is an example of the response.</span></span>
><span data-ttu-id="bfb41-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bfb41-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bfb41-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfb41-142">All the properties will be returned from an actual call.</span></span>
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
