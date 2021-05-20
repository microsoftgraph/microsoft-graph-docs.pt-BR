---
title: Obter cloudPcDeviceImages
description: Leia as propriedades e as relações de um objeto cloudPcDeviceImage.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 1db3504d2915723d950ab6f52706429cedbd4765
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546851"
---
# <a name="get-cloudpcdeviceimage"></a><span data-ttu-id="9bd4c-103">Obter cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="9bd4c-103">Get cloudPcDeviceImage</span></span>

<span data-ttu-id="9bd4c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bd4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bd4c-105">Leia as propriedades e as relações de um objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) específico.</span><span class="sxs-lookup"><span data-stu-id="9bd4c-105">Read the properties and relationships of a specific [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="9bd4c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9bd4c-106">Permissions</span></span>

<span data-ttu-id="9bd4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bd4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bd4c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bd4c-109">Permission type</span></span>|<span data-ttu-id="9bd4c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9bd4c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bd4c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bd4c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9bd4c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bd4c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="9bd4c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bd4c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bd4c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bd4c-114">Not supported.</span></span>|
|<span data-ttu-id="9bd4c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bd4c-115">Application</span></span>|<span data-ttu-id="9bd4c-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bd4c-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bd4c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bd4c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9bd4c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9bd4c-118">Optional query parameters</span></span>

<span data-ttu-id="9bd4c-119">Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9bd4c-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="9bd4c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9bd4c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bd4c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bd4c-121">Request headers</span></span>

| <span data-ttu-id="9bd4c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9bd4c-122">Name</span></span>          | <span data-ttu-id="9bd4c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bd4c-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9bd4c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bd4c-124">Authorization</span></span> | <span data-ttu-id="9bd4c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bd4c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9bd4c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bd4c-127">Request body</span></span>

<span data-ttu-id="9bd4c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9bd4c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bd4c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bd4c-129">Response</span></span>

<span data-ttu-id="9bd4c-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bd4c-130">If successful, this method returns a `200 OK` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9bd4c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9bd4c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9bd4c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bd4c-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9bd4c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bd4c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcdeviceimage"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{id}
```
# <a name="c"></a>[<span data-ttu-id="9bd4c-134">C#</span><span class="sxs-lookup"><span data-stu-id="9bd4c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bd4c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bd4c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bd4c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bd4c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9bd4c-137">Java</span><span class="sxs-lookup"><span data-stu-id="9bd4c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9bd4c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bd4c-138">Response</span></span>

<span data-ttu-id="9bd4c-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9bd4c-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
