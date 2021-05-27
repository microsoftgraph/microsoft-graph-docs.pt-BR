---
title: Listar unifiedRoleManagementPolicyRules
description: Obter uma lista dos objetos unifiedRoleManagementPolicyRule e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bc0f1fa8627f6a3ff49891aae9ddaf702f46c821
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680224"
---
# <a name="list-unifiedrolemanagementpolicyrules"></a><span data-ttu-id="fa2f1-103">Listar unifiedRoleManagementPolicyRules</span><span class="sxs-lookup"><span data-stu-id="fa2f1-103">List unifiedRoleManagementPolicyRules</span></span>
<span data-ttu-id="fa2f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa2f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fa2f1-105">Obter uma lista dos [objetos unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="fa2f1-105">Get a list of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa2f1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa2f1-106">Permissions</span></span>
<span data-ttu-id="fa2f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa2f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa2f1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa2f1-109">Permission type</span></span>|<span data-ttu-id="fa2f1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa2f1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa2f1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa2f1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa2f1-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="fa2f1-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="fa2f1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa2f1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa2f1-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fa2f1-114">Not supported</span></span>|
|<span data-ttu-id="fa2f1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa2f1-115">Application</span></span>|<span data-ttu-id="fa2f1-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="fa2f1-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa2f1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa2f1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa2f1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa2f1-118">Optional query parameters</span></span>
<span data-ttu-id="fa2f1-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fa2f1-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fa2f1-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fa2f1-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa2f1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa2f1-121">Request headers</span></span>
|<span data-ttu-id="fa2f1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fa2f1-122">Name</span></span>|<span data-ttu-id="fa2f1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa2f1-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fa2f1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa2f1-124">Authorization</span></span>|<span data-ttu-id="fa2f1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa2f1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa2f1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa2f1-127">Request body</span></span>
<span data-ttu-id="fa2f1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa2f1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa2f1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa2f1-129">Response</span></span>

<span data-ttu-id="fa2f1-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa2f1-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa2f1-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fa2f1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa2f1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa2f1-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fa2f1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa2f1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules
```
# <a name="c"></a>[<span data-ttu-id="fa2f1-134">C#</span><span class="sxs-lookup"><span data-stu-id="fa2f1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa2f1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa2f1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa2f1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa2f1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa2f1-137">Java</span><span class="sxs-lookup"><span data-stu-id="fa2f1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fa2f1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa2f1-138">Response</span></span>
<span data-ttu-id="fa2f1-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fa2f1-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

