---
title: Criar cloudPcDeviceImage
description: Carregue uma imagem de sistema operacional personalizada que possa ser provisionada posteriormente em PCs em nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 4cbfb96f6adf70a197b3d648d1bddb4cd405a1c9
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563461"
---
# <a name="create-cloudpcdeviceimage"></a><span data-ttu-id="8f0ba-103">Criar cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="8f0ba-103">Create cloudPcDeviceImage</span></span>

<span data-ttu-id="8f0ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f0ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f0ba-105">Criar um novo objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="8f0ba-105">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span> <span data-ttu-id="8f0ba-106">Carregue uma imagem de sistema operacional personalizada que possa ser provisionada posteriormente em PCs em nuvem.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-106">Upload a custom OS image that you can later provision on cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="8f0ba-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8f0ba-107">Permissions</span></span>

<span data-ttu-id="8f0ba-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f0ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f0ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f0ba-110">Permission type</span></span>|<span data-ttu-id="8f0ba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f0ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f0ba-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f0ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f0ba-113">CloudPC. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8f0ba-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="8f0ba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f0ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f0ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-115">Not supported.</span></span>|
|<span data-ttu-id="8f0ba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f0ba-116">Application</span></span>|<span data-ttu-id="8f0ba-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f0ba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f0ba-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="request-headers"></a><span data-ttu-id="8f0ba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f0ba-119">Request headers</span></span>

| <span data-ttu-id="8f0ba-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8f0ba-120">Name</span></span>          | <span data-ttu-id="8f0ba-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f0ba-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="8f0ba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f0ba-122">Authorization</span></span> | <span data-ttu-id="8f0ba-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8f0ba-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f0ba-125">Content-Type</span></span>  | <span data-ttu-id="8f0ba-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f0ba-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f0ba-128">Request body</span></span>

<span data-ttu-id="8f0ba-129">No corpo da solicitação, forneça uma representação JSON do objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="8f0ba-129">In the request body, supply a JSON representation of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

<span data-ttu-id="8f0ba-130">A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span><span class="sxs-lookup"><span data-stu-id="8f0ba-130">The following table shows the properties that are required when you create the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span></span>

|<span data-ttu-id="8f0ba-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f0ba-131">Property</span></span>|<span data-ttu-id="8f0ba-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f0ba-132">Type</span></span>|<span data-ttu-id="8f0ba-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f0ba-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f0ba-134">displayName</span><span class="sxs-lookup"><span data-stu-id="8f0ba-134">displayName</span></span>|<span data-ttu-id="8f0ba-135">String</span><span class="sxs-lookup"><span data-stu-id="8f0ba-135">String</span></span>|<span data-ttu-id="8f0ba-136">O nome de exibição da imagem.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-136">The image's display name.</span></span>|
|<span data-ttu-id="8f0ba-137">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="8f0ba-137">sourceImageResourceId</span></span>|<span data-ttu-id="8f0ba-138">String</span><span class="sxs-lookup"><span data-stu-id="8f0ba-138">String</span></span>|<span data-ttu-id="8f0ba-139">A ID do recurso de imagem de origem no Azure.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-139">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="8f0ba-140">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span><span class="sxs-lookup"><span data-stu-id="8f0ba-140">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="8f0ba-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8f0ba-141">operatingSystem</span></span>|<span data-ttu-id="8f0ba-142">String</span><span class="sxs-lookup"><span data-stu-id="8f0ba-142">String</span></span>|<span data-ttu-id="8f0ba-143">O sistema operacional da imagem.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-143">The image's operating system.</span></span> <span data-ttu-id="8f0ba-144">Por exemplo: Windows 10 Enterprise.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-144">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="8f0ba-145">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="8f0ba-145">osBuildNumber</span></span>|<span data-ttu-id="8f0ba-146">String</span><span class="sxs-lookup"><span data-stu-id="8f0ba-146">String</span></span>|<span data-ttu-id="8f0ba-147">A versão de compilação do so da imagem.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-147">The image's OS build version.</span></span> <span data-ttu-id="8f0ba-148">Por exemplo: 1909.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-148">For example: 1909.</span></span>|
|<span data-ttu-id="8f0ba-149">versão</span><span class="sxs-lookup"><span data-stu-id="8f0ba-149">version</span></span>|<span data-ttu-id="8f0ba-150">String</span><span class="sxs-lookup"><span data-stu-id="8f0ba-150">String</span></span>|<span data-ttu-id="8f0ba-151">A versão da imagem.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-151">The image version.</span></span> <span data-ttu-id="8f0ba-152">Por exemplo: 0.0.1, 1.5.13.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-152">For example: 0.0.1, 1.5.13.</span></span>|

## <a name="response"></a><span data-ttu-id="8f0ba-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f0ba-153">Response</span></span>

<span data-ttu-id="8f0ba-154">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-154">If successful, this method returns a `201 Created` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f0ba-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8f0ba-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f0ba-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f0ba-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8f0ba-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f0ba-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcdeviceimage_from_cloudpcdeviceimage"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
Content-Type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "displayName": "Display Name value",
  "osBuildNumber": "OS Build Number value",
  "operatingSystem": "Operating System value",
  "version": "Version value",
  "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage"
}
```
# <a name="c"></a>[<span data-ttu-id="8f0ba-158">C#</span><span class="sxs-lookup"><span data-stu-id="8f0ba-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcdeviceimage-from-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f0ba-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f0ba-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcdeviceimage-from-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f0ba-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f0ba-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcdeviceimage-from-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f0ba-161">Java</span><span class="sxs-lookup"><span data-stu-id="8f0ba-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcdeviceimage-from-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8f0ba-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f0ba-162">Response</span></span>

<span data-ttu-id="8f0ba-163">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8f0ba-163">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcDeviceImage"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 508

{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "eda7ed64-7705-4079-9d08-c2bd883fffff",
  "displayName": "Display Name value",
  "osBuildNumber": "OS Build Number value",
  "operatingSystem": "Operating System value",
  "version": "Version value",
  "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage",
  "lastModifiedDateTime": "2020-11-03T07:03:44.97Z",
  "status": "pending",
  "statusDetails": null
}
```
