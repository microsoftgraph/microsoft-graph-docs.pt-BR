---
title: Obter cloudPcDeviceImages
description: Leia as propriedades e os relacionamentos de um objeto cloudPcDeviceImage.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: a6981958dea9bb2f503a676397a2917b970aa30b
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378239"
---
# <a name="get-cloudpcdeviceimage"></a><span data-ttu-id="9c622-103">Obter cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="9c622-103">Get cloudPcDeviceImage</span></span>

<span data-ttu-id="9c622-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c622-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c622-105">Leia as propriedades e os relacionamentos de um objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) específico.</span><span class="sxs-lookup"><span data-stu-id="9c622-105">Read the properties and relationships of a specific [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c622-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9c622-106">Permissions</span></span>

<span data-ttu-id="9c622-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c622-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c622-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c622-109">Permission type</span></span>|<span data-ttu-id="9c622-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9c622-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c622-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c622-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9c622-112">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="9c622-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="9c622-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c622-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c622-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c622-114">Not supported.</span></span>|
|<span data-ttu-id="9c622-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c622-115">Application</span></span>|<span data-ttu-id="9c622-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c622-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c622-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c622-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c622-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9c622-118">Optional query parameters</span></span>

<span data-ttu-id="9c622-119">Este método oferece suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9c622-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="9c622-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9c622-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c622-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c622-121">Request headers</span></span>

| <span data-ttu-id="9c622-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9c622-122">Name</span></span>          | <span data-ttu-id="9c622-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c622-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9c622-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c622-124">Authorization</span></span> | <span data-ttu-id="9c622-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c622-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c622-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c622-127">Request body</span></span>

<span data-ttu-id="9c622-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c622-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c622-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c622-129">Response</span></span>

<span data-ttu-id="9c622-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c622-130">If successful, this method returns a `200 OK` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9c622-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9c622-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9c622-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c622-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpcdeviceimage"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{id}
```

### <a name="response"></a><span data-ttu-id="9c622-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c622-133">Response</span></span>

<span data-ttu-id="9c622-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9c622-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
