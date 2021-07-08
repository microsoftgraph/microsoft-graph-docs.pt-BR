---
title: Listar unifiedRoleManagementPolicyAssignments
description: Obter uma lista dos objetos unifiedRoleManagementPolicyAssignment e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c6f67fd562623e6f195c9ae0a6bfd9cc96096f45
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334630"
---
# <a name="list-unifiedrolemanagementpolicyassignments"></a><span data-ttu-id="fabcd-103">Listar unifiedRoleManagementPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="fabcd-103">List unifiedRoleManagementPolicyAssignments</span></span>
<span data-ttu-id="fabcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fabcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fabcd-105">Obter uma lista dos [objetos unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="fabcd-105">Get a list of the [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="fabcd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fabcd-106">Permissions</span></span>
<span data-ttu-id="fabcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fabcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fabcd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fabcd-109">Permission type</span></span>|<span data-ttu-id="fabcd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fabcd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fabcd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fabcd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fabcd-112">RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="fabcd-112">RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="fabcd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fabcd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fabcd-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fabcd-114">Not supported</span></span>|
|<span data-ttu-id="fabcd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fabcd-115">Application</span></span>|<span data-ttu-id="fabcd-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="fabcd-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="fabcd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fabcd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicyAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fabcd-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fabcd-118">Optional query parameters</span></span>
<span data-ttu-id="fabcd-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fabcd-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fabcd-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fabcd-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fabcd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fabcd-121">Request headers</span></span>
|<span data-ttu-id="fabcd-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fabcd-122">Name</span></span>|<span data-ttu-id="fabcd-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fabcd-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fabcd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fabcd-124">Authorization</span></span>|<span data-ttu-id="fabcd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fabcd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fabcd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fabcd-127">Request body</span></span>
<span data-ttu-id="fabcd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fabcd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fabcd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fabcd-129">Response</span></span>

<span data-ttu-id="fabcd-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fabcd-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fabcd-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fabcd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fabcd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fabcd-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fabcd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fabcd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicyAssignments
```
# <a name="c"></a>[<span data-ttu-id="fabcd-134">C#</span><span class="sxs-lookup"><span data-stu-id="fabcd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicyassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fabcd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fabcd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicyassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fabcd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fabcd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicyassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fabcd-137">Java</span><span class="sxs-lookup"><span data-stu-id="fabcd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicyassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fabcd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fabcd-138">Response</span></span>
<span data-ttu-id="fabcd-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fabcd-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicyAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
      "policyId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
      "scopeId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
      "scopeType": "subscription",
      "roleDefinitionId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6"
    }
  ]
}
```

