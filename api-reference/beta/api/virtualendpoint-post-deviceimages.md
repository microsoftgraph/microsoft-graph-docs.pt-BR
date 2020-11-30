---
title: Criar cloudPcDeviceImage
description: Carregue uma imagem de sistema operacional personalizada que possa ser provisionada posteriormente em PCs em nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 7b2e60355bfe4db8eee014ac2290c83d146eea37
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378248"
---
# <a name="create-cloudpcdeviceimage"></a><span data-ttu-id="94337-103">Criar cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="94337-103">Create cloudPcDeviceImage</span></span>

<span data-ttu-id="94337-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94337-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94337-105">Criar um novo objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="94337-105">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span> <span data-ttu-id="94337-106">Carregue uma imagem de sistema operacional personalizada que possa ser provisionada posteriormente em PCs em nuvem.</span><span class="sxs-lookup"><span data-stu-id="94337-106">Upload a custom OS image that you can later provision on cloud PCs.</span></span>

## <a name="permissions"></a><span data-ttu-id="94337-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="94337-107">Permissions</span></span>

<span data-ttu-id="94337-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94337-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94337-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94337-110">Permission type</span></span>|<span data-ttu-id="94337-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94337-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94337-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94337-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94337-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94337-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="94337-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94337-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94337-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94337-115">Not supported.</span></span>|
|<span data-ttu-id="94337-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94337-116">Application</span></span>|<span data-ttu-id="94337-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94337-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94337-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94337-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="request-headers"></a><span data-ttu-id="94337-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94337-119">Request headers</span></span>

| <span data-ttu-id="94337-120">Nome</span><span class="sxs-lookup"><span data-stu-id="94337-120">Name</span></span>          | <span data-ttu-id="94337-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="94337-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="94337-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94337-122">Authorization</span></span> | <span data-ttu-id="94337-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94337-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="94337-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94337-125">Content-Type</span></span>  | <span data-ttu-id="94337-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94337-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94337-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94337-128">Request body</span></span>

<span data-ttu-id="94337-129">No corpo da solicitação, forneça uma representação JSON do objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="94337-129">In the request body, supply a JSON representation of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

<span data-ttu-id="94337-130">A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span><span class="sxs-lookup"><span data-stu-id="94337-130">The following table shows the properties that are required when you create the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span></span>

|<span data-ttu-id="94337-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94337-131">Property</span></span>|<span data-ttu-id="94337-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="94337-132">Type</span></span>|<span data-ttu-id="94337-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="94337-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94337-134">displayName</span><span class="sxs-lookup"><span data-stu-id="94337-134">displayName</span></span>|<span data-ttu-id="94337-135">String</span><span class="sxs-lookup"><span data-stu-id="94337-135">String</span></span>|<span data-ttu-id="94337-136">O nome de exibição da imagem.</span><span class="sxs-lookup"><span data-stu-id="94337-136">The image's display name.</span></span>|
|<span data-ttu-id="94337-137">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="94337-137">sourceImageResourceId</span></span>|<span data-ttu-id="94337-138">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="94337-138">String</span></span>|<span data-ttu-id="94337-139">A ID do recurso de imagem de origem no Azure.</span><span class="sxs-lookup"><span data-stu-id="94337-139">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="94337-140">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span><span class="sxs-lookup"><span data-stu-id="94337-140">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="94337-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="94337-141">operatingSystem</span></span>|<span data-ttu-id="94337-142">String</span><span class="sxs-lookup"><span data-stu-id="94337-142">String</span></span>|<span data-ttu-id="94337-143">O sistema operacional da imagem.</span><span class="sxs-lookup"><span data-stu-id="94337-143">The image's operating system.</span></span> <span data-ttu-id="94337-144">Por exemplo: Windows 10 Enterprise.</span><span class="sxs-lookup"><span data-stu-id="94337-144">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="94337-145">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="94337-145">osBuildNumber</span></span>|<span data-ttu-id="94337-146">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="94337-146">String</span></span>|<span data-ttu-id="94337-147">A versão de compilação do so da imagem.</span><span class="sxs-lookup"><span data-stu-id="94337-147">The image's OS build version.</span></span> <span data-ttu-id="94337-148">Por exemplo: 1909.</span><span class="sxs-lookup"><span data-stu-id="94337-148">For example: 1909.</span></span>|
|<span data-ttu-id="94337-149">versão</span><span class="sxs-lookup"><span data-stu-id="94337-149">version</span></span>|<span data-ttu-id="94337-150">String</span><span class="sxs-lookup"><span data-stu-id="94337-150">String</span></span>|<span data-ttu-id="94337-151">A versão da imagem.</span><span class="sxs-lookup"><span data-stu-id="94337-151">The image version.</span></span> <span data-ttu-id="94337-152">Por exemplo: 0.0.1, 1.5.13.</span><span class="sxs-lookup"><span data-stu-id="94337-152">For example: 0.0.1, 1.5.13.</span></span>|

## <a name="response"></a><span data-ttu-id="94337-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="94337-153">Response</span></span>

<span data-ttu-id="94337-154">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94337-154">If successful, this method returns a `201 Created` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94337-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="94337-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94337-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94337-156">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="94337-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="94337-157">Response</span></span>

<span data-ttu-id="94337-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="94337-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
