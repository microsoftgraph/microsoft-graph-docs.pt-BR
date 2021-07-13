---
title: Obter cloudPcConnection
description: Leia as propriedades e as relações de um objeto cloudPcConnection.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: eab1d8d41a8c79f011de369fd9e4d2f31d5a7ed6
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401926"
---
# <a name="get-cloudpcconnection"></a><span data-ttu-id="36abc-103">Obter cloudPcConnection</span><span class="sxs-lookup"><span data-stu-id="36abc-103">Get cloudPcConnection</span></span>
<span data-ttu-id="36abc-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="36abc-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36abc-105">Leia as propriedades e as relações de um [objeto cloudPcConnection.](../resources/managedtenants-cloudpcconnection.md)</span><span class="sxs-lookup"><span data-stu-id="36abc-105">Read the properties and relationships of a [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="36abc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="36abc-106">Permissions</span></span>
<span data-ttu-id="36abc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36abc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36abc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36abc-109">Permission type</span></span>|<span data-ttu-id="36abc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36abc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36abc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36abc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36abc-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36abc-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="36abc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36abc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36abc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36abc-114">Not supported.</span></span>|
|<span data-ttu-id="36abc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36abc-115">Application</span></span>|<span data-ttu-id="36abc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36abc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36abc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36abc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcConnections/{cloudPcConnectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36abc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36abc-118">Optional query parameters</span></span>
<span data-ttu-id="36abc-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="36abc-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36abc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36abc-120">Request headers</span></span>
|<span data-ttu-id="36abc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="36abc-121">Name</span></span>|<span data-ttu-id="36abc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="36abc-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="36abc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="36abc-123">Authorization</span></span>|<span data-ttu-id="36abc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36abc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36abc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36abc-126">Request body</span></span>
<span data-ttu-id="36abc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36abc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36abc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="36abc-128">Response</span></span>

<span data-ttu-id="36abc-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36abc-129">If successful, this method returns a `200 OK` response code and a [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36abc-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="36abc-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36abc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36abc-131">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["86789ee0-e31d-4bee-98e6-6f310bd327bb"],
  "name": "get_cloudpcconnection"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcConnections/86789ee0-e31d-4bee-98e6-6f310bd327bb
```


### <a name="response"></a><span data-ttu-id="36abc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="36abc-132">Response</span></span>
><span data-ttu-id="36abc-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="36abc-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.cloudPcConnection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcConnection",
  "id": "86789ee0-e31d-4bee-98e6-6f310bd327bb",
  "lastUpdated": "2021-07-11T15:46:28.1243279Z",
  "displayName": "Az-Connection-93ac6d62-7d78-4477-bd43-db5e2013864d",
  "healthCheckStatus": "Failed",
  "tenantId": "aa060093-1e81-45b4-bebc-652713194ef7",
  "tenantDisplayName": "Lucerne Publishing",
  "lastRefreshedDateTime": "2021-07-11T15:46:28.1243279Z"
}
```
