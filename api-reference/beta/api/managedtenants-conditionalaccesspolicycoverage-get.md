---
title: Obter conditionalAccessPolicyCoverage
description: Leia as propriedades e as relações de um objeto conditionalAccessPolicyCoverage.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 1c3dffaea58476a30c28d05ea3aceeba750741e5
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440096"
---
# <a name="get-conditionalaccesspolicycoverage"></a><span data-ttu-id="79272-103">Obter conditionalAccessPolicyCoverage</span><span class="sxs-lookup"><span data-stu-id="79272-103">Get conditionalAccessPolicyCoverage</span></span>
<span data-ttu-id="79272-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="79272-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79272-105">Leia as propriedades e as relações de [um objeto conditionalAccessPolicyCoverage.](../resources/managedtenants-conditionalaccesspolicycoverage.md)</span><span class="sxs-lookup"><span data-stu-id="79272-105">Read the properties and relationships of a [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="79272-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="79272-106">Permissions</span></span>
<span data-ttu-id="79272-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79272-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79272-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79272-109">Permission type</span></span>|<span data-ttu-id="79272-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79272-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79272-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79272-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79272-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess e Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="79272-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess, and Application.Read.All</span></span>|
|<span data-ttu-id="79272-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79272-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79272-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79272-114">Not supported.</span></span>|
|<span data-ttu-id="79272-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79272-115">Application</span></span>|<span data-ttu-id="79272-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79272-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79272-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79272-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79272-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79272-118">Optional query parameters</span></span>
<span data-ttu-id="79272-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="79272-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79272-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79272-120">Request headers</span></span>
|<span data-ttu-id="79272-121">Nome</span><span class="sxs-lookup"><span data-stu-id="79272-121">Name</span></span>|<span data-ttu-id="79272-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="79272-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79272-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79272-123">Authorization</span></span>|<span data-ttu-id="79272-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79272-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79272-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79272-126">Request body</span></span>
<span data-ttu-id="79272-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79272-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79272-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="79272-128">Response</span></span>

<span data-ttu-id="79272-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79272-129">If successful, this method returns a `200 OK` response code and a [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79272-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="79272-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79272-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79272-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="79272-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="79272-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicycoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}
```
# <a name="c"></a>[<span data-ttu-id="79272-133">C#</span><span class="sxs-lookup"><span data-stu-id="79272-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conditionalaccesspolicycoverage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79272-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79272-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conditionalaccesspolicycoverage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79272-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79272-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conditionalaccesspolicycoverage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79272-136">Java</span><span class="sxs-lookup"><span data-stu-id="79272-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conditionalaccesspolicycoverage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="79272-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="79272-137">Response</span></span>
><span data-ttu-id="79272-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="79272-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.conditionalAccessPolicyCoverage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "id": "38227791-a88b-4fcc-81c5-58cf77668320",
  "conditionalAccessPolicyState": "enabled",
  "requiresDeviceCompliance": false,
  "latestPolicyModifiedDateTime": "2021-07-11T14:56:13.598304Z",
  "tenantDisplayName": "Consolidated Messenger"
}
```
