---
title: Listar cloudPcProvisioningPolicy
description: Exibir as propriedades e as relações de todas as políticas de provisionamento do Cloud PC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b9d62152228518aa856b48e3fc064ce77fd1801f
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378249"
---
# <a name="list-provisioningpolicies"></a><span data-ttu-id="5c41b-103">Listar provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="5c41b-103">List provisioningPolicies</span></span>

<span data-ttu-id="5c41b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c41b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5c41b-105">Listar Propriedades e relações dos objetos [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="5c41b-105">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c41b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5c41b-106">Permissions</span></span>

<span data-ttu-id="5c41b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c41b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c41b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c41b-109">Permission type</span></span>|<span data-ttu-id="5c41b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c41b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c41b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c41b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c41b-112">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="5c41b-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="5c41b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c41b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c41b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c41b-114">Not supported.</span></span>|
|<span data-ttu-id="5c41b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c41b-115">Application</span></span>|<span data-ttu-id="5c41b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c41b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c41b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c41b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c41b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5c41b-118">Optional query parameters</span></span>

<span data-ttu-id="5c41b-119">Este método oferece `$select` suporte `$filter` e `$expand` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5c41b-119">This method supports `$select`, `$filter` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="5c41b-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5c41b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c41b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c41b-121">Request headers</span></span>

| <span data-ttu-id="5c41b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5c41b-122">Name</span></span>          | <span data-ttu-id="5c41b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c41b-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5c41b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c41b-124">Authorization</span></span> | <span data-ttu-id="5c41b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c41b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c41b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c41b-127">Request body</span></span>

<span data-ttu-id="5c41b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c41b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c41b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c41b-129">Response</span></span>

<span data-ttu-id="5c41b-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c41b-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c41b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5c41b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c41b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c41b-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_cloudpcprovisioningpolicies"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
```

### <a name="response"></a><span data-ttu-id="5c41b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c41b-133">Response</span></span>

<span data-ttu-id="5c41b-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c41b-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcProvisioningPolicy)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
      "id": "1d164206-bf41-4fd2-8424-a3192d392273",
      "displayName": "Display Name value",
      "description": "Description value",
      "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
      "imageId": "Image ID value",
      "imageDisplayName": "Image Display Name value",
      "imageType":"custom"
    }
  ]
}
```
