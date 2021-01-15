---
title: Excluir connectedOrganization
description: Exclua connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8ce2aed28aaa4d1b97767e7ebb46e9b206d32d75
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872713"
---
# <a name="delete-connectedorganization"></a><span data-ttu-id="acd90-103">Excluir connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="acd90-103">Delete connectedOrganization</span></span>

<span data-ttu-id="acd90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acd90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acd90-105">[Exclua um objeto connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="acd90-105">Delete a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="acd90-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="acd90-106">Permissions</span></span>

<span data-ttu-id="acd90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acd90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acd90-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="acd90-109">Permission type</span></span>|<span data-ttu-id="acd90-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="acd90-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="acd90-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="acd90-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="acd90-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acd90-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="acd90-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="acd90-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acd90-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acd90-114">Not supported.</span></span> |
| <span data-ttu-id="acd90-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="acd90-115">Application</span></span>                            | <span data-ttu-id="acd90-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acd90-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="acd90-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acd90-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="acd90-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="acd90-118">Request headers</span></span>
|<span data-ttu-id="acd90-119">Nome</span><span class="sxs-lookup"><span data-stu-id="acd90-119">Name</span></span>|<span data-ttu-id="acd90-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="acd90-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="acd90-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="acd90-121">Authorization</span></span>|<span data-ttu-id="acd90-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acd90-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="acd90-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="acd90-124">Request body</span></span>
<span data-ttu-id="acd90-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="acd90-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acd90-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="acd90-126">Response</span></span>

<span data-ttu-id="acd90-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="acd90-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="acd90-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="acd90-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="acd90-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acd90-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="acd90-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="acd90-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```
# <a name="c"></a>[<span data-ttu-id="acd90-131">C#</span><span class="sxs-lookup"><span data-stu-id="acd90-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acd90-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acd90-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acd90-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acd90-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="acd90-134">Java</span><span class="sxs-lookup"><span data-stu-id="acd90-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="acd90-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="acd90-135">Response</span></span>
<span data-ttu-id="acd90-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="acd90-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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


