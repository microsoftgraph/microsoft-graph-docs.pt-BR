---
title: Listar cloudPcDeviceImages
description: Listar as propriedades e os relacionamentos das imagens do sistema operacional carregadas no computador em nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: c1e278ac26e86417432159e6a191a6bf0606813b
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873973"
---
# <a name="list-deviceimages"></a><span data-ttu-id="7748c-103">Listar deviceImages</span><span class="sxs-lookup"><span data-stu-id="7748c-103">List deviceImages</span></span>

<span data-ttu-id="7748c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7748c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7748c-105">Listar as propriedades e as relações dos objetos [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) (imagens do sistema operacional) carregados no computador em nuvem.</span><span class="sxs-lookup"><span data-stu-id="7748c-105">List the properties and relationships of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects (OS images) uploaded to cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="7748c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7748c-106">Permissions</span></span>

<span data-ttu-id="7748c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7748c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7748c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7748c-109">Permission type</span></span>|<span data-ttu-id="7748c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7748c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7748c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7748c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7748c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7748c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="7748c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7748c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7748c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7748c-114">Not supported.</span></span>|
|<span data-ttu-id="7748c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7748c-115">Application</span></span>|<span data-ttu-id="7748c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7748c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7748c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7748c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7748c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7748c-118">Optional query parameters</span></span>

<span data-ttu-id="7748c-119">Esse método dá `$select` suporte a `$filter` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7748c-119">This method supports `$select` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="7748c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7748c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7748c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7748c-121">Request headers</span></span>

| <span data-ttu-id="7748c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7748c-122">Name</span></span>          | <span data-ttu-id="7748c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7748c-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7748c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7748c-124">Authorization</span></span> | <span data-ttu-id="7748c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7748c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7748c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7748c-127">Request body</span></span>

<span data-ttu-id="7748c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7748c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7748c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7748c-129">Response</span></span>

<span data-ttu-id="7748c-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7748c-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7748c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7748c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7748c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7748c-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7748c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7748c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcdeviceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
```
# <a name="c"></a>[<span data-ttu-id="7748c-134">C#</span><span class="sxs-lookup"><span data-stu-id="7748c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcdeviceimages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7748c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7748c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcdeviceimages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7748c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7748c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcdeviceimages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7748c-137">Java</span><span class="sxs-lookup"><span data-stu-id="7748c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcdeviceimages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7748c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7748c-138">Response</span></span>

<span data-ttu-id="7748c-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7748c-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
