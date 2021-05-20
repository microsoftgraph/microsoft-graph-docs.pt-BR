---
title: Listar cloudPcDeviceImages
description: Listar as propriedades e as relações das imagens do sistema operacional carregadas no computador de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 9a125cbd111a4646f6f7a07ddd4a44b6aab34053
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547019"
---
# <a name="list-deviceimages"></a><span data-ttu-id="47732-103">Listar deviceImages</span><span class="sxs-lookup"><span data-stu-id="47732-103">List deviceImages</span></span>

<span data-ttu-id="47732-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47732-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47732-105">Listar as propriedades e as relações dos objetos [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) (imagens do sistema operacional) carregados no computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="47732-105">List the properties and relationships of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects (OS images) uploaded to cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="47732-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="47732-106">Permissions</span></span>

<span data-ttu-id="47732-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47732-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47732-109">Permission type</span></span>|<span data-ttu-id="47732-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47732-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47732-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47732-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47732-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47732-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="47732-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47732-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47732-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47732-114">Not supported.</span></span>|
|<span data-ttu-id="47732-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47732-115">Application</span></span>|<span data-ttu-id="47732-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47732-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47732-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47732-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47732-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47732-118">Optional query parameters</span></span>

<span data-ttu-id="47732-119">Este método oferece `$select` suporte e `$filter` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="47732-119">This method supports `$select` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="47732-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="47732-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="47732-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47732-121">Request headers</span></span>

| <span data-ttu-id="47732-122">Nome</span><span class="sxs-lookup"><span data-stu-id="47732-122">Name</span></span>          | <span data-ttu-id="47732-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="47732-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="47732-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="47732-124">Authorization</span></span> | <span data-ttu-id="47732-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47732-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47732-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47732-127">Request body</span></span>

<span data-ttu-id="47732-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47732-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47732-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="47732-129">Response</span></span>

<span data-ttu-id="47732-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47732-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47732-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47732-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47732-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47732-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="47732-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="47732-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcdeviceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
```
# <a name="c"></a>[<span data-ttu-id="47732-134">C#</span><span class="sxs-lookup"><span data-stu-id="47732-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcdeviceimages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47732-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47732-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcdeviceimages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47732-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47732-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcdeviceimages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47732-137">Java</span><span class="sxs-lookup"><span data-stu-id="47732-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcdeviceimages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="47732-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="47732-138">Response</span></span>

<span data-ttu-id="47732-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="47732-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
