---
title: tipo de recurso virtualEndpoint
description: O recurso virtualEndpoint representa um contêiner para a funcionalidade de gerenciamento de computador de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 168a6f35a3d758911913422f96ea5dc070d57a47
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378230"
---
# <a name="virtualendpoint-resource-type"></a><span data-ttu-id="9ec7c-103">tipo de recurso virtualEndpoint</span><span class="sxs-lookup"><span data-stu-id="9ec7c-103">virtualEndpoint resource type</span></span>

<span data-ttu-id="9ec7c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ec7c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ec7c-105">O recurso virtualEndpoint representa um contêiner para APIs para gerenciar o computador de nuvem.</span><span class="sxs-lookup"><span data-stu-id="9ec7c-105">The virtualEndpoint resource represents a container for APIs to manage cloud PC.</span></span>

<span data-ttu-id="9ec7c-106">Use a API do Cloud PC para provisionar e gerenciar áreas de trabalho virtuais para os funcionários de uma organização.</span><span class="sxs-lookup"><span data-stu-id="9ec7c-106">Use the cloud PC API to provision and manage virtual desktops for employees in an organization.</span></span> <span data-ttu-id="9ec7c-107">Use-o em conjunto com a [API do Intune](../resources/intune-graph-overview.md) para gerenciar pontos de extremidade físicos e virtuais.</span><span class="sxs-lookup"><span data-stu-id="9ec7c-107">Use it in conjunction with the [Intune API](../resources/intune-graph-overview.md) to manage physical and virtual endpoints.</span></span>

## <a name="methods"></a><span data-ttu-id="9ec7c-108">Methods</span><span class="sxs-lookup"><span data-stu-id="9ec7c-108">Methods</span></span>

|<span data-ttu-id="9ec7c-109">Método</span><span class="sxs-lookup"><span data-stu-id="9ec7c-109">Method</span></span>|<span data-ttu-id="9ec7c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9ec7c-110">Return type</span></span>|<span data-ttu-id="9ec7c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ec7c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ec7c-112">Obter permissões efetivas</span><span class="sxs-lookup"><span data-stu-id="9ec7c-112">Get effective permissions</span></span>](../api/virtualendpoint-geteffectivepermissions.md)|<span data-ttu-id="9ec7c-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ec7c-113">String collection</span></span>|<span data-ttu-id="9ec7c-114">Exibir as permissões efetivas do usuário autenticado no momento.</span><span class="sxs-lookup"><span data-stu-id="9ec7c-114">View the effective permissions of the currently authenticated user.</span></span>|
|[<span data-ttu-id="9ec7c-115">Listar cloudPCs</span><span class="sxs-lookup"><span data-stu-id="9ec7c-115">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="9ec7c-116">coleção [cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="9ec7c-116">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="9ec7c-117">Listar Propriedades e relações dos objetos [cloudPC](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="9ec7c-117">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="9ec7c-118">Listar deviceImages</span><span class="sxs-lookup"><span data-stu-id="9ec7c-118">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="9ec7c-119">coleção [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="9ec7c-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="9ec7c-120">Listar as propriedades e as relações dos objetos [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="9ec7c-120">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="9ec7c-121">Criar cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="9ec7c-121">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="9ec7c-122">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="9ec7c-122">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="9ec7c-123">Criar um novo objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="9ec7c-123">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="9ec7c-124">Listar onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="9ec7c-124">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="9ec7c-125">coleção [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="9ec7c-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="9ec7c-126">Listar Propriedades e relações dos objetos [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="9ec7c-126">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="9ec7c-127">Criar cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="9ec7c-127">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="9ec7c-128">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="9ec7c-128">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="9ec7c-129">Criar um novo objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="9ec7c-129">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="9ec7c-130">Listar provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="9ec7c-130">List provisioningPolicies</span></span>](../api/virtualendpoint-list-provisioningpolicies.md)|<span data-ttu-id="9ec7c-131">coleção [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ec7c-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="9ec7c-132">Listar Propriedades e relações dos objetos [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9ec7c-132">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>|
|[<span data-ttu-id="9ec7c-133">Criar cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="9ec7c-133">Create cloudPcProvisioningPolicy</span></span>](../api/virtualendpoint-post-provisioningpolicies.md)|[<span data-ttu-id="9ec7c-134">cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="9ec7c-134">cloudPcProvisioningPolicy</span></span>](../resources/cloudpcprovisioningpolicy.md)|<span data-ttu-id="9ec7c-135">Criar um novo objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9ec7c-135">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ec7c-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ec7c-136">Properties</span></span>

|<span data-ttu-id="9ec7c-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ec7c-137">Property</span></span>|<span data-ttu-id="9ec7c-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ec7c-138">Type</span></span>|<span data-ttu-id="9ec7c-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ec7c-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ec7c-140">id</span><span class="sxs-lookup"><span data-stu-id="9ec7c-140">id</span></span>|<span data-ttu-id="9ec7c-141">String</span><span class="sxs-lookup"><span data-stu-id="9ec7c-141">String</span></span>|<span data-ttu-id="9ec7c-142">O identificador exclusivo da ID de ponto de extremidade virtual. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ec7c-142">The unique identifier for the virtual endpoint id. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ec7c-143">Relações</span><span class="sxs-lookup"><span data-stu-id="9ec7c-143">Relationships</span></span>

|<span data-ttu-id="9ec7c-144">Relação</span><span class="sxs-lookup"><span data-stu-id="9ec7c-144">Relationship</span></span>|<span data-ttu-id="9ec7c-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ec7c-145">Type</span></span>|<span data-ttu-id="9ec7c-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ec7c-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ec7c-147">cloudPCs</span><span class="sxs-lookup"><span data-stu-id="9ec7c-147">cloudPCs</span></span>|<span data-ttu-id="9ec7c-148">coleção [cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="9ec7c-148">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="9ec7c-149">Áreas de trabalho virtuais gerenciadas pela nuvem.</span><span class="sxs-lookup"><span data-stu-id="9ec7c-149">Cloud managed virtual desktops.</span></span>|
|<span data-ttu-id="9ec7c-150">deviceImages</span><span class="sxs-lookup"><span data-stu-id="9ec7c-150">deviceImages</span></span>|<span data-ttu-id="9ec7c-151">coleção [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="9ec7c-151">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="9ec7c-152">O recurso de imagem no PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="9ec7c-152">The image resource on cloud PC.</span></span>|
|<span data-ttu-id="9ec7c-153">onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="9ec7c-153">onPremisesConnections</span></span>|<span data-ttu-id="9ec7c-154">coleção [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="9ec7c-154">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="9ec7c-155">Uma coleção definida de informações de recursos do Azure que podem ser usadas para estabelecer conectividade de rede local para PCs em nuvem.</span><span class="sxs-lookup"><span data-stu-id="9ec7c-155">A defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>|
|<span data-ttu-id="9ec7c-156">provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="9ec7c-156">provisioningPolicies</span></span>|<span data-ttu-id="9ec7c-157">coleção [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ec7c-157">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="9ec7c-158">política de provisionamento do Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="9ec7c-158">cloud PC provisioning policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ec7c-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ec7c-159">JSON representation</span></span>

<span data-ttu-id="9ec7c-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ec7c-160">The following is a JSON representation of the resource.</span></span>
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
