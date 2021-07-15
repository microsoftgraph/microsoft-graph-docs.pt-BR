---
title: Listar conditionalAccessPolicyCoverages
description: Obter uma lista dos objetos conditionalAccessPolicyCoverage e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a35b7032b4b1fb19b73ff4110a4b43af3c388487
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442639"
---
# <a name="list-conditionalaccesspolicycoverages"></a><span data-ttu-id="eecdd-103">Listar conditionalAccessPolicyCoverages</span><span class="sxs-lookup"><span data-stu-id="eecdd-103">List conditionalAccessPolicyCoverages</span></span>
<span data-ttu-id="eecdd-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="eecdd-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eecdd-105">Obter uma lista dos [objetos conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="eecdd-105">Get a list of the [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects and their properties.</span></span> <span data-ttu-id="eecdd-106">Use essa operação para listar Azure Active Directory de política de acesso condicional em todos os locatários que estão sendo gerenciados pela plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="eecdd-106">Use this operation to list of Azure Active Directory conditional access policy coverage across all tenants that are being managed by the multi-tenant management platform.</span></span>

## <a name="permissions"></a><span data-ttu-id="eecdd-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="eecdd-107">Permissions</span></span>
<span data-ttu-id="eecdd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eecdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eecdd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eecdd-110">Permission type</span></span>|<span data-ttu-id="eecdd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eecdd-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eecdd-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eecdd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eecdd-113">Policy.Read.All, Policy.ReadWrite.ConditionalAccess e Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="eecdd-113">Policy.Read.All, Policy.ReadWrite.ConditionalAccess, and Application.Read.All</span></span>|
|<span data-ttu-id="eecdd-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eecdd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eecdd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eecdd-115">Not supported.</span></span>|
|<span data-ttu-id="eecdd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eecdd-116">Application</span></span>|<span data-ttu-id="eecdd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eecdd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eecdd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eecdd-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/conditionalAccessPolicyCoverages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eecdd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eecdd-119">Optional query parameters</span></span>
<span data-ttu-id="eecdd-120">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="eecdd-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eecdd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eecdd-121">Request headers</span></span>
|<span data-ttu-id="eecdd-122">Nome</span><span class="sxs-lookup"><span data-stu-id="eecdd-122">Name</span></span>|<span data-ttu-id="eecdd-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="eecdd-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eecdd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="eecdd-124">Authorization</span></span>|<span data-ttu-id="eecdd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eecdd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eecdd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eecdd-127">Request body</span></span>
<span data-ttu-id="eecdd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eecdd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eecdd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="eecdd-129">Response</span></span>

<span data-ttu-id="eecdd-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eecdd-130">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eecdd-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eecdd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eecdd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eecdd-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eecdd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="eecdd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conditionalaccesspolicycoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages
```
# <a name="c"></a>[<span data-ttu-id="eecdd-134">C#</span><span class="sxs-lookup"><span data-stu-id="eecdd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conditionalaccesspolicycoverage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eecdd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eecdd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conditionalaccesspolicycoverage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eecdd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eecdd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conditionalaccesspolicycoverage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eecdd-137">Java</span><span class="sxs-lookup"><span data-stu-id="eecdd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-conditionalaccesspolicycoverage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="eecdd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="eecdd-138">Response</span></span>
><span data-ttu-id="eecdd-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eecdd-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.conditionalAccessPolicyCoverage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "conditionalAccessPolicyState": "enabled",
      "requiresDeviceCompliance": false,
      "latestPolicyModifiedDateTime": "2021-07-11T14:56:13.598304Z",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```
