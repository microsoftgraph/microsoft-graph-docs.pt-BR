---
title: Listar cloudPCs
description: Listar propriedades e relações dos objetos cloudPC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: dd8c0aaa6b9551f041a5d90f6f3ddc777b5d1b87
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547659"
---
# <a name="list-cloudpcs"></a><span data-ttu-id="a77ec-103">Listar cloudPCs</span><span class="sxs-lookup"><span data-stu-id="a77ec-103">List cloudPCs</span></span>

<span data-ttu-id="a77ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a77ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a77ec-105">Listar propriedades e relações dos objetos [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="a77ec-105">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="a77ec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a77ec-106">Permissions</span></span>

<span data-ttu-id="a77ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a77ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a77ec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a77ec-109">Permission type</span></span>|<span data-ttu-id="a77ec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a77ec-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a77ec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a77ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a77ec-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a77ec-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="a77ec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a77ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a77ec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a77ec-114">Not supported.</span></span>|
|<span data-ttu-id="a77ec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a77ec-115">Application</span></span>|<span data-ttu-id="a77ec-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a77ec-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a77ec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a77ec-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a77ec-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a77ec-118">Optional query parameters</span></span>

<span data-ttu-id="a77ec-119">Este método oferece `$select` suporte a parâmetros de consulta OData e para `$filter` ajudar a personalizar a `$count` resposta.</span><span class="sxs-lookup"><span data-stu-id="a77ec-119">This method supports `$select`, `$filter` and `$count` OData query parameters to help customize the response.</span></span> <span data-ttu-id="a77ec-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a77ec-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a77ec-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a77ec-121">Request headers</span></span>

| <span data-ttu-id="a77ec-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a77ec-122">Name</span></span>          | <span data-ttu-id="a77ec-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a77ec-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a77ec-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a77ec-124">Authorization</span></span> | <span data-ttu-id="a77ec-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a77ec-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a77ec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a77ec-127">Request body</span></span>

<span data-ttu-id="a77ec-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a77ec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a77ec-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a77ec-129">Response</span></span>

<span data-ttu-id="a77ec-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [cloudPC](../resources/cloudpc.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a77ec-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPC](../resources/cloudpc.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a77ec-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a77ec-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a77ec-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a77ec-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a77ec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a77ec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcs"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs
```
# <a name="c"></a>[<span data-ttu-id="a77ec-134">C#</span><span class="sxs-lookup"><span data-stu-id="a77ec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a77ec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a77ec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a77ec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a77ec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a77ec-137">Java</span><span class="sxs-lookup"><span data-stu-id="a77ec-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a77ec-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a77ec-138">Response</span></span>

<span data-ttu-id="a77ec-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a77ec-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
