---
title: Listar cloudPcDeviceImages
description: Listar as propriedades e as relações das imagens do sistema operacional carregadas no Cloud PC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: cb1aad5278341e3fdc00ee6937970e997365aa23
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563895"
---
# <a name="list-deviceimages"></a><span data-ttu-id="3c236-103">Listar deviceImages</span><span class="sxs-lookup"><span data-stu-id="3c236-103">List deviceImages</span></span>

<span data-ttu-id="3c236-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c236-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c236-105">Liste as propriedades e as relações dos objetos [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) (imagens de so) carregadas no Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="3c236-105">List the properties and relationships of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects (OS images) uploaded to cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="3c236-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3c236-106">Permissions</span></span>

<span data-ttu-id="3c236-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c236-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c236-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c236-109">Permission type</span></span>|<span data-ttu-id="3c236-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c236-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c236-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c236-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3c236-112">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="3c236-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="3c236-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c236-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c236-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c236-114">Not supported.</span></span>|
|<span data-ttu-id="3c236-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c236-115">Application</span></span>|<span data-ttu-id="3c236-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c236-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c236-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c236-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c236-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c236-118">Optional query parameters</span></span>

<span data-ttu-id="3c236-119">Este método oferece suporte a `$select` `$filter` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3c236-119">This method supports `$select` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="3c236-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3c236-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c236-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c236-121">Request headers</span></span>

| <span data-ttu-id="3c236-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3c236-122">Name</span></span>          | <span data-ttu-id="3c236-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c236-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3c236-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c236-124">Authorization</span></span> | <span data-ttu-id="3c236-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c236-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c236-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c236-127">Request body</span></span>

<span data-ttu-id="3c236-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c236-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c236-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c236-129">Response</span></span>

<span data-ttu-id="3c236-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c236-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c236-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3c236-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c236-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c236-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3c236-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c236-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcdeviceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
```
# <a name="c"></a>[<span data-ttu-id="3c236-134">C#</span><span class="sxs-lookup"><span data-stu-id="3c236-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcdeviceimages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c236-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c236-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcdeviceimages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c236-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c236-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcdeviceimages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c236-137">Java</span><span class="sxs-lookup"><span data-stu-id="3c236-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcdeviceimages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3c236-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c236-138">Response</span></span>

<span data-ttu-id="3c236-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3c236-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcDeviceImage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
      "id": "eda7ed64-7705-4079-9d08-c2bd883fffff",
      "displayName": "Display Name value",
      "osBuildNumber": "OS Build Number value",
      "operatingSystem": "Operating System value",
      "version": "Version value",
      "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Compute/images/ExampleImage",
      "lastModifiedDateTime": "2020-11-03T07:03:44Z",
      "status": "pending",
      "statusDetails": null
    }
  ]
}
```
