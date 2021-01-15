---
title: Listar cloudPcOnPremisesConnection
description: Obter uma lista dos objetos cloudPcOnPremisesConnection e suas propriedades.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 35f5d9722a2da8cd2b25d822188eebbd399157e0
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873966"
---
# <a name="list-onpremisesconnections"></a><span data-ttu-id="831a0-103">Listar onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="831a0-103">List onPremisesConnections</span></span>

<span data-ttu-id="831a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="831a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="831a0-105">Listar propriedades e relações dos objetos [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="831a0-105">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="831a0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="831a0-106">Permissions</span></span>

<span data-ttu-id="831a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="831a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="831a0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="831a0-109">Permission type</span></span>|<span data-ttu-id="831a0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="831a0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="831a0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="831a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="831a0-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="831a0-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="831a0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="831a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="831a0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="831a0-114">Not supported.</span></span>|
|<span data-ttu-id="831a0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="831a0-115">Application</span></span>|<span data-ttu-id="831a0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="831a0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="831a0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="831a0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/onPremisesConnections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="831a0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="831a0-118">Optional query parameters</span></span>

<span data-ttu-id="831a0-119">Esse método dá `$select` suporte a `$filter` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="831a0-119">This method supports `$select` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="831a0-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="831a0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="831a0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="831a0-121">Request headers</span></span>

| <span data-ttu-id="831a0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="831a0-122">Name</span></span>          | <span data-ttu-id="831a0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="831a0-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="831a0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="831a0-124">Authorization</span></span> | <span data-ttu-id="831a0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="831a0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="831a0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="831a0-127">Request body</span></span>

<span data-ttu-id="831a0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="831a0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="831a0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="831a0-129">Response</span></span>

<span data-ttu-id="831a0-130">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="831a0-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="831a0-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="831a0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="831a0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="831a0-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="831a0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="831a0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpconpremisesconnections"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections
```
# <a name="c"></a>[<span data-ttu-id="831a0-134">C#</span><span class="sxs-lookup"><span data-stu-id="831a0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpconpremisesconnections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="831a0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="831a0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpconpremisesconnections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="831a0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="831a0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpconpremisesconnections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="831a0-137">Java</span><span class="sxs-lookup"><span data-stu-id="831a0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpconpremisesconnections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="831a0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="831a0-138">Response</span></span>

<span data-ttu-id="831a0-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="831a0-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
