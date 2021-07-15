---
title: Obter tenantCustomizedInformation
description: Leia as propriedades e as relações de um objeto tenantCustomizedInformation.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 2561111648b226fe598d9e86be677596dc1b709d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440307"
---
# <a name="get-tenantcustomizedinformation"></a><span data-ttu-id="81cce-103">Obter tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="81cce-103">Get tenantCustomizedInformation</span></span>
<span data-ttu-id="81cce-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="81cce-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81cce-105">Leia as propriedades e as relações de um [objeto tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="81cce-105">Read the properties and relationships of a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81cce-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="81cce-106">Permissions</span></span>
<span data-ttu-id="81cce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81cce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81cce-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81cce-109">Permission type</span></span>|<span data-ttu-id="81cce-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81cce-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81cce-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81cce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81cce-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81cce-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="81cce-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81cce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81cce-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81cce-114">Not supported.</span></span>|
|<span data-ttu-id="81cce-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81cce-115">Application</span></span>|<span data-ttu-id="81cce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81cce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81cce-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81cce-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81cce-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="81cce-118">Optional query parameters</span></span>
<span data-ttu-id="81cce-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="81cce-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81cce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81cce-120">Request headers</span></span>
|<span data-ttu-id="81cce-121">Nome</span><span class="sxs-lookup"><span data-stu-id="81cce-121">Name</span></span>|<span data-ttu-id="81cce-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="81cce-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="81cce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="81cce-123">Authorization</span></span>|<span data-ttu-id="81cce-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81cce-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81cce-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81cce-126">Request body</span></span>
<span data-ttu-id="81cce-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81cce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81cce-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="81cce-128">Response</span></span>

<span data-ttu-id="81cce-129">Se tiver êxito, este método retornará um código de `200 OK` resposta e um objeto [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81cce-129">If successful, this method returns a `200 OK` response code and a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81cce-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="81cce-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81cce-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81cce-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="81cce-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="81cce-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tenantcustomizedinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
```
# <a name="c"></a>[<span data-ttu-id="81cce-133">C#</span><span class="sxs-lookup"><span data-stu-id="81cce-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tenantcustomizedinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81cce-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81cce-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tenantcustomizedinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81cce-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81cce-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tenantcustomizedinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81cce-136">Java</span><span class="sxs-lookup"><span data-stu-id="81cce-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tenantcustomizedinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="81cce-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="81cce-137">Response</span></span>
><span data-ttu-id="81cce-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="81cce-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantCustomizedInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "website": "https://www.fourthcoffee.com",
  "contacts": [
    {
      "name": "Sally",
      "email": "sally@fourthcoffee.com",
      "phone": "5558009731"
    },
    {
      "name": "Hector",
      "email": "hector@fourthcoffee.com",
      "phone": "5558009732"
    }
  ]
}
```
