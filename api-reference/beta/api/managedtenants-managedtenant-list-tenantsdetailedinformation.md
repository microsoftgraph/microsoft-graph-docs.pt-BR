---
title: Listar tenantDetailedInformation
description: Obter uma lista dos objetos tenantDetailedInformation e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 3841183b9a11ab1d9112b94cc9dab00ae24457dc
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440579"
---
# <a name="list-tenantdetailedinformation"></a><span data-ttu-id="28bd3-103">Listar tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="28bd3-103">List tenantDetailedInformation</span></span>
<span data-ttu-id="28bd3-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="28bd3-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28bd3-105">Obter uma lista dos [objetos tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="28bd3-105">Get a list of the [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="28bd3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="28bd3-106">Permissions</span></span>
<span data-ttu-id="28bd3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28bd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28bd3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28bd3-109">Permission type</span></span>|<span data-ttu-id="28bd3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28bd3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28bd3-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28bd3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="28bd3-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28bd3-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="28bd3-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28bd3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28bd3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28bd3-114">Not supported.</span></span>|
|<span data-ttu-id="28bd3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28bd3-115">Application</span></span>|<span data-ttu-id="28bd3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28bd3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28bd3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28bd3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantsDetailedInformation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28bd3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28bd3-118">Optional query parameters</span></span>
<span data-ttu-id="28bd3-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="28bd3-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28bd3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28bd3-120">Request headers</span></span>
|<span data-ttu-id="28bd3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="28bd3-121">Name</span></span>|<span data-ttu-id="28bd3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="28bd3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="28bd3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="28bd3-123">Authorization</span></span>|<span data-ttu-id="28bd3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28bd3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28bd3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28bd3-126">Request body</span></span>
<span data-ttu-id="28bd3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28bd3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28bd3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="28bd3-128">Response</span></span>

<span data-ttu-id="28bd3-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28bd3-129">If successful, this method returns a `200 OK` response code and a collection of [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28bd3-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="28bd3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="28bd3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28bd3-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="28bd3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="28bd3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tenantdetailedinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsDetailedInformation
```
# <a name="c"></a>[<span data-ttu-id="28bd3-133">C#</span><span class="sxs-lookup"><span data-stu-id="28bd3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tenantdetailedinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28bd3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28bd3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tenantdetailedinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28bd3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28bd3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tenantdetailedinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28bd3-136">Java</span><span class="sxs-lookup"><span data-stu-id="28bd3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tenantdetailedinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="28bd3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="28bd3-137">Response</span></span>
><span data-ttu-id="28bd3-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="28bd3-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantDetailedInformation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/managedTenants/$metadata#tenantDetailedInformation",
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "companyName": "Fourth Coffee",
      "defaultDomainName": "fourthcoffee001.onmicrosoft.com",
      "countryName": "United States",
      "countryCode": "US",
      "city": "Redmond",
      "region": "NA",
      "verticalName": "Software",
      "industryName": "Computer",
      "segmentName": "Service"
    },
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "companyName": "Consolidated Messenger",
      "defaultDomainName": "consoldiatedmessenger001.onmicrosoft.com",
      "countryName": "United States",
      "countryCode": "US",
      "city": "Redmond",
      "region": "NA",
      "verticalName": "Software",
      "industryName": "Computer",
      "segmentName": "Service"
    }
  ]
}
```
