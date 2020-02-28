---
title: Criar accessPackageAssignmentPolicy
description: Use esta API para criar um novo accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ffa1b1ac1519c933e9ca352ec90b45a5161d2a43
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331180"
---
# <a name="create-accesspackageassignmentpolicy"></a><span data-ttu-id="c18b9-103">Criar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="c18b9-103">Create accessPackageAssignmentPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c18b9-104">No [Gerenciamento de qualificação do Azure ad](../resources/entitlementmanagement-root.md), use esta API para criar um novo objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="c18b9-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), use this API to create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c18b9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c18b9-105">Permissions</span></span>

<span data-ttu-id="c18b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c18b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c18b9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c18b9-108">Permission type</span></span>                        | <span data-ttu-id="c18b9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c18b9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c18b9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c18b9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c18b9-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c18b9-111">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="c18b9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c18b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c18b9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c18b9-113">Not supported.</span></span> |
| <span data-ttu-id="c18b9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c18b9-114">Application</span></span>                            | <span data-ttu-id="c18b9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c18b9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c18b9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c18b9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c18b9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c18b9-117">Request headers</span></span>

| <span data-ttu-id="c18b9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c18b9-118">Name</span></span>          | <span data-ttu-id="c18b9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c18b9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c18b9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c18b9-120">Authorization</span></span> | <span data-ttu-id="c18b9-121">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="c18b9-121">Bearer \{token\}.</span></span> <span data-ttu-id="c18b9-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c18b9-122">Required.</span></span> |
| <span data-ttu-id="c18b9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c18b9-123">Content-Type</span></span>  | <span data-ttu-id="c18b9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c18b9-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c18b9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c18b9-125">Request body</span></span>

<span data-ttu-id="c18b9-126">No corpo da solicitação, forneça uma representação JSON do objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="c18b9-126">In the request body, supply a JSON representation of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c18b9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c18b9-127">Response</span></span>

<span data-ttu-id="c18b9-128">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c18b9-128">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c18b9-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c18b9-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c18b9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c18b9-130">Request</span></span>

<span data-ttu-id="c18b9-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c18b9-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c18b9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c18b9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator",
  "isDenyPolicy": false,
  "accessReviewSettings": null,
  "requestorSettings": {
    "scopeType": "NoSubjects",
    "acceptRequests": true,
    "allowedRequestors": []
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```
# <a name="c"></a>[<span data-ttu-id="c18b9-133">C#</span><span class="sxs-lookup"><span data-stu-id="c18b9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c18b9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c18b9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c18b9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c18b9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c18b9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c18b9-136">Response</span></span>

<span data-ttu-id="c18b9-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c18b9-137">The following is an example of the response.</span></span>

> <span data-ttu-id="c18b9-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c18b9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "4c02f928-7752-49aa-8fc8-e286d973a965",
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator",
  "isDenyPolicy": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
