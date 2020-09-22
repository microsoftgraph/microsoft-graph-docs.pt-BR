---
title: Excluir connectedOrganization
description: Exclua connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b26e7a2d872e75217a0a4fc0a40e9e88df197310
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996527"
---
# <a name="delete-connectedorganization"></a><span data-ttu-id="1eb03-103">Excluir connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="1eb03-103">Delete connectedOrganization</span></span>

<span data-ttu-id="1eb03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1eb03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1eb03-105">Excluir um objeto [connectedOrganization](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="1eb03-105">Delete a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1eb03-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1eb03-106">Permissions</span></span>

<span data-ttu-id="1eb03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1eb03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1eb03-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1eb03-109">Permission type</span></span>|<span data-ttu-id="1eb03-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1eb03-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="1eb03-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1eb03-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1eb03-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eb03-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="1eb03-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1eb03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1eb03-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1eb03-114">Not supported.</span></span> |
| <span data-ttu-id="1eb03-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1eb03-115">Application</span></span>                            | <span data-ttu-id="1eb03-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1eb03-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1eb03-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1eb03-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1eb03-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb03-118">Request headers</span></span>
|<span data-ttu-id="1eb03-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1eb03-119">Name</span></span>|<span data-ttu-id="1eb03-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1eb03-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1eb03-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1eb03-121">Authorization</span></span>|<span data-ttu-id="1eb03-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1eb03-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1eb03-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb03-124">Request body</span></span>
<span data-ttu-id="1eb03-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1eb03-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1eb03-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb03-126">Response</span></span>

<span data-ttu-id="1eb03-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1eb03-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1eb03-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1eb03-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1eb03-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb03-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1eb03-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="1eb03-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```
# <a name="c"></a>[<span data-ttu-id="1eb03-131">C#</span><span class="sxs-lookup"><span data-stu-id="1eb03-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1eb03-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1eb03-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1eb03-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1eb03-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1eb03-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb03-134">Response</span></span>
<span data-ttu-id="1eb03-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1eb03-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


