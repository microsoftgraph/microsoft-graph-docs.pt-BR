---
title: Remover grupo de incompatibleGroups
description: Remova um link que indica que um grupo é incompatível com um pacote de acesso especificado.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 403d583aa2b4e4592a4ec0bd9d9f29c3b93a1927
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439394"
---
# <a name="remove-group-from-incompatiblegroups"></a><span data-ttu-id="37206-103">Remover grupo de incompatibleGroups</span><span class="sxs-lookup"><span data-stu-id="37206-103">Remove group from incompatibleGroups</span></span>

<span data-ttu-id="37206-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37206-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37206-105">Remover um [grupo](../resources/group.md) da lista de grupos que foram marcados como incompatíveis em [um accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="37206-105">Remove a [group](../resources/group.md) from the list of groups that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="37206-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="37206-106">Permissions</span></span>

<span data-ttu-id="37206-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37206-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37206-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37206-109">Permission type</span></span>                        | <span data-ttu-id="37206-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37206-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="37206-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37206-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="37206-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37206-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="37206-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37206-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37206-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37206-114">Not supported.</span></span> |
| <span data-ttu-id="37206-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37206-115">Application</span></span>                            | <span data-ttu-id="37206-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37206-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37206-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37206-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="37206-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37206-118">Request headers</span></span>

| <span data-ttu-id="37206-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37206-119">Name</span></span>          | <span data-ttu-id="37206-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37206-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="37206-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37206-121">Authorization</span></span> | <span data-ttu-id="37206-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37206-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37206-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37206-124">Content-Type</span></span>  | <span data-ttu-id="37206-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37206-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37206-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37206-127">Request body</span></span>

<span data-ttu-id="37206-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37206-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37206-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="37206-129">Response</span></span>

<span data-ttu-id="37206-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37206-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37206-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37206-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37206-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37206-133">Request</span></span>

<span data-ttu-id="37206-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37206-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="37206-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="37206-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_incompatiblegroup_from_accesspackage"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="37206-136">C#</span><span class="sxs-lookup"><span data-stu-id="37206-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-incompatiblegroup-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37206-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37206-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-incompatiblegroup-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37206-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37206-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-incompatiblegroup-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37206-139">Java</span><span class="sxs-lookup"><span data-stu-id="37206-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-incompatiblegroup-from-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="37206-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="37206-140">Response</span></span>

<span data-ttu-id="37206-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37206-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove incompatibleGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


