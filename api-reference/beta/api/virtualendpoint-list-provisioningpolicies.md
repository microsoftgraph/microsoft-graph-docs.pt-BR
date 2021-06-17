---
title: Listar cloudPcProvisioningPolicies
description: Exibir as propriedades e as relações de todas as políticas de provisionamento de computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: fb98af7ff5c97b78e0c1ba76ecc307813db36e6d
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992825"
---
# <a name="list-provisioningpolicies"></a><span data-ttu-id="13bcd-103">Listar provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="13bcd-103">List provisioningPolicies</span></span>

<span data-ttu-id="13bcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13bcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13bcd-105">Listar propriedades e relações dos objetos [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="13bcd-105">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="13bcd-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="13bcd-106">Permissions</span></span>

<span data-ttu-id="13bcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13bcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13bcd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13bcd-109">Permission type</span></span>|<span data-ttu-id="13bcd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13bcd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13bcd-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13bcd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13bcd-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13bcd-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="13bcd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13bcd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13bcd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13bcd-114">Not supported.</span></span>|
|<span data-ttu-id="13bcd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13bcd-115">Application</span></span>|<span data-ttu-id="13bcd-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13bcd-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13bcd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13bcd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13bcd-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="13bcd-118">Optional query parameters</span></span>

<span data-ttu-id="13bcd-119">Este método oferece `$select` suporte a parâmetros de consulta OData e para `$filter` ajudar a personalizar a `$expand` resposta.</span><span class="sxs-lookup"><span data-stu-id="13bcd-119">This method supports `$select`, `$filter` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="13bcd-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="13bcd-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="13bcd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13bcd-121">Request headers</span></span>

| <span data-ttu-id="13bcd-122">Nome</span><span class="sxs-lookup"><span data-stu-id="13bcd-122">Name</span></span>          | <span data-ttu-id="13bcd-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="13bcd-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="13bcd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="13bcd-124">Authorization</span></span> | <span data-ttu-id="13bcd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13bcd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13bcd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13bcd-127">Request body</span></span>

<span data-ttu-id="13bcd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13bcd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13bcd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="13bcd-129">Response</span></span>

<span data-ttu-id="13bcd-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13bcd-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13bcd-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="13bcd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="13bcd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13bcd-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="13bcd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="13bcd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcprovisioningpolicies"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
```
# <a name="c"></a>[<span data-ttu-id="13bcd-134">C#</span><span class="sxs-lookup"><span data-stu-id="13bcd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcprovisioningpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13bcd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13bcd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcprovisioningpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13bcd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13bcd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcprovisioningpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13bcd-137">Java</span><span class="sxs-lookup"><span data-stu-id="13bcd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcprovisioningpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="13bcd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="13bcd-138">Response</span></span>

<span data-ttu-id="13bcd-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="13bcd-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
