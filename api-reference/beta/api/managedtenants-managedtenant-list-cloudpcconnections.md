---
title: Listar cloudPcConnections
description: Obter uma lista dos objetos cloudPcConnection e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: eca2e9437c9f1fd200516fb76cd00923ba10e23a
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401919"
---
# <a name="list-cloudpcconnections"></a><span data-ttu-id="24d3c-103">Listar cloudPcConnections</span><span class="sxs-lookup"><span data-stu-id="24d3c-103">List cloudPcConnections</span></span>
<span data-ttu-id="24d3c-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="24d3c-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24d3c-105">Obter uma lista dos objetos [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="24d3c-105">Get a list of the [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="24d3c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="24d3c-106">Permissions</span></span>
<span data-ttu-id="24d3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24d3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24d3c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24d3c-109">Permission type</span></span>|<span data-ttu-id="24d3c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24d3c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24d3c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24d3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="24d3c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24d3c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="24d3c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24d3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24d3c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24d3c-114">Not supported.</span></span>|
|<span data-ttu-id="24d3c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24d3c-115">Application</span></span>|<span data-ttu-id="24d3c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24d3c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24d3c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24d3c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcConnections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24d3c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24d3c-118">Optional query parameters</span></span>
<span data-ttu-id="24d3c-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="24d3c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24d3c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24d3c-120">Request headers</span></span>
|<span data-ttu-id="24d3c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="24d3c-121">Name</span></span>|<span data-ttu-id="24d3c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="24d3c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="24d3c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="24d3c-123">Authorization</span></span>|<span data-ttu-id="24d3c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24d3c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24d3c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24d3c-126">Request body</span></span>
<span data-ttu-id="24d3c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24d3c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24d3c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="24d3c-128">Response</span></span>

<span data-ttu-id="24d3c-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24d3c-129">If successful, this method returns a `200 OK` response code and a collection of [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24d3c-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="24d3c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24d3c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24d3c-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_cloudpcconnection"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcConnections
```


### <a name="response"></a><span data-ttu-id="24d3c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="24d3c-132">Response</span></span>
><span data-ttu-id="24d3c-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24d3c-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.cloudPcConnection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/cloudPcConnections",
  "value": [
    {
      "id": "021bd3a9-59c6-4503-b408-c326a98f238f",
      "lastUpdated": "2021-07-11T18:02:16.6450704Z",
      "displayName": "RunnerPlus-Az-Connection",
      "organizationId": "0b9701e1-f1ae-4f15-bd67-f4f591595454",
      "organizationDisplayName": "Terra Firm",
      "healthCheckStatus": "Passed",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee",
      "lastRefreshedDateTime": "2021-07-11T18:02:16.6450704Z"
    }
  ]
}
```
