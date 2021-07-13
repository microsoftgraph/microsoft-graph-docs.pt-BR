---
title: Listar cloudPcOverviews
description: Obter uma lista dos objetos cloudPcOverview e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 5550c1bf9bccf00552d5251b7bf173a4022d1cd3
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401906"
---
# <a name="list-cloudpcoverviews"></a><span data-ttu-id="4285b-103">Listar cloudPcOverviews</span><span class="sxs-lookup"><span data-stu-id="4285b-103">List cloudPcOverviews</span></span>
<span data-ttu-id="4285b-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="4285b-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4285b-105">Obter uma lista dos objetos [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="4285b-105">Get a list of the [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="4285b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4285b-106">Permissions</span></span>
<span data-ttu-id="4285b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4285b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4285b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4285b-109">Permission type</span></span>|<span data-ttu-id="4285b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4285b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4285b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4285b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4285b-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4285b-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="4285b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4285b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4285b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4285b-114">Not supported.</span></span>|
|<span data-ttu-id="4285b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4285b-115">Application</span></span>|<span data-ttu-id="4285b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4285b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4285b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4285b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcsOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4285b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4285b-118">Optional query parameters</span></span>
<span data-ttu-id="4285b-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="4285b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4285b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4285b-120">Request headers</span></span>
|<span data-ttu-id="4285b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4285b-121">Name</span></span>|<span data-ttu-id="4285b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4285b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4285b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4285b-123">Authorization</span></span>|<span data-ttu-id="4285b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4285b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4285b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4285b-126">Request body</span></span>
<span data-ttu-id="4285b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4285b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4285b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4285b-128">Response</span></span>

<span data-ttu-id="4285b-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4285b-129">If successful, this method returns a `200 OK` response code and a collection of [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4285b-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4285b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4285b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4285b-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_cloudpcoverview"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcsOverview
```


### <a name="response"></a><span data-ttu-id="4285b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4285b-132">Response</span></span>
><span data-ttu-id="4285b-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4285b-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.cloudPcOverview)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.cloudPcOverview",
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee",
      "totalCloudPcStatus": 18,
      "numberOfCloudPcStatusNotProvisioned": 4,
      "numberOfCloudPcStatusProvisioning": 0,
      "numberOfCloudPcStatusProvisioned": 14,
      "numberOfCloudPcStatusUpgrading": 0,
      "numberOfCloudPcStatusInGracePeriod": 0,
      "numberOfCloudPcStatusDeprovisioning": 0,
      "numberOfCloudPcStatusFailed": 0,
      "numberOfCloudPcStatusUnknown": 0,
      "totalCloudPcConnectionStatus": 25,
      "numberOfCloudPcConnectionStatusPending": 0,
      "numberOfCloudPcConnectionStatusRunning": 0,
      "numberOfCloudPcConnectionStatusPassed": 17,
      "numberOfCloudPcConnectionStatusFailed": 6,
      "numberOfCloudPcConnectionStatusUnkownFutureValue": 0,
      "lastRefreshedDateTime": "2021-07-11T17:18:46.4830816Z"
    }
  ]
}
```
