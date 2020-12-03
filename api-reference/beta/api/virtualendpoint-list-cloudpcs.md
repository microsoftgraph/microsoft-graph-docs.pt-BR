---
title: Listar cloudPCs
description: Listar Propriedades e relações dos objetos cloudPC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 80fe8d0f8850acc7da90f44b7f6a96eb89c2d785
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563896"
---
# <a name="list-cloudpcs"></a><span data-ttu-id="4e5b6-103">Listar cloudPCs</span><span class="sxs-lookup"><span data-stu-id="4e5b6-103">List cloudPCs</span></span>

<span data-ttu-id="4e5b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e5b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e5b6-105">Listar Propriedades e relações dos objetos [cloudPC](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="4e5b6-105">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="4e5b6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4e5b6-106">Permissions</span></span>

<span data-ttu-id="4e5b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e5b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e5b6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e5b6-109">Permission type</span></span>|<span data-ttu-id="4e5b6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e5b6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e5b6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e5b6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4e5b6-112">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="4e5b6-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="4e5b6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e5b6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e5b6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e5b6-114">Not supported.</span></span>|
|<span data-ttu-id="4e5b6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e5b6-115">Application</span></span>|<span data-ttu-id="4e5b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e5b6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e5b6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e5b6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e5b6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4e5b6-118">Optional query parameters</span></span>

<span data-ttu-id="4e5b6-119">Este método oferece `$select` suporte `$filter` e `$count` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4e5b6-119">This method supports `$select`, `$filter` and `$count` OData query parameters to help customize the response.</span></span> <span data-ttu-id="4e5b6-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4e5b6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e5b6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e5b6-121">Request headers</span></span>

| <span data-ttu-id="4e5b6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4e5b6-122">Name</span></span>          | <span data-ttu-id="4e5b6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e5b6-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4e5b6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e5b6-124">Authorization</span></span> | <span data-ttu-id="4e5b6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e5b6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e5b6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e5b6-127">Request body</span></span>

<span data-ttu-id="4e5b6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4e5b6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e5b6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e5b6-129">Response</span></span>

<span data-ttu-id="4e5b6-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [cloudPC](../resources/cloudpc.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e5b6-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPC](../resources/cloudpc.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4e5b6-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4e5b6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4e5b6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e5b6-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4e5b6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e5b6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcs"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs
```
# <a name="c"></a>[<span data-ttu-id="4e5b6-134">C#</span><span class="sxs-lookup"><span data-stu-id="4e5b6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e5b6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e5b6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e5b6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e5b6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e5b6-137">Java</span><span class="sxs-lookup"><span data-stu-id="4e5b6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4e5b6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e5b6-138">Response</span></span>

<span data-ttu-id="4e5b6-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4e5b6-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPC)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPC",
      "id": "662009bc-7732-4f6f-8726-25883518ffff",
      "displayName": "Display Name value",
      "imageDisplayName": "Image Display Name value",
      "managedDeviceId": "bdc8e6dd-0455-4412-83d9-c818664fffff",
      "managedDeviceName": "Managed Device Name value",
      "provisioningPolicyId": "7ed725ad-0a00-4117-b557-d965c373ffff",
      "servicePlanId": "dbb9148c-ff83-4a4c-8d7f-28752e93ffff",
      "servicePlanName": "lite",
      "status": "provisioned",
      "userPrincipalName": "User Principal Name value",
      "lastModifiedDateTime": "2020-11-03T10:29:57Z",
      "statusDetails": null
    }
  ]
}
```
