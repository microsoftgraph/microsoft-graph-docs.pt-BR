---
title: Criar cloudPcDeviceImage
description: Carregue uma imagem do sistema operacional personalizada que você poderá provisioná-la posteriormente em PCs na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: aa0d7ba5a15acacf22cce43e4a4989dabb131118
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873945"
---
# <a name="create-cloudpcdeviceimage"></a><span data-ttu-id="1f5d8-103">Criar cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="1f5d8-103">Create cloudPcDeviceImage</span></span>

<span data-ttu-id="1f5d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f5d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f5d8-105">Crie um novo [objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="1f5d8-105">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span> <span data-ttu-id="1f5d8-106">Carregue uma imagem do sistema operacional personalizada que você poderá provisioná-la posteriormente em PCs na nuvem.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-106">Upload a custom OS image that you can later provision on cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="1f5d8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f5d8-107">Permissions</span></span>

<span data-ttu-id="1f5d8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f5d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f5d8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f5d8-110">Permission type</span></span>|<span data-ttu-id="1f5d8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f5d8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f5d8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f5d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f5d8-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f5d8-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="1f5d8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f5d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f5d8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-115">Not supported.</span></span>|
|<span data-ttu-id="1f5d8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f5d8-116">Application</span></span>|<span data-ttu-id="1f5d8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f5d8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f5d8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="request-headers"></a><span data-ttu-id="1f5d8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f5d8-119">Request headers</span></span>

| <span data-ttu-id="1f5d8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1f5d8-120">Name</span></span>          | <span data-ttu-id="1f5d8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f5d8-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="1f5d8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f5d8-122">Authorization</span></span> | <span data-ttu-id="1f5d8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1f5d8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f5d8-125">Content-Type</span></span>  | <span data-ttu-id="1f5d8-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f5d8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f5d8-128">Request body</span></span>

<span data-ttu-id="1f5d8-129">No corpo da solicitação, fornece uma representação JSON do objeto [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="1f5d8-129">In the request body, supply a JSON representation of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

<span data-ttu-id="1f5d8-130">A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span><span class="sxs-lookup"><span data-stu-id="1f5d8-130">The following table shows the properties that are required when you create the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span></span>

|<span data-ttu-id="1f5d8-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f5d8-131">Property</span></span>|<span data-ttu-id="1f5d8-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f5d8-132">Type</span></span>|<span data-ttu-id="1f5d8-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f5d8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f5d8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1f5d8-134">displayName</span></span>|<span data-ttu-id="1f5d8-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f5d8-135">String</span></span>|<span data-ttu-id="1f5d8-136">O nome de exibição da imagem.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-136">The image's display name.</span></span>|
|<span data-ttu-id="1f5d8-137">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="1f5d8-137">sourceImageResourceId</span></span>|<span data-ttu-id="1f5d8-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f5d8-138">String</span></span>|<span data-ttu-id="1f5d8-139">A ID do recurso de imagem de origem no Azure.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-139">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="1f5d8-140">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span><span class="sxs-lookup"><span data-stu-id="1f5d8-140">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="1f5d8-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="1f5d8-141">operatingSystem</span></span>|<span data-ttu-id="1f5d8-142">String</span><span class="sxs-lookup"><span data-stu-id="1f5d8-142">String</span></span>|<span data-ttu-id="1f5d8-143">O sistema operacional da imagem.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-143">The image's operating system.</span></span> <span data-ttu-id="1f5d8-144">Por exemplo: Windows 10 Enterprise.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-144">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="1f5d8-145">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="1f5d8-145">osBuildNumber</span></span>|<span data-ttu-id="1f5d8-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f5d8-146">String</span></span>|<span data-ttu-id="1f5d8-147">A versão de com build do sistema operacional da imagem.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-147">The image's OS build version.</span></span> <span data-ttu-id="1f5d8-148">Por exemplo: 1909.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-148">For example: 1909.</span></span>|
|<span data-ttu-id="1f5d8-149">versão</span><span class="sxs-lookup"><span data-stu-id="1f5d8-149">version</span></span>|<span data-ttu-id="1f5d8-150">String</span><span class="sxs-lookup"><span data-stu-id="1f5d8-150">String</span></span>|<span data-ttu-id="1f5d8-151">A versão da imagem.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-151">The image version.</span></span> <span data-ttu-id="1f5d8-152">Por exemplo: 0.0.1, 1.5.13.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-152">For example: 0.0.1, 1.5.13.</span></span>|

## <a name="response"></a><span data-ttu-id="1f5d8-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f5d8-153">Response</span></span>

<span data-ttu-id="1f5d8-154">Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-154">If successful, this method returns a `201 Created` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f5d8-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1f5d8-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f5d8-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f5d8-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1f5d8-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f5d8-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1f5d8-158">C#</span><span class="sxs-lookup"><span data-stu-id="1f5d8-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcdeviceimage-from-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f5d8-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f5d8-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcdeviceimage-from-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f5d8-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f5d8-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcdeviceimage-from-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f5d8-161">Java</span><span class="sxs-lookup"><span data-stu-id="1f5d8-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcdeviceimage-from-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f5d8-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f5d8-162">Response</span></span>

<span data-ttu-id="1f5d8-163">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1f5d8-163">**Note:** The response object shown here might be shortened for readability.</span></span>
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
