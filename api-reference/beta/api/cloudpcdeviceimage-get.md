---
title: Obter cloudPcDeviceImages
description: Leia as propriedades e os relacionamentos de um objeto cloudPcDeviceImage.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: bb78a1eb6b6015ab7b32eb68fdaf4edc68f387e4
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563321"
---
# <a name="get-cloudpcdeviceimage"></a><span data-ttu-id="e9e5f-103">Obter cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="e9e5f-103">Get cloudPcDeviceImage</span></span>

<span data-ttu-id="e9e5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9e5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9e5f-105">Leia as propriedades e os relacionamentos de um objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) específico.</span><span class="sxs-lookup"><span data-stu-id="e9e5f-105">Read the properties and relationships of a specific [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="e9e5f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e9e5f-106">Permissions</span></span>

<span data-ttu-id="e9e5f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9e5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9e5f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9e5f-109">Permission type</span></span>|<span data-ttu-id="e9e5f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9e5f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9e5f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9e5f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e9e5f-112">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="e9e5f-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="e9e5f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9e5f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9e5f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9e5f-114">Not supported.</span></span>|
|<span data-ttu-id="e9e5f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9e5f-115">Application</span></span>|<span data-ttu-id="e9e5f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9e5f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9e5f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9e5f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9e5f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9e5f-118">Optional query parameters</span></span>

<span data-ttu-id="e9e5f-119">Este método oferece suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9e5f-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="e9e5f-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e9e5f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9e5f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9e5f-121">Request headers</span></span>

| <span data-ttu-id="e9e5f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e9e5f-122">Name</span></span>          | <span data-ttu-id="e9e5f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9e5f-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e9e5f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9e5f-124">Authorization</span></span> | <span data-ttu-id="e9e5f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9e5f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9e5f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9e5f-127">Request body</span></span>

<span data-ttu-id="e9e5f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9e5f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9e5f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9e5f-129">Response</span></span>

<span data-ttu-id="e9e5f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9e5f-130">If successful, this method returns a `200 OK` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9e5f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e9e5f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9e5f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9e5f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e9e5f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9e5f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcdeviceimage"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{id}
```
# <a name="c"></a>[<span data-ttu-id="e9e5f-134">C#</span><span class="sxs-lookup"><span data-stu-id="e9e5f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9e5f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9e5f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9e5f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9e5f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9e5f-137">Java</span><span class="sxs-lookup"><span data-stu-id="e9e5f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9e5f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9e5f-138">Response</span></span>

<span data-ttu-id="e9e5f-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e9e5f-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcDeviceImage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
    "id": "eda7ed64-7705-4079-9d08-c2bd883f4fff",
    "displayName": "Display Name value",
    "osBuildNumber": "OS Build Number value",
    "operatingSystem": "Operating System value",
    "version": "Version value",
    "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage",
    "lastModifiedDateTime": "2020-11-03T07:03:44.97Z",
    "status": "pending",
    "statusDetails": null
  }
}
```
