---
title: 'cloudPcDeviceImage: getSourceImages'
description: Exibir uma lista de todos os recursos de imagem gerenciados de suas assinaturas do Azure. Essas imagens de origem podem ser carregadas e usadas em PCs de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 244531c8dc1f54d7af3c901b45711431afc1992b
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378210"
---
# <a name="cloudpcdeviceimage-getsourceimages"></a><span data-ttu-id="5dff5-104">cloudPcDeviceImage: getSourceImages</span><span class="sxs-lookup"><span data-stu-id="5dff5-104">cloudPcDeviceImage: getSourceImages</span></span>

<span data-ttu-id="5dff5-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dff5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5dff5-106">Obter objetos [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="5dff5-106">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span> <span data-ttu-id="5dff5-107">Exibir uma lista de todos os recursos de imagem gerenciados de suas assinaturas do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5dff5-107">View a list of all the managed image resources from your Azure Active Directory subscriptions.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dff5-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="5dff5-108">Permissions</span></span>

<span data-ttu-id="5dff5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dff5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dff5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dff5-111">Permission type</span></span>|<span data-ttu-id="5dff5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5dff5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dff5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dff5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5dff5-114">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="5dff5-114">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="5dff5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dff5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dff5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dff5-116">Not supported.</span></span>|
|<span data-ttu-id="5dff5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dff5-117">Application</span></span>|<span data-ttu-id="5dff5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dff5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dff5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dff5-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```

## <a name="request-headers"></a><span data-ttu-id="5dff5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dff5-120">Request headers</span></span>

|<span data-ttu-id="5dff5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5dff5-121">Name</span></span>|<span data-ttu-id="5dff5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dff5-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5dff5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dff5-123">Authorization</span></span>|<span data-ttu-id="5dff5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dff5-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dff5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dff5-126">Request body</span></span>

<span data-ttu-id="5dff5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5dff5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dff5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dff5-128">Response</span></span>

<span data-ttu-id="5dff5-129">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dff5-129">If successful, this function returns a `200 OK` response code and a [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5dff5-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5dff5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5dff5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dff5-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "cloudpcdeviceimage_getsourceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```

### <a name="response"></a><span data-ttu-id="5dff5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dff5-132">Response</span></span>

<span data-ttu-id="5dff5-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5dff5-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcSourceDeviceImage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
      "id": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Compute/images/ExampleImage",
      "displayName": "Display Name value"
    }
  ]
}
```
