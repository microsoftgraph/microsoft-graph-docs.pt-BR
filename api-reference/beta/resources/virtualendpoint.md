---
title: Tipo de recurso virtualEndpoint
description: O recurso virtualEndpoint representa um contêiner para a funcionalidade de gerenciamento de computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ea76f9267bc9be33c88a4d6a615f2fe881a3b193
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156676"
---
# <a name="virtualendpoint-resource-type"></a><span data-ttu-id="de2f1-103">Tipo de recurso virtualEndpoint</span><span class="sxs-lookup"><span data-stu-id="de2f1-103">virtualEndpoint resource type</span></span>

<span data-ttu-id="de2f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de2f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de2f1-105">O recurso virtualEndpoint representa um contêiner para APIs gerenciarem o computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="de2f1-105">The virtualEndpoint resource represents a container for APIs to manage cloud PC.</span></span>

<span data-ttu-id="de2f1-106">Use a API do computador na nuvem para provisionar e gerenciar áreas de trabalho virtuais para funcionários em uma organização.</span><span class="sxs-lookup"><span data-stu-id="de2f1-106">Use the cloud PC API to provision and manage virtual desktops for employees in an organization.</span></span> <span data-ttu-id="de2f1-107">Use-o em conjunto com a [API do Intune](../resources/intune-graph-overview.md) para gerenciar pontos de extremidade físicos e virtuais.</span><span class="sxs-lookup"><span data-stu-id="de2f1-107">Use it in conjunction with the [Intune API](../resources/intune-graph-overview.md) to manage physical and virtual endpoints.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="methods"></a><span data-ttu-id="de2f1-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="de2f1-108">Methods</span></span>

|<span data-ttu-id="de2f1-109">Método</span><span class="sxs-lookup"><span data-stu-id="de2f1-109">Method</span></span>|<span data-ttu-id="de2f1-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="de2f1-110">Return type</span></span>|<span data-ttu-id="de2f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="de2f1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="de2f1-112">Obter permissões efetivas</span><span class="sxs-lookup"><span data-stu-id="de2f1-112">Get effective permissions</span></span>](../api/virtualendpoint-geteffectivepermissions.md)|<span data-ttu-id="de2f1-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="de2f1-113">String collection</span></span>|<span data-ttu-id="de2f1-114">Exibir as permissões efetivas do usuário autenticado no momento.</span><span class="sxs-lookup"><span data-stu-id="de2f1-114">View the effective permissions of the currently authenticated user.</span></span>|
|[<span data-ttu-id="de2f1-115">Listar cloudPCs</span><span class="sxs-lookup"><span data-stu-id="de2f1-115">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="de2f1-116">[Coleção cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-116">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="de2f1-117">Listar propriedades e relações dos objetos [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-117">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="de2f1-118">Listar deviceImages</span><span class="sxs-lookup"><span data-stu-id="de2f1-118">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="de2f1-119">[Coleção cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="de2f1-120">Listar as propriedades e os relacionamentos dos [objetos cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-120">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="de2f1-121">Criar cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="de2f1-121">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="de2f1-122">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="de2f1-122">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="de2f1-123">Crie um novo [objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-123">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="de2f1-124">Listar onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="de2f1-124">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="de2f1-125">[Coleção cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="de2f1-126">Listar propriedades e relações dos objetos [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-126">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="de2f1-127">Criar cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="de2f1-127">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="de2f1-128">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="de2f1-128">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="de2f1-129">Crie um novo [objeto cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-129">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="de2f1-130">Listar provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="de2f1-130">List provisioningPolicies</span></span>](../api/virtualendpoint-list-provisioningpolicies.md)|<span data-ttu-id="de2f1-131">[Coleção cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="de2f1-132">Listar propriedades e relações dos objetos [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-132">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>|
|[<span data-ttu-id="de2f1-133">Criar cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="de2f1-133">Create cloudPcProvisioningPolicy</span></span>](../api/virtualendpoint-post-provisioningpolicies.md)|[<span data-ttu-id="de2f1-134">cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="de2f1-134">cloudPcProvisioningPolicy</span></span>](../resources/cloudpcprovisioningpolicy.md)|<span data-ttu-id="de2f1-135">Criar um novo [objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-135">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="de2f1-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de2f1-136">Properties</span></span>

|<span data-ttu-id="de2f1-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de2f1-137">Property</span></span>|<span data-ttu-id="de2f1-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="de2f1-138">Type</span></span>|<span data-ttu-id="de2f1-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="de2f1-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de2f1-140">id</span><span class="sxs-lookup"><span data-stu-id="de2f1-140">id</span></span>|<span data-ttu-id="de2f1-141">String</span><span class="sxs-lookup"><span data-stu-id="de2f1-141">String</span></span>|<span data-ttu-id="de2f1-142">O identificador exclusivo da ID do ponto de extremidade virtual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de2f1-142">The unique identifier for the virtual endpoint id. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de2f1-143">Relações</span><span class="sxs-lookup"><span data-stu-id="de2f1-143">Relationships</span></span>

|<span data-ttu-id="de2f1-144">Relação</span><span class="sxs-lookup"><span data-stu-id="de2f1-144">Relationship</span></span>|<span data-ttu-id="de2f1-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="de2f1-145">Type</span></span>|<span data-ttu-id="de2f1-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="de2f1-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de2f1-147">cloudPCs</span><span class="sxs-lookup"><span data-stu-id="de2f1-147">cloudPCs</span></span>|<span data-ttu-id="de2f1-148">[Coleção cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-148">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="de2f1-149">Áreas de trabalho virtuais gerenciadas na nuvem.</span><span class="sxs-lookup"><span data-stu-id="de2f1-149">Cloud managed virtual desktops.</span></span>|
|<span data-ttu-id="de2f1-150">deviceImages</span><span class="sxs-lookup"><span data-stu-id="de2f1-150">deviceImages</span></span>|<span data-ttu-id="de2f1-151">[Coleção cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-151">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="de2f1-152">O recurso de imagem no computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="de2f1-152">The image resource on cloud PC.</span></span>|
|<span data-ttu-id="de2f1-153">onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="de2f1-153">onPremisesConnections</span></span>|<span data-ttu-id="de2f1-154">[Coleção cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-154">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="de2f1-155">Uma coleção definida de informações de recursos do Azure que pode ser usada para estabelecer conectividade de rede local para PCs na nuvem.</span><span class="sxs-lookup"><span data-stu-id="de2f1-155">A defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>|
|<span data-ttu-id="de2f1-156">provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="de2f1-156">provisioningPolicies</span></span>|<span data-ttu-id="de2f1-157">[Coleção cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="de2f1-157">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="de2f1-158">política de provisionamento de computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="de2f1-158">cloud PC provisioning policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de2f1-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de2f1-159">JSON representation</span></span>

<span data-ttu-id="de2f1-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de2f1-160">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.virtualEndpoint",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.virtualEndpoint",
  "id": "string"
}
```
