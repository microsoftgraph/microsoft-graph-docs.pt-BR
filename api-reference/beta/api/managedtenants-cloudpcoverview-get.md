---
title: Obter cloudPcOverview
description: Leia as propriedades e as relações de um objeto cloudPcOverview.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: f6874205f1a5fc37c135c152a16b0491821c2613
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401929"
---
# <a name="get-cloudpcoverview"></a><span data-ttu-id="fea6c-103">Obter cloudPcOverview</span><span class="sxs-lookup"><span data-stu-id="fea6c-103">Get cloudPcOverview</span></span>
<span data-ttu-id="fea6c-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="fea6c-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fea6c-105">Leia as propriedades e as relações de um [objeto cloudPcOverview.](../resources/managedtenants-cloudpcoverview.md)</span><span class="sxs-lookup"><span data-stu-id="fea6c-105">Read the properties and relationships of a [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fea6c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fea6c-106">Permissions</span></span>
<span data-ttu-id="fea6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fea6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fea6c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fea6c-109">Permission type</span></span>|<span data-ttu-id="fea6c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fea6c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fea6c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fea6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fea6c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fea6c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="fea6c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fea6c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fea6c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fea6c-114">Not supported.</span></span>|
|<span data-ttu-id="fea6c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fea6c-115">Application</span></span>|<span data-ttu-id="fea6c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fea6c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fea6c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fea6c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcsOverview/{cloudPcOverviewId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fea6c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fea6c-118">Optional query parameters</span></span>
<span data-ttu-id="fea6c-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="fea6c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fea6c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fea6c-120">Request headers</span></span>
|<span data-ttu-id="fea6c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fea6c-121">Name</span></span>|<span data-ttu-id="fea6c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fea6c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fea6c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fea6c-123">Authorization</span></span>|<span data-ttu-id="fea6c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fea6c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fea6c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fea6c-126">Request body</span></span>
<span data-ttu-id="fea6c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fea6c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fea6c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fea6c-128">Response</span></span>

<span data-ttu-id="fea6c-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fea6c-129">If successful, this method returns a `200 OK` response code and a [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fea6c-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fea6c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fea6c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fea6c-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_cloudpcoverview"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcsOverview/{cloudPcOverviewId}
```


### <a name="response"></a><span data-ttu-id="fea6c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fea6c-132">Response</span></span>
><span data-ttu-id="fea6c-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fea6c-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.cloudPcOverview"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
```
