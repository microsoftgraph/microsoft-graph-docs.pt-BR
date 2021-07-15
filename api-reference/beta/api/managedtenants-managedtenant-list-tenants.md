---
title: Listar locatários
description: Obter uma lista dos objetos de locatário e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 2ffea17f39ee0db99b3b9aa964c73ccd5763f909
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440768"
---
# <a name="list-tenants"></a><span data-ttu-id="20d55-103">Listar locatários</span><span class="sxs-lookup"><span data-stu-id="20d55-103">List tenants</span></span>
<span data-ttu-id="20d55-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="20d55-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20d55-105">Obter uma lista dos objetos [de locatário](../resources/managedtenants-tenant.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="20d55-105">Get a list of the [tenant](../resources/managedtenants-tenant.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="20d55-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="20d55-106">Permissions</span></span>
<span data-ttu-id="20d55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20d55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20d55-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20d55-109">Permission type</span></span>|<span data-ttu-id="20d55-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20d55-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20d55-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20d55-111">Delegated (work or school account)</span></span>|<span data-ttu-id="20d55-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d55-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="20d55-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20d55-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20d55-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20d55-114">Not supported.</span></span>|
|<span data-ttu-id="20d55-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20d55-115">Application</span></span>|<span data-ttu-id="20d55-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20d55-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20d55-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20d55-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20d55-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20d55-118">Optional query parameters</span></span>
<span data-ttu-id="20d55-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="20d55-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20d55-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20d55-120">Request headers</span></span>
|<span data-ttu-id="20d55-121">Nome</span><span class="sxs-lookup"><span data-stu-id="20d55-121">Name</span></span>|<span data-ttu-id="20d55-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="20d55-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="20d55-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="20d55-123">Authorization</span></span>|<span data-ttu-id="20d55-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20d55-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20d55-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20d55-126">Request body</span></span>
<span data-ttu-id="20d55-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20d55-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20d55-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="20d55-128">Response</span></span>

<span data-ttu-id="20d55-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [locatários](../resources/managedtenants-tenant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20d55-129">If successful, this method returns a `200 OK` response code and a collection of [tenant](../resources/managedtenants-tenant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20d55-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20d55-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20d55-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20d55-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="20d55-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="20d55-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tenant"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants
```
# <a name="c"></a>[<span data-ttu-id="20d55-133">C#</span><span class="sxs-lookup"><span data-stu-id="20d55-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20d55-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20d55-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20d55-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20d55-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20d55-136">Java</span><span class="sxs-lookup"><span data-stu-id="20d55-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tenant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="20d55-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="20d55-137">Response</span></span>
><span data-ttu-id="20d55-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="20d55-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenant)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "contract": {
        "displayName": "Fourth Coffee",
        "defaultDomainName": "fourthcoffe01.onmicrosoft.com",
        "contractType": 2
      },
      "tenantStatusInformation": {
        "onboardingStatus": "ineligible",
        "onboardingDateTime": "2012-02-20T00:00:00Z",
        "onboardedByUserId": "",
        "offboardedDateTime": "2012-02-20T00:00:00Z",
        "offboardedBy": "",
        "delegatedPrivilegeStatus": "delegatedAdminPrivileges",
        "workloadStatuses": [
          {
            "displayName": "Device Management",
            "onboardingStatus": "onboarded",
            "onboardedDateTime": "2012-02-20T00:00:00Z",
            "offboardedDateTime": null
          },
          {
            "displayName": "Cloud PC",
            "onboardingStatus": "notOnboarded",
            "onboardedDateTime": "2012-02-20T00:00:00Z",
            "offboardedDateTime": null
          }
        ]
      },
      "createdDateTime": "2012-02-20T00:00:00Z",
      "lastUpdatedDatetime": "2021-02-20T00:00:00Z"
    }
  ]
}
```
