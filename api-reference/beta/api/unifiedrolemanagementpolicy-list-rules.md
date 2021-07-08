---
title: Listar regras
description: Obter os recursos unifiedRoleManagementPolicyRule da propriedade de navegação de regras.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c129ed8467e558fa63ceb550489b5a3240051587
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334651"
---
# <a name="list-rules"></a><span data-ttu-id="2ba14-103">Listar regras</span><span class="sxs-lookup"><span data-stu-id="2ba14-103">List rules</span></span>
<span data-ttu-id="2ba14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ba14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ba14-105">Obter os recursos unifiedRoleManagementPolicyRule da propriedade de navegação de regras.</span><span class="sxs-lookup"><span data-stu-id="2ba14-105">Get the unifiedRoleManagementPolicyRule resources from the rules navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ba14-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ba14-106">Permissions</span></span>
<span data-ttu-id="2ba14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ba14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ba14-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ba14-109">Permission type</span></span>|<span data-ttu-id="2ba14-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ba14-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ba14-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ba14-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2ba14-112">RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="2ba14-112">RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="2ba14-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ba14-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ba14-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2ba14-114">Not supported</span></span>|
|<span data-ttu-id="2ba14-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ba14-115">Application</span></span>|<span data-ttu-id="2ba14-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="2ba14-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ba14-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ba14-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ba14-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ba14-118">Optional query parameters</span></span>
<span data-ttu-id="2ba14-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2ba14-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2ba14-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2ba14-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ba14-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ba14-121">Request headers</span></span>
|<span data-ttu-id="2ba14-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2ba14-122">Name</span></span>|<span data-ttu-id="2ba14-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ba14-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2ba14-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ba14-124">Authorization</span></span>|<span data-ttu-id="2ba14-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ba14-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ba14-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ba14-127">Request body</span></span>
<span data-ttu-id="2ba14-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ba14-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ba14-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ba14-129">Response</span></span>

<span data-ttu-id="2ba14-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ba14-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ba14-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2ba14-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ba14-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ba14-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2ba14-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ba14-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba/rules
```
# <a name="c"></a>[<span data-ttu-id="2ba14-134">C#</span><span class="sxs-lookup"><span data-stu-id="2ba14-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ba14-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ba14-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ba14-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ba14-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ba14-137">Java</span><span class="sxs-lookup"><span data-stu-id="2ba14-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2ba14-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ba14-138">Response</span></span>
<span data-ttu-id="2ba14-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2ba14-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicyRule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba",
      "target": {
        "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
      }
    }
  ]
}
```

