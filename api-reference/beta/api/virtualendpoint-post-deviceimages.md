---
title: Criar cloudPcDeviceImage
description: Upload uma imagem personalizada do sistema operacional que você pode provisioná-la posteriormente em PCs de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: e7da8717b9dcbf34d40de5bbcb08247d80d04514
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547089"
---
# <a name="create-cloudpcdeviceimage"></a><span data-ttu-id="8d890-103">Criar cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="8d890-103">Create cloudPcDeviceImage</span></span>

<span data-ttu-id="8d890-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d890-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d890-105">Crie um novo [objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="8d890-105">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span> <span data-ttu-id="8d890-106">Upload uma imagem personalizada do sistema operacional que você pode provisioná-la posteriormente em PCs de nuvem.</span><span class="sxs-lookup"><span data-stu-id="8d890-106">Upload a custom OS image that you can later provision on cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="8d890-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d890-107">Permissions</span></span>

<span data-ttu-id="8d890-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d890-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d890-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d890-110">Permission type</span></span>|<span data-ttu-id="8d890-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d890-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d890-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d890-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d890-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d890-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="8d890-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d890-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d890-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d890-115">Not supported.</span></span>|
|<span data-ttu-id="8d890-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d890-116">Application</span></span>|<span data-ttu-id="8d890-117">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d890-117">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d890-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d890-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="request-headers"></a><span data-ttu-id="8d890-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d890-119">Request headers</span></span>

| <span data-ttu-id="8d890-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8d890-120">Name</span></span>          | <span data-ttu-id="8d890-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d890-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="8d890-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d890-122">Authorization</span></span> | <span data-ttu-id="8d890-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d890-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8d890-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d890-125">Content-Type</span></span>  | <span data-ttu-id="8d890-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d890-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d890-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d890-128">Request body</span></span>

<span data-ttu-id="8d890-129">No corpo da solicitação, fornece uma representação JSON do [objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="8d890-129">In the request body, supply a JSON representation of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

<span data-ttu-id="8d890-130">A tabela a seguir mostra as propriedades que são necessárias ao criar [o cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span><span class="sxs-lookup"><span data-stu-id="8d890-130">The following table shows the properties that are required when you create the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span></span>

|<span data-ttu-id="8d890-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d890-131">Property</span></span>|<span data-ttu-id="8d890-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d890-132">Type</span></span>|<span data-ttu-id="8d890-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d890-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d890-134">displayName</span><span class="sxs-lookup"><span data-stu-id="8d890-134">displayName</span></span>|<span data-ttu-id="8d890-135">String</span><span class="sxs-lookup"><span data-stu-id="8d890-135">String</span></span>|<span data-ttu-id="8d890-136">O nome de exibição da imagem.</span><span class="sxs-lookup"><span data-stu-id="8d890-136">The image's display name.</span></span>|
|<span data-ttu-id="8d890-137">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="8d890-137">sourceImageResourceId</span></span>|<span data-ttu-id="8d890-138">String</span><span class="sxs-lookup"><span data-stu-id="8d890-138">String</span></span>|<span data-ttu-id="8d890-139">A ID do recurso de imagem de origem no Azure.</span><span class="sxs-lookup"><span data-stu-id="8d890-139">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="8d890-140">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span><span class="sxs-lookup"><span data-stu-id="8d890-140">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="8d890-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8d890-141">operatingSystem</span></span>|<span data-ttu-id="8d890-142">String</span><span class="sxs-lookup"><span data-stu-id="8d890-142">String</span></span>|<span data-ttu-id="8d890-143">O sistema operacional da imagem.</span><span class="sxs-lookup"><span data-stu-id="8d890-143">The image's operating system.</span></span> <span data-ttu-id="8d890-144">Por exemplo: Windows 10 Enterprise.</span><span class="sxs-lookup"><span data-stu-id="8d890-144">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="8d890-145">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="8d890-145">osBuildNumber</span></span>|<span data-ttu-id="8d890-146">String</span><span class="sxs-lookup"><span data-stu-id="8d890-146">String</span></span>|<span data-ttu-id="8d890-147">A versão de com build do sistema operacional da imagem.</span><span class="sxs-lookup"><span data-stu-id="8d890-147">The image's OS build version.</span></span> <span data-ttu-id="8d890-148">Por exemplo: 1909.</span><span class="sxs-lookup"><span data-stu-id="8d890-148">For example: 1909.</span></span>|
|<span data-ttu-id="8d890-149">versão</span><span class="sxs-lookup"><span data-stu-id="8d890-149">version</span></span>|<span data-ttu-id="8d890-150">String</span><span class="sxs-lookup"><span data-stu-id="8d890-150">String</span></span>|<span data-ttu-id="8d890-151">A versão da imagem.</span><span class="sxs-lookup"><span data-stu-id="8d890-151">The image version.</span></span> <span data-ttu-id="8d890-152">Por exemplo: 0.0.1, 1.5.13.</span><span class="sxs-lookup"><span data-stu-id="8d890-152">For example: 0.0.1, 1.5.13.</span></span>|

## <a name="response"></a><span data-ttu-id="8d890-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d890-153">Response</span></span>

<span data-ttu-id="8d890-154">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d890-154">If successful, this method returns a `201 Created` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d890-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8d890-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d890-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d890-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8d890-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d890-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8d890-158">C#</span><span class="sxs-lookup"><span data-stu-id="8d890-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcdeviceimage-from-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d890-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d890-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcdeviceimage-from-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d890-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d890-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcdeviceimage-from-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d890-161">Java</span><span class="sxs-lookup"><span data-stu-id="8d890-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcdeviceimage-from-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8d890-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d890-162">Response</span></span>

<span data-ttu-id="8d890-163">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8d890-163">**Note:** The response object shown here might be shortened for readability.</span></span>
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
