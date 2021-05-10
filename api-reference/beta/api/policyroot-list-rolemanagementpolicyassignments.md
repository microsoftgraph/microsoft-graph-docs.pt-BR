---
title: Listar roleManagementPolicyAssignments
description: Obter os recursos de navegação unifiedRoleManagementPolicyAssignment da propriedade de navegação roleManagementPolicyAssignments.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b16faca5c197fd4e5b2b76639be3778d1d3fc2c2
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299096"
---
# <a name="list-rolemanagementpolicyassignments"></a><span data-ttu-id="ec648-103">Listar roleManagementPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="ec648-103">List roleManagementPolicyAssignments</span></span>
<span data-ttu-id="ec648-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec648-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec648-105">Obter os recursos de navegação unifiedRoleManagementPolicyAssignment da propriedade de navegação roleManagementPolicyAssignments.</span><span class="sxs-lookup"><span data-stu-id="ec648-105">Get the unifiedRoleManagementPolicyAssignment resources from the roleManagementPolicyAssignments navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec648-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec648-106">Permissions</span></span>
<span data-ttu-id="ec648-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec648-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec648-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec648-109">Permission type</span></span>|<span data-ttu-id="ec648-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec648-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec648-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec648-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ec648-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ec648-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="ec648-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec648-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec648-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ec648-114">Not supported</span></span>|
|<span data-ttu-id="ec648-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec648-115">Application</span></span>|<span data-ttu-id="ec648-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ec648-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec648-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec648-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicyAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec648-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ec648-118">Optional query parameters</span></span>
<span data-ttu-id="ec648-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ec648-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ec648-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ec648-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec648-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec648-121">Request headers</span></span>
|<span data-ttu-id="ec648-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ec648-122">Name</span></span>|<span data-ttu-id="ec648-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec648-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ec648-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec648-124">Authorization</span></span>|<span data-ttu-id="ec648-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec648-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec648-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec648-127">Request body</span></span>
<span data-ttu-id="ec648-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec648-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec648-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec648-129">Response</span></span>

<span data-ttu-id="ec648-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec648-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec648-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ec648-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec648-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec648-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicyAssignments
```


### <a name="response"></a><span data-ttu-id="ec648-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec648-133">Response</span></span>
<span data-ttu-id="ec648-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ec648-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

