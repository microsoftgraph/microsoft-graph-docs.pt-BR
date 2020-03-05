---
title: Excluir accessPackageAssignmentPolicy
description: Excluir um accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 74d3416fbffe95d558f75c00bf55ef60523cb3c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448461"
---
# <a name="delete-accesspackageassignmentpolicy"></a><span data-ttu-id="069d9-103">Excluir accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="069d9-103">Delete accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="069d9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="069d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="069d9-105">Em [Gerenciamento de qualificação do Azure ad](../resources/entitlementmanagement-root.md), exclua um [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="069d9-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), delete an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="069d9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="069d9-106">Permissions</span></span>

<span data-ttu-id="069d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="069d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="069d9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="069d9-109">Permission type</span></span>                        | <span data-ttu-id="069d9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="069d9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="069d9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="069d9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="069d9-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="069d9-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="069d9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="069d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="069d9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="069d9-114">Not supported.</span></span> |
| <span data-ttu-id="069d9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="069d9-115">Application</span></span>                            | <span data-ttu-id="069d9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="069d9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="069d9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="069d9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="069d9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="069d9-118">Request headers</span></span>

| <span data-ttu-id="069d9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="069d9-119">Name</span></span>          | <span data-ttu-id="069d9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="069d9-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="069d9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="069d9-121">Authorization</span></span> | <span data-ttu-id="069d9-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="069d9-122">Bearer \{token\}.</span></span> <span data-ttu-id="069d9-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="069d9-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="069d9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="069d9-124">Request body</span></span>

<span data-ttu-id="069d9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="069d9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="069d9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="069d9-126">Response</span></span>

<span data-ttu-id="069d9-127">Se tiver êxito, este método retornará um código de resposta de conteúdo de 204.</span><span class="sxs-lookup"><span data-stu-id="069d9-127">If successful, this method returns a 204 No Content response code.</span></span> <span data-ttu-id="069d9-128">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="069d9-128">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="069d9-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="069d9-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="069d9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="069d9-130">Request</span></span>

<span data-ttu-id="069d9-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="069d9-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="069d9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="069d9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackageassignmentpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="069d9-133">C#</span><span class="sxs-lookup"><span data-stu-id="069d9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="069d9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="069d9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="069d9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="069d9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="069d9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="069d9-136">Response</span></span>

<span data-ttu-id="069d9-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="069d9-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
