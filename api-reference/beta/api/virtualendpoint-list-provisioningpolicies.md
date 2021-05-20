---
title: Listar cloudPcProvisioningPolicy
description: Exibir as propriedades e as relações de todas as políticas de provisionamento de computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: e7d1090af54f82e730b20238ddb4e26c8e5a31de
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547643"
---
# <a name="list-provisioningpolicies"></a><span data-ttu-id="173d5-103">Listar provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="173d5-103">List provisioningPolicies</span></span>

<span data-ttu-id="173d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="173d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="173d5-105">Listar propriedades e relações dos objetos [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="173d5-105">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="173d5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="173d5-106">Permissions</span></span>

<span data-ttu-id="173d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="173d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="173d5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="173d5-109">Permission type</span></span>|<span data-ttu-id="173d5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="173d5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="173d5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="173d5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="173d5-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="173d5-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="173d5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="173d5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="173d5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="173d5-114">Not supported.</span></span>|
|<span data-ttu-id="173d5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="173d5-115">Application</span></span>|<span data-ttu-id="173d5-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="173d5-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="173d5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="173d5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="173d5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="173d5-118">Optional query parameters</span></span>

<span data-ttu-id="173d5-119">Este método oferece `$select` suporte a parâmetros de consulta OData e para `$filter` ajudar a personalizar a `$expand` resposta.</span><span class="sxs-lookup"><span data-stu-id="173d5-119">This method supports `$select`, `$filter` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="173d5-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="173d5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="173d5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="173d5-121">Request headers</span></span>

| <span data-ttu-id="173d5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="173d5-122">Name</span></span>          | <span data-ttu-id="173d5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="173d5-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="173d5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="173d5-124">Authorization</span></span> | <span data-ttu-id="173d5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="173d5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="173d5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="173d5-127">Request body</span></span>

<span data-ttu-id="173d5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="173d5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="173d5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="173d5-129">Response</span></span>

<span data-ttu-id="173d5-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="173d5-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="173d5-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="173d5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="173d5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="173d5-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="173d5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="173d5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcprovisioningpolicies"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
```
# <a name="c"></a>[<span data-ttu-id="173d5-134">C#</span><span class="sxs-lookup"><span data-stu-id="173d5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcprovisioningpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="173d5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="173d5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcprovisioningpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="173d5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="173d5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcprovisioningpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="173d5-137">Java</span><span class="sxs-lookup"><span data-stu-id="173d5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcprovisioningpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="173d5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="173d5-138">Response</span></span>

<span data-ttu-id="173d5-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="173d5-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
