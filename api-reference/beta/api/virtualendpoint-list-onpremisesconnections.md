---
title: Listar cloudPcOnPremisesConnection
description: Obtenha uma lista dos objetos cloudPcOnPremisesConnection e suas propriedades.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 0227dd6225d177c3e11de37be399a01814b63bd1
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378250"
---
# <a name="list-onpremisesconnections"></a><span data-ttu-id="7ae9f-103">Listar onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="7ae9f-103">List onPremisesConnections</span></span>

<span data-ttu-id="7ae9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ae9f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ae9f-105">Listar Propriedades e relações dos objetos [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="7ae9f-105">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ae9f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7ae9f-106">Permissions</span></span>

<span data-ttu-id="7ae9f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ae9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ae9f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ae9f-109">Permission type</span></span>|<span data-ttu-id="7ae9f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ae9f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ae9f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ae9f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7ae9f-112">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="7ae9f-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="7ae9f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ae9f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ae9f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ae9f-114">Not supported.</span></span>|
|<span data-ttu-id="7ae9f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ae9f-115">Application</span></span>|<span data-ttu-id="7ae9f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ae9f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ae9f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ae9f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/onPremisesConnections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ae9f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7ae9f-118">Optional query parameters</span></span>

<span data-ttu-id="7ae9f-119">Este método oferece suporte a `$select` `$filter` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7ae9f-119">This method supports `$select` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="7ae9f-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7ae9f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ae9f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ae9f-121">Request headers</span></span>

| <span data-ttu-id="7ae9f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7ae9f-122">Name</span></span>          | <span data-ttu-id="7ae9f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ae9f-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7ae9f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ae9f-124">Authorization</span></span> | <span data-ttu-id="7ae9f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ae9f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ae9f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ae9f-127">Request body</span></span>

<span data-ttu-id="7ae9f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ae9f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ae9f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ae9f-129">Response</span></span>

<span data-ttu-id="7ae9f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ae9f-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7ae9f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7ae9f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7ae9f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ae9f-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_cloudpconpremisesconnections"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections
```

### <a name="response"></a><span data-ttu-id="7ae9f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ae9f-133">Response</span></span>

<span data-ttu-id="7ae9f-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7ae9f-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcOnPremisesConnection)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
      "id": "07f12770-a225-4957-9127-0d247cf4ffff",
      "displayName": "Display Name value",
      "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
      "subscriptionName": "Subscription Name value",
      "adDomainName": "Active Directory Domain Name value",
      "adDomainUsername": "Active Directory Domain User Name value",
      "organizationalUnit": "Organization Unit value",
      "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
      "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
      "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
      "healthCheckStatus": "passed",
      "inUse": false
    }
  ]
}
```
