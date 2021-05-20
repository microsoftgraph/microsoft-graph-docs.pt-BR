---
title: Obter cloudPcProvisioningPolicy
description: Leia as propriedades e as relações de um objeto cloudPcProvisioningPolicy.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 7a5f0c1bab5b0bd05667d6d4e75fc5ff19ef03c4
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546697"
---
# <a name="get-cloudpcprovisioningpolicy"></a><span data-ttu-id="fb671-103">Obter cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="fb671-103">Get cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="fb671-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb671-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb671-105">Leia as propriedades e as relações de um [objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fb671-105">Read the properties and relationships of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="fb671-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb671-106">Permissions</span></span>

<span data-ttu-id="fb671-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb671-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb671-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb671-109">Permission type</span></span>|<span data-ttu-id="fb671-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb671-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb671-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb671-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb671-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb671-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="fb671-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb671-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb671-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb671-114">Not supported.</span></span>|
|<span data-ttu-id="fb671-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb671-115">Application</span></span>|<span data-ttu-id="fb671-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb671-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb671-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb671-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb671-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fb671-118">Optional query parameters</span></span>

<span data-ttu-id="fb671-119">Este método oferece `$select` suporte e `$expand` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fb671-119">This method supports `$select` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="fb671-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fb671-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb671-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb671-121">Request headers</span></span>

| <span data-ttu-id="fb671-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fb671-122">Name</span></span>          | <span data-ttu-id="fb671-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb671-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fb671-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb671-124">Authorization</span></span> | <span data-ttu-id="fb671-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb671-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb671-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb671-127">Request body</span></span>

<span data-ttu-id="fb671-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb671-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb671-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb671-129">Response</span></span>

<span data-ttu-id="fb671-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb671-130">If successful, this method returns a `200 OK` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb671-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fb671-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-the-specified-provisioning-policy"></a><span data-ttu-id="fb671-132">Exemplo 1: Obter as propriedades da política de provisionamento especificada</span><span class="sxs-lookup"><span data-stu-id="fb671-132">Example 1: Get the properties of the specified provisioning policy</span></span>

#### <a name="request"></a><span data-ttu-id="fb671-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb671-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fb671-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb671-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcprovisioningpolicy_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="fb671-135">C#</span><span class="sxs-lookup"><span data-stu-id="fb671-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcprovisioningpolicy-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb671-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb671-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcprovisioningpolicy-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb671-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb671-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcprovisioningpolicy-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb671-138">Java</span><span class="sxs-lookup"><span data-stu-id="fb671-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcprovisioningpolicy-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fb671-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb671-139">Response</span></span>

<span data-ttu-id="fb671-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fb671-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-the-properties-of-the-specified-provisioning-policy-and-expand-on-the-assignments"></a><span data-ttu-id="fb671-141">Exemplo 2: Obter as propriedades da política de provisionamento especificada e expandir nas atribuições</span><span class="sxs-lookup"><span data-stu-id="fb671-141">Example 2: Get the properties of the specified provisioning policy and expand on the assignments</span></span>

#### <a name="request"></a><span data-ttu-id="fb671-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb671-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fb671-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb671-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcprovisioningpolicy_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}?$expand=assignments
```
# <a name="c"></a>[<span data-ttu-id="fb671-144">C#</span><span class="sxs-lookup"><span data-stu-id="fb671-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcprovisioningpolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb671-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb671-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcprovisioningpolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb671-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb671-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcprovisioningpolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb671-147">Java</span><span class="sxs-lookup"><span data-stu-id="fb671-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcprovisioningpolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fb671-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb671-148">Response</span></span>

<span data-ttu-id="fb671-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fb671-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
