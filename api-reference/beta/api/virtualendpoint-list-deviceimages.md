---
title: Listar cloudPcDeviceImages
description: Listar as propriedades e as relações das imagens do sistema operacional carregadas no Cloud PC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4d392331b2cb07446374275d0ffb8e606fe7d99d
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378251"
---
# <a name="list-deviceimages"></a><span data-ttu-id="b246a-103">Listar deviceImages</span><span class="sxs-lookup"><span data-stu-id="b246a-103">List deviceImages</span></span>

<span data-ttu-id="b246a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b246a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b246a-105">Liste as propriedades e as relações dos objetos [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) (imagens de so) carregadas no Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="b246a-105">List the properties and relationships of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects (OS images) uploaded to cloud PC.</span></span>

## <a name="permissions"></a><span data-ttu-id="b246a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b246a-106">Permissions</span></span>

<span data-ttu-id="b246a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b246a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b246a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b246a-109">Permission type</span></span>|<span data-ttu-id="b246a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b246a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b246a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b246a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b246a-112">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="b246a-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="b246a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b246a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b246a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b246a-114">Not supported.</span></span>|
|<span data-ttu-id="b246a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b246a-115">Application</span></span>|<span data-ttu-id="b246a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b246a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b246a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b246a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b246a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b246a-118">Optional query parameters</span></span>

<span data-ttu-id="b246a-119">Este método oferece suporte a `$select` `$filter` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b246a-119">This method supports `$select` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="b246a-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b246a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b246a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b246a-121">Request headers</span></span>

| <span data-ttu-id="b246a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b246a-122">Name</span></span>          | <span data-ttu-id="b246a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b246a-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b246a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b246a-124">Authorization</span></span> | <span data-ttu-id="b246a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b246a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b246a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b246a-127">Request body</span></span>

<span data-ttu-id="b246a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b246a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b246a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b246a-129">Response</span></span>

<span data-ttu-id="b246a-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b246a-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b246a-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b246a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b246a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b246a-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_cloudpcdeviceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
```

### <a name="response"></a><span data-ttu-id="b246a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b246a-133">Response</span></span>

<span data-ttu-id="b246a-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b246a-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
