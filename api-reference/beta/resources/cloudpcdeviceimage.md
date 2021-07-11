---
title: Tipo de recurso cloudPcDeviceImage
description: Representa o recurso de imagem no computador de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 50154654835d1137db49f9f5690115c05ea7e0c1
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367000"
---
# <a name="cloudpcdeviceimage-resource-type"></a><span data-ttu-id="9f59c-103">Tipo de recurso cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="9f59c-103">cloudPcDeviceImage resource type</span></span>

<span data-ttu-id="9f59c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f59c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f59c-105">Representa o recurso de imagem em um computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="9f59c-105">Represents the image resource on a cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="9f59c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9f59c-106">Methods</span></span>

|<span data-ttu-id="9f59c-107">Método</span><span class="sxs-lookup"><span data-stu-id="9f59c-107">Method</span></span>|<span data-ttu-id="9f59c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9f59c-108">Return type</span></span>|<span data-ttu-id="9f59c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f59c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f59c-110">Listar deviceImages</span><span class="sxs-lookup"><span data-stu-id="9f59c-110">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="9f59c-111">[Coleção cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="9f59c-111">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="9f59c-112">Listar as propriedades e as relações dos [objetos cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="9f59c-112">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="9f59c-113">Obter cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="9f59c-113">Get cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-get.md)|[<span data-ttu-id="9f59c-114">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="9f59c-114">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="9f59c-115">Leia as propriedades e as relações de um [objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="9f59c-115">Read the properties and relationships of a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="9f59c-116">Criar cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="9f59c-116">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="9f59c-117">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="9f59c-117">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="9f59c-118">Crie um novo [objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="9f59c-118">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="9f59c-119">Excluir cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="9f59c-119">Delete cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-delete.md)|<span data-ttu-id="9f59c-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f59c-120">None</span></span>|<span data-ttu-id="9f59c-121">[Exclua um objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="9f59c-121">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="9f59c-122">getSourceImages</span><span class="sxs-lookup"><span data-stu-id="9f59c-122">getSourceImages</span></span>](../api/cloudpcdeviceimage-getsourceimages.md)|<span data-ttu-id="9f59c-123">[Coleção cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="9f59c-123">[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection</span></span>|<span data-ttu-id="9f59c-124">Obter [objetos cloudPcSourceDeviceImage.](../resources/cloudpcsourcedeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="9f59c-124">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="9f59c-125">Reupload cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="9f59c-125">Reupload cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-reupload.md)|<span data-ttu-id="9f59c-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f59c-126">None</span></span>|<span data-ttu-id="9f59c-127">Reupload a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object that failed to upload.</span><span class="sxs-lookup"><span data-stu-id="9f59c-127">Reupload a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object that failed to upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f59c-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f59c-128">Properties</span></span>

|<span data-ttu-id="9f59c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f59c-129">Property</span></span>|<span data-ttu-id="9f59c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f59c-130">Type</span></span>|<span data-ttu-id="9f59c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f59c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f59c-132">id</span><span class="sxs-lookup"><span data-stu-id="9f59c-132">id</span></span>|<span data-ttu-id="9f59c-133">String</span><span class="sxs-lookup"><span data-stu-id="9f59c-133">String</span></span>|<span data-ttu-id="9f59c-134">Identificador exclusivo do recurso de imagem no computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="9f59c-134">Unique identifier for the image resource on the cloud PC.</span></span> <span data-ttu-id="9f59c-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f59c-135">Read-only.</span></span>|
|<span data-ttu-id="9f59c-136">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="9f59c-136">sourceImageResourceId</span></span>|<span data-ttu-id="9f59c-137">String</span><span class="sxs-lookup"><span data-stu-id="9f59c-137">String</span></span>|<span data-ttu-id="9f59c-138">A ID do recurso de imagem de origem no Azure.</span><span class="sxs-lookup"><span data-stu-id="9f59c-138">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="9f59c-139">Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span><span class="sxs-lookup"><span data-stu-id="9f59c-139">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="9f59c-140">displayName</span><span class="sxs-lookup"><span data-stu-id="9f59c-140">displayName</span></span>|<span data-ttu-id="9f59c-141">String</span><span class="sxs-lookup"><span data-stu-id="9f59c-141">String</span></span>|<span data-ttu-id="9f59c-142">O nome de exibição da imagem.</span><span class="sxs-lookup"><span data-stu-id="9f59c-142">The image's display name.</span></span>|
|<span data-ttu-id="9f59c-143">versão</span><span class="sxs-lookup"><span data-stu-id="9f59c-143">version</span></span>|<span data-ttu-id="9f59c-144">String</span><span class="sxs-lookup"><span data-stu-id="9f59c-144">String</span></span>|<span data-ttu-id="9f59c-145">A versão da imagem.</span><span class="sxs-lookup"><span data-stu-id="9f59c-145">The image version.</span></span> <span data-ttu-id="9f59c-146">Por exemplo: 0.0.1, 1.5.13.</span><span class="sxs-lookup"><span data-stu-id="9f59c-146">For example: 0.0.1, 1.5.13.</span></span>|
|<span data-ttu-id="9f59c-147">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="9f59c-147">osBuildNumber</span></span>|<span data-ttu-id="9f59c-148">String</span><span class="sxs-lookup"><span data-stu-id="9f59c-148">String</span></span>|<span data-ttu-id="9f59c-149">A versão de com build do sistema operacional da imagem.</span><span class="sxs-lookup"><span data-stu-id="9f59c-149">The image's OS build version.</span></span> <span data-ttu-id="9f59c-150">Por exemplo: 1909.</span><span class="sxs-lookup"><span data-stu-id="9f59c-150">For example: 1909.</span></span>|
|<span data-ttu-id="9f59c-151">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="9f59c-151">operatingSystem</span></span>|<span data-ttu-id="9f59c-152">String</span><span class="sxs-lookup"><span data-stu-id="9f59c-152">String</span></span>|<span data-ttu-id="9f59c-153">O sistema operacional da imagem.</span><span class="sxs-lookup"><span data-stu-id="9f59c-153">The image's operating system.</span></span> <span data-ttu-id="9f59c-154">Por exemplo: Windows 10 Enterprise.</span><span class="sxs-lookup"><span data-stu-id="9f59c-154">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="9f59c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f59c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="9f59c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f59c-156">DateTimeOffset</span></span>|<span data-ttu-id="9f59c-157">Os dados e a hora em que a imagem foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9f59c-157">The data and time that the image was last modified.</span></span> <span data-ttu-id="9f59c-158">O tempo é mostrado no formato ISO 8601 e hora UTC (Tempo Universal Coordenado).</span><span class="sxs-lookup"><span data-stu-id="9f59c-158">The time is shown in ISO 8601 format and  Coordinated Universal Time (UTC) time.</span></span> <span data-ttu-id="9f59c-159">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 aparece como '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="9f59c-159">For example, midnight UTC on Jan 1, 2014 appears as '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="9f59c-160">status</span><span class="sxs-lookup"><span data-stu-id="9f59c-160">status</span></span>|<span data-ttu-id="9f59c-161">cloudPcDeviceImageStatus</span><span class="sxs-lookup"><span data-stu-id="9f59c-161">cloudPcDeviceImageStatus</span></span>|<span data-ttu-id="9f59c-162">O status da imagem no computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="9f59c-162">The status of the image on cloud PC.</span></span> <span data-ttu-id="9f59c-163">Os valores possíveis são: `pending`, `ready`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9f59c-163">Possible values are: `pending`, `ready`, `failed`.</span></span>|
|<span data-ttu-id="9f59c-164">statusDetails</span><span class="sxs-lookup"><span data-stu-id="9f59c-164">statusDetails</span></span>|<span data-ttu-id="9f59c-165">cloudPcDeviceImageStatusDetails</span><span class="sxs-lookup"><span data-stu-id="9f59c-165">cloudPcDeviceImageStatusDetails</span></span>|<span data-ttu-id="9f59c-166">Os detalhes do status da imagem, que indica por que o carregamento falhou, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="9f59c-166">The details of the image's status, which indicates why the upload failed, if applicable.</span></span> <span data-ttu-id="9f59c-167">Os valores possíveis são: `internalServerError`, `sourceImageNotFound`, `osVersionNotSupported`, e `sourceImageInvalid`.</span><span class="sxs-lookup"><span data-stu-id="9f59c-167">Possible values are: `internalServerError`, `sourceImageNotFound`, `osVersionNotSupported`, and `sourceImageInvalid`.</span></span>|

### <a name="cloudpcdeviceimagestatus-values"></a><span data-ttu-id="9f59c-168">valores cloudPcDeviceImageStatus</span><span class="sxs-lookup"><span data-stu-id="9f59c-168">cloudPcDeviceImageStatus values</span></span>

|<span data-ttu-id="9f59c-169">Member</span><span class="sxs-lookup"><span data-stu-id="9f59c-169">Member</span></span>|<span data-ttu-id="9f59c-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f59c-170">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9f59c-171">pendente</span><span class="sxs-lookup"><span data-stu-id="9f59c-171">pending</span></span>|<span data-ttu-id="9f59c-172">O carregamento da imagem está em andamento.</span><span class="sxs-lookup"><span data-stu-id="9f59c-172">The image upload is in progress.</span></span>|
|<span data-ttu-id="9f59c-173">ready</span><span class="sxs-lookup"><span data-stu-id="9f59c-173">ready</span></span>|<span data-ttu-id="9f59c-174">A imagem está pronta para uso em PCs de nuvem.</span><span class="sxs-lookup"><span data-stu-id="9f59c-174">The image is ready for use on cloud PCs.</span></span>|
|<span data-ttu-id="9f59c-175">failed</span><span class="sxs-lookup"><span data-stu-id="9f59c-175">failed</span></span>|<span data-ttu-id="9f59c-176">A imagem não pôde ser carregada.</span><span class="sxs-lookup"><span data-stu-id="9f59c-176">The image couldn’t be uploaded.</span></span> |

### <a name="cloudpcdeviceimagestatusdetails-values"></a><span data-ttu-id="9f59c-177">valores cloudPcDeviceImageStatusDetails</span><span class="sxs-lookup"><span data-stu-id="9f59c-177">cloudPcDeviceImageStatusDetails values</span></span>

|<span data-ttu-id="9f59c-178">Member</span><span class="sxs-lookup"><span data-stu-id="9f59c-178">Member</span></span>|<span data-ttu-id="9f59c-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f59c-179">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9f59c-180">internalServerError</span><span class="sxs-lookup"><span data-stu-id="9f59c-180">internalServerError</span></span>|<span data-ttu-id="9f59c-181">Houve um erro de servidor interno durante o processamento da imagem.</span><span class="sxs-lookup"><span data-stu-id="9f59c-181">There was an internal server error while processing the image.</span></span>|
|<span data-ttu-id="9f59c-182">sourceImageNotFound</span><span class="sxs-lookup"><span data-stu-id="9f59c-182">sourceImageNotFound</span></span>|<span data-ttu-id="9f59c-183">A imagem de origem está inacessível ou não encontrada.</span><span class="sxs-lookup"><span data-stu-id="9f59c-183">Source image is inaccessible or not found.</span></span>|
|<span data-ttu-id="9f59c-184">osVersionNotSupported</span><span class="sxs-lookup"><span data-stu-id="9f59c-184">osVersionNotSupported</span></span>| <span data-ttu-id="9f59c-185">A versão do sistema operacional não é suportada.</span><span class="sxs-lookup"><span data-stu-id="9f59c-185">OS version is not supported.</span></span>|
|<span data-ttu-id="9f59c-186">sourceImageInvalid</span><span class="sxs-lookup"><span data-stu-id="9f59c-186">sourceImageInvalid</span></span>|<span data-ttu-id="9f59c-187">A imagem de origem não é válida para provisionar uma Windows VM com ela.</span><span class="sxs-lookup"><span data-stu-id="9f59c-187">The source image is not valid for provisioning a Windows VM with it.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f59c-188">Relações</span><span class="sxs-lookup"><span data-stu-id="9f59c-188">Relationships</span></span>

<span data-ttu-id="9f59c-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f59c-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f59c-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f59c-190">JSON representation</span></span>

<span data-ttu-id="9f59c-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f59c-191">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcDeviceImage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "String (identifier)",
  "displayName": "String",
  "operatingSystem": "String",
  "osBuildNumber": "String",
  "version": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "statusDetails": "String",
  "sourceImageResourceId": "String"
}
```
