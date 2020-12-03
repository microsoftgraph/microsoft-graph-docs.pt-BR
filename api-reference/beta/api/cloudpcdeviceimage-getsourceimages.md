---
title: 'cloudPcDeviceImage: getSourceImages'
description: Exibir uma lista de todos os recursos de imagem gerenciados de suas assinaturas do Azure. Essas imagens de origem podem ser carregadas e usadas em PCs de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 824a33fbe28aeca25ea5e1420559cbac71ebffc5
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563391"
---
# <a name="cloudpcdeviceimage-getsourceimages"></a><span data-ttu-id="935d2-104">cloudPcDeviceImage: getSourceImages</span><span class="sxs-lookup"><span data-stu-id="935d2-104">cloudPcDeviceImage: getSourceImages</span></span>

<span data-ttu-id="935d2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="935d2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="935d2-106">Obter objetos [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="935d2-106">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span> <span data-ttu-id="935d2-107">Exibir uma lista de todos os recursos de imagem gerenciados de suas assinaturas do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="935d2-107">View a list of all the managed image resources from your Azure Active Directory subscriptions.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="935d2-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="935d2-108">Permissions</span></span>

<span data-ttu-id="935d2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="935d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="935d2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="935d2-111">Permission type</span></span>|<span data-ttu-id="935d2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="935d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="935d2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="935d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="935d2-114">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="935d2-114">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="935d2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="935d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="935d2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="935d2-116">Not supported.</span></span>|
|<span data-ttu-id="935d2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="935d2-117">Application</span></span>|<span data-ttu-id="935d2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="935d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="935d2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="935d2-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```

## <a name="request-headers"></a><span data-ttu-id="935d2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="935d2-120">Request headers</span></span>

|<span data-ttu-id="935d2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="935d2-121">Name</span></span>|<span data-ttu-id="935d2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="935d2-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="935d2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="935d2-123">Authorization</span></span>|<span data-ttu-id="935d2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="935d2-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="935d2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="935d2-126">Request body</span></span>

<span data-ttu-id="935d2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="935d2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="935d2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="935d2-128">Response</span></span>

<span data-ttu-id="935d2-129">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="935d2-129">If successful, this function returns a `200 OK` response code and a [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="935d2-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="935d2-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="935d2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="935d2-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="935d2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="935d2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpcdeviceimage_getsourceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```
# <a name="c"></a>[<span data-ttu-id="935d2-133">C#</span><span class="sxs-lookup"><span data-stu-id="935d2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpcdeviceimage-getsourceimages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="935d2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="935d2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpcdeviceimage-getsourceimages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="935d2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="935d2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpcdeviceimage-getsourceimages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="935d2-136">Java</span><span class="sxs-lookup"><span data-stu-id="935d2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpcdeviceimage-getsourceimages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="935d2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="935d2-137">Response</span></span>

<span data-ttu-id="935d2-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="935d2-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
