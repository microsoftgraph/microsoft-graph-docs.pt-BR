---
title: Obter unifiedRoleManagementPolicyAssignment
description: Leia as propriedades e as relações de um objeto unifiedRoleManagementPolicyAssignment.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c5efdf8e2890651c8629efb27837ffb1953c1376
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682303"
---
# <a name="get-unifiedrolemanagementpolicyassignment"></a><span data-ttu-id="c1b16-103">Obter unifiedRoleManagementPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="c1b16-103">Get unifiedRoleManagementPolicyAssignment</span></span>
<span data-ttu-id="c1b16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1b16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1b16-105">Leia as propriedades e as relações de [um objeto unifiedRoleManagementPolicyAssignment.](../resources/unifiedrolemanagementpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c1b16-105">Read the properties and relationships of an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1b16-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1b16-106">Permissions</span></span>
<span data-ttu-id="c1b16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1b16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1b16-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1b16-109">Permission type</span></span>|<span data-ttu-id="c1b16-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1b16-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1b16-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1b16-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c1b16-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="c1b16-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="c1b16-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1b16-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1b16-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c1b16-114">Not supported</span></span>|
|<span data-ttu-id="c1b16-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1b16-115">Application</span></span>|<span data-ttu-id="c1b16-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="c1b16-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1b16-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1b16-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicyAssignments/{unifiedRoleManagementPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1b16-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c1b16-118">Optional query parameters</span></span>
<span data-ttu-id="c1b16-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c1b16-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c1b16-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c1b16-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1b16-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1b16-121">Request headers</span></span>
|<span data-ttu-id="c1b16-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c1b16-122">Name</span></span>|<span data-ttu-id="c1b16-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1b16-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c1b16-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1b16-124">Authorization</span></span>|<span data-ttu-id="c1b16-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1b16-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1b16-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1b16-127">Request body</span></span>
<span data-ttu-id="c1b16-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c1b16-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1b16-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1b16-129">Response</span></span>

<span data-ttu-id="c1b16-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1b16-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1b16-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c1b16-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c1b16-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1b16-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c1b16-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1b16-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicyassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicyAssignments/d6e4112f-112f-d6e4-2f11-e4d62f11e4d6
```
# <a name="c"></a>[<span data-ttu-id="c1b16-134">C#</span><span class="sxs-lookup"><span data-stu-id="c1b16-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedrolemanagementpolicyassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1b16-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1b16-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedrolemanagementpolicyassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1b16-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1b16-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedrolemanagementpolicyassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1b16-137">Java</span><span class="sxs-lookup"><span data-stu-id="c1b16-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedrolemanagementpolicyassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c1b16-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1b16-138">Response</span></span>
<span data-ttu-id="c1b16-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c1b16-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "policyId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "scopeId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "scopeType": "subscription",
    "roleDefinitionId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6"
  }
}
```

