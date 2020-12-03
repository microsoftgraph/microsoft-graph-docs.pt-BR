---
title: tipo de recurso virtualEndpoint
description: O recurso virtualEndpoint representa um contêiner para a funcionalidade de gerenciamento de computador de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7e29e59658914e0f07af7635979e1b8938b99491
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563944"
---
# <a name="virtualendpoint-resource-type"></a><span data-ttu-id="182bb-103">tipo de recurso virtualEndpoint</span><span class="sxs-lookup"><span data-stu-id="182bb-103">virtualEndpoint resource type</span></span>

<span data-ttu-id="182bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="182bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="182bb-105">O recurso virtualEndpoint representa um contêiner para APIs para gerenciar o computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="182bb-105">The virtualEndpoint resource represents a container for APIs to manage cloud PC.</span></span>

<span data-ttu-id="182bb-106">Use a API do Cloud PC para provisionar e gerenciar áreas de trabalho virtuais para os funcionários de uma organização.</span><span class="sxs-lookup"><span data-stu-id="182bb-106">Use the cloud PC API to provision and manage virtual desktops for employees in an organization.</span></span> <span data-ttu-id="182bb-107">Use-o em conjunto com a [API do Intune](../resources/intune-graph-overview.md) para gerenciar pontos de extremidade físicos e virtuais.</span><span class="sxs-lookup"><span data-stu-id="182bb-107">Use it in conjunction with the [Intune API](../resources/intune-graph-overview.md) to manage physical and virtual endpoints.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="methods"></a><span data-ttu-id="182bb-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="182bb-108">Methods</span></span>

|<span data-ttu-id="182bb-109">Método</span><span class="sxs-lookup"><span data-stu-id="182bb-109">Method</span></span>|<span data-ttu-id="182bb-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="182bb-110">Return type</span></span>|<span data-ttu-id="182bb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="182bb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="182bb-112">Obter permissões efetivas</span><span class="sxs-lookup"><span data-stu-id="182bb-112">Get effective permissions</span></span>](../api/virtualendpoint-geteffectivepermissions.md)|<span data-ttu-id="182bb-113">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="182bb-113">String collection</span></span>|<span data-ttu-id="182bb-114">Exibir as permissões efetivas do usuário autenticado no momento.</span><span class="sxs-lookup"><span data-stu-id="182bb-114">View the effective permissions of the currently authenticated user.</span></span>|
|[<span data-ttu-id="182bb-115">Listar cloudPCs</span><span class="sxs-lookup"><span data-stu-id="182bb-115">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="182bb-116">coleção [cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="182bb-116">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="182bb-117">Listar Propriedades e relações dos objetos [cloudPC](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="182bb-117">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="182bb-118">Listar deviceImages</span><span class="sxs-lookup"><span data-stu-id="182bb-118">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="182bb-119">coleção [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="182bb-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="182bb-120">Listar as propriedades e as relações dos objetos [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="182bb-120">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="182bb-121">Criar cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="182bb-121">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="182bb-122">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="182bb-122">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="182bb-123">Criar um novo objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="182bb-123">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="182bb-124">Listar onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="182bb-124">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="182bb-125">coleção [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="182bb-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="182bb-126">Listar Propriedades e relações dos objetos [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="182bb-126">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="182bb-127">Criar cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="182bb-127">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="182bb-128">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="182bb-128">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="182bb-129">Criar um novo objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="182bb-129">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="182bb-130">Listar provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="182bb-130">List provisioningPolicies</span></span>](../api/virtualendpoint-list-provisioningpolicies.md)|<span data-ttu-id="182bb-131">coleção [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="182bb-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="182bb-132">Listar Propriedades e relações dos objetos [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="182bb-132">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>|
|[<span data-ttu-id="182bb-133">Criar cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="182bb-133">Create cloudPcProvisioningPolicy</span></span>](../api/virtualendpoint-post-provisioningpolicies.md)|[<span data-ttu-id="182bb-134">cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="182bb-134">cloudPcProvisioningPolicy</span></span>](../resources/cloudpcprovisioningpolicy.md)|<span data-ttu-id="182bb-135">Criar um novo objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="182bb-135">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="182bb-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="182bb-136">Properties</span></span>

|<span data-ttu-id="182bb-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="182bb-137">Property</span></span>|<span data-ttu-id="182bb-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="182bb-138">Type</span></span>|<span data-ttu-id="182bb-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="182bb-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="182bb-140">id</span><span class="sxs-lookup"><span data-stu-id="182bb-140">id</span></span>|<span data-ttu-id="182bb-141">String</span><span class="sxs-lookup"><span data-stu-id="182bb-141">String</span></span>|<span data-ttu-id="182bb-142">O identificador exclusivo da ID de ponto de extremidade virtual. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="182bb-142">The unique identifier for the virtual endpoint id. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="182bb-143">Relações</span><span class="sxs-lookup"><span data-stu-id="182bb-143">Relationships</span></span>

|<span data-ttu-id="182bb-144">Relação</span><span class="sxs-lookup"><span data-stu-id="182bb-144">Relationship</span></span>|<span data-ttu-id="182bb-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="182bb-145">Type</span></span>|<span data-ttu-id="182bb-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="182bb-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="182bb-147">cloudPCs</span><span class="sxs-lookup"><span data-stu-id="182bb-147">cloudPCs</span></span>|<span data-ttu-id="182bb-148">coleção [cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="182bb-148">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="182bb-149">Áreas de trabalho virtuais gerenciadas pela nuvem.</span><span class="sxs-lookup"><span data-stu-id="182bb-149">Cloud managed virtual desktops.</span></span>|
|<span data-ttu-id="182bb-150">deviceImages</span><span class="sxs-lookup"><span data-stu-id="182bb-150">deviceImages</span></span>|<span data-ttu-id="182bb-151">coleção [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="182bb-151">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="182bb-152">O recurso de imagem no PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="182bb-152">The image resource on cloud PC.</span></span>|
|<span data-ttu-id="182bb-153">onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="182bb-153">onPremisesConnections</span></span>|<span data-ttu-id="182bb-154">coleção [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="182bb-154">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="182bb-155">Uma coleção definida de informações de recursos do Azure que podem ser usadas para estabelecer conectividade de rede local para PCs em nuvem.</span><span class="sxs-lookup"><span data-stu-id="182bb-155">A defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>|
|<span data-ttu-id="182bb-156">provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="182bb-156">provisioningPolicies</span></span>|<span data-ttu-id="182bb-157">coleção [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="182bb-157">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="182bb-158">política de provisionamento do Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="182bb-158">cloud PC provisioning policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="182bb-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="182bb-159">JSON representation</span></span>

<span data-ttu-id="182bb-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="182bb-160">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.virtualEndpoint",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.virtualEndpoint",
  "id": "string"
}
```
