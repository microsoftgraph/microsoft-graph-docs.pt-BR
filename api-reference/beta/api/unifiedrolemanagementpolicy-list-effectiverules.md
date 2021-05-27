---
title: Listar effectiveRules
description: Obter os recursos unifiedRoleManagementPolicyRule da propriedade de navegação effectiveRules.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7dcc8a410d7ae47552c6c5d294334e64e1721124
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682338"
---
# <a name="list-effectiverules"></a><span data-ttu-id="60d8c-103">Listar effectiveRules</span><span class="sxs-lookup"><span data-stu-id="60d8c-103">List effectiveRules</span></span>
<span data-ttu-id="60d8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60d8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60d8c-105">Obter os recursos unifiedRoleManagementPolicyRule da propriedade de navegação effectiveRules.</span><span class="sxs-lookup"><span data-stu-id="60d8c-105">Get the unifiedRoleManagementPolicyRule resources from the effectiveRules navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="60d8c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="60d8c-106">Permissions</span></span>
<span data-ttu-id="60d8c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60d8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60d8c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60d8c-109">Permission type</span></span>|<span data-ttu-id="60d8c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60d8c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60d8c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60d8c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="60d8c-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="60d8c-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="60d8c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60d8c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60d8c-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="60d8c-114">Not supported</span></span>|
|<span data-ttu-id="60d8c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60d8c-115">Application</span></span>|<span data-ttu-id="60d8c-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="60d8c-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="60d8c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60d8c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60d8c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="60d8c-118">Optional query parameters</span></span>
<span data-ttu-id="60d8c-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="60d8c-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="60d8c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="60d8c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="60d8c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60d8c-121">Request headers</span></span>
|<span data-ttu-id="60d8c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="60d8c-122">Name</span></span>|<span data-ttu-id="60d8c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="60d8c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="60d8c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="60d8c-124">Authorization</span></span>|<span data-ttu-id="60d8c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60d8c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60d8c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60d8c-127">Request body</span></span>
<span data-ttu-id="60d8c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60d8c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60d8c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="60d8c-129">Response</span></span>

<span data-ttu-id="60d8c-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60d8c-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60d8c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="60d8c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60d8c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60d8c-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="60d8c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="60d8c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba/effectiveRules
```
# <a name="c"></a>[<span data-ttu-id="60d8c-134">C#</span><span class="sxs-lookup"><span data-stu-id="60d8c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60d8c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60d8c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60d8c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60d8c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60d8c-137">Java</span><span class="sxs-lookup"><span data-stu-id="60d8c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="60d8c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="60d8c-138">Response</span></span>
<span data-ttu-id="60d8c-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="60d8c-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

