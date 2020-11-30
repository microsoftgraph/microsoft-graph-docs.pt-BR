---
title: Obter cloudPcProvisioningPolicy
description: Leia as propriedades e os relacionamentos de um objeto cloudPcProvisioningPolicy.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: fa46603bddde0e12e34ad1abccf5afaa74861971
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378235"
---
# <a name="get-cloudpcprovisioningpolicy"></a><span data-ttu-id="c309b-103">Obter cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="c309b-103">Get cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="c309b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c309b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c309b-105">Leia as propriedades e os relacionamentos de um objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="c309b-105">Read the properties and relationships of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c309b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c309b-106">Permissions</span></span>

<span data-ttu-id="c309b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c309b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c309b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c309b-109">Permission type</span></span>|<span data-ttu-id="c309b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c309b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c309b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c309b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c309b-112">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="c309b-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="c309b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c309b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c309b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c309b-114">Not supported.</span></span>|
|<span data-ttu-id="c309b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c309b-115">Application</span></span>|<span data-ttu-id="c309b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c309b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c309b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c309b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c309b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c309b-118">Optional query parameters</span></span>

<span data-ttu-id="c309b-119">Este método oferece suporte a `$select` `$expand` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c309b-119">This method supports `$select` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="c309b-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c309b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c309b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c309b-121">Request headers</span></span>

| <span data-ttu-id="c309b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c309b-122">Name</span></span>          | <span data-ttu-id="c309b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c309b-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c309b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c309b-124">Authorization</span></span> | <span data-ttu-id="c309b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c309b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c309b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c309b-127">Request body</span></span>

<span data-ttu-id="c309b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c309b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c309b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c309b-129">Response</span></span>

<span data-ttu-id="c309b-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c309b-130">If successful, this method returns a `200 OK` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c309b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c309b-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-the-specified-provisioning-policy"></a><span data-ttu-id="c309b-132">Exemplo 1: obter as propriedades da política de provisionamento especificada</span><span class="sxs-lookup"><span data-stu-id="c309b-132">Example 1: Get the properties of the specified provisioning policy</span></span>

#### <a name="request"></a><span data-ttu-id="c309b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c309b-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpcprovisioningpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

#### <a name="response"></a><span data-ttu-id="c309b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c309b-134">Response</span></span>

<span data-ttu-id="c309b-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c309b-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
    "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff",
    "displayName": "Display Name value",
    "description": "Description value",
    "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
    "imageId": "Image ID value",
    "imageDisplayName": "Image Display Name value",
    "imageType": "custom"
  }
}
```

### <a name="example-2-get-the-properties-of-the-specified-provisioning-policy-and-expand-on-the-assignments"></a><span data-ttu-id="c309b-136">Exemplo 2: obter as propriedades da política de provisionamento especificada e expandir as atribuições</span><span class="sxs-lookup"><span data-stu-id="c309b-136">Example 2: Get the properties of the specified provisioning policy and expand on the assignments</span></span>

#### <a name="request"></a><span data-ttu-id="c309b-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c309b-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpcprovisioningpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}?$expand=assignments
```

#### <a name="response"></a><span data-ttu-id="c309b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c309b-138">Response</span></span>

<span data-ttu-id="c309b-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c309b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
    "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff",
    "displayName": "Display Name value",
    "description": "Description value",
    "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
    "imageId": "Image ID value",
    "imageDisplayName": "Image Display Name value",
    "imageType": "custom",
    "assignments": [
      {
        "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
        "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
        "target": {
          "@odata.type":"microsoft.graph.cloudPCManagementGroupAssignmentTarget",
          "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26bfd9"
          }
      }
    ]
  }
}
```
