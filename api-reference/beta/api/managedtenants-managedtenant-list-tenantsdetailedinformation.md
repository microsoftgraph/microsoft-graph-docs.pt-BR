---
title: Listar tenantDetailedInformation
description: Obter uma lista dos objetos tenantDetailedInformation e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e9c1bfd7b460dbb093b308aa2b3f9d19ffe18f81
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402101"
---
# <a name="list-tenantdetailedinformation"></a><span data-ttu-id="89ede-103">Listar tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="89ede-103">List tenantDetailedInformation</span></span>
<span data-ttu-id="89ede-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="89ede-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89ede-105">Obter uma lista dos [objetos tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="89ede-105">Get a list of the [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="89ede-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="89ede-106">Permissions</span></span>
<span data-ttu-id="89ede-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89ede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ede-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89ede-109">Permission type</span></span>|<span data-ttu-id="89ede-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89ede-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89ede-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89ede-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89ede-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ede-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="89ede-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89ede-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89ede-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89ede-114">Not supported.</span></span>|
|<span data-ttu-id="89ede-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89ede-115">Application</span></span>|<span data-ttu-id="89ede-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89ede-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89ede-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89ede-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantsDetailedInformation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89ede-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="89ede-118">Optional query parameters</span></span>
<span data-ttu-id="89ede-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="89ede-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89ede-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89ede-120">Request headers</span></span>
|<span data-ttu-id="89ede-121">Nome</span><span class="sxs-lookup"><span data-stu-id="89ede-121">Name</span></span>|<span data-ttu-id="89ede-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="89ede-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="89ede-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89ede-123">Authorization</span></span>|<span data-ttu-id="89ede-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89ede-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89ede-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89ede-126">Request body</span></span>
<span data-ttu-id="89ede-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89ede-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89ede-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ede-128">Response</span></span>

<span data-ttu-id="89ede-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89ede-129">If successful, this method returns a `200 OK` response code and a collection of [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89ede-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89ede-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89ede-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89ede-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_tenantdetailedinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsDetailedInformation
```


### <a name="response"></a><span data-ttu-id="89ede-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ede-132">Response</span></span>
><span data-ttu-id="89ede-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="89ede-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
