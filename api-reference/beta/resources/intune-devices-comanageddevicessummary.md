---
title: tipo de recurso comanagedDevicesSummary
description: Dados de resumo para dispositivos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f592ba7900f0761a24b02495dc337046b615bb1
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793462"
---
# <a name="comanageddevicessummary-resource-type"></a><span data-ttu-id="3d0ab-103">tipo de recurso comanagedDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="3d0ab-103">comanagedDevicesSummary resource type</span></span>

<span data-ttu-id="3d0ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d0ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d0ab-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d0ab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d0ab-107">Dados de resumo para dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="3d0ab-107">Summary data for co managed devices</span></span>

## <a name="properties"></a><span data-ttu-id="3d0ab-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d0ab-108">Properties</span></span>
|<span data-ttu-id="3d0ab-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d0ab-109">Property</span></span>|<span data-ttu-id="3d0ab-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d0ab-110">Type</span></span>|<span data-ttu-id="3d0ab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d0ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d0ab-112">inventoryCount</span><span class="sxs-lookup"><span data-stu-id="3d0ab-112">inventoryCount</span></span>|<span data-ttu-id="3d0ab-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3d0ab-113">Int32</span></span>|<span data-ttu-id="3d0ab-114">Número de dispositivos com Swung de inventário.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-114">Number of devices with Inventory swung-over.</span></span> <span data-ttu-id="3d0ab-115">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-115">This property is read-only.</span></span>|
|<span data-ttu-id="3d0ab-116">compliancePolicyCount</span><span class="sxs-lookup"><span data-stu-id="3d0ab-116">compliancePolicyCount</span></span>|<span data-ttu-id="3d0ab-117">Int32</span><span class="sxs-lookup"><span data-stu-id="3d0ab-117">Int32</span></span>|<span data-ttu-id="3d0ab-118">Número de dispositivos com o CompliancePolicy de Swung.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-118">Number of devices with CompliancePolicy swung-over.</span></span> <span data-ttu-id="3d0ab-119">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-119">This property is read-only.</span></span>|
|<span data-ttu-id="3d0ab-120">resourceAccessCount</span><span class="sxs-lookup"><span data-stu-id="3d0ab-120">resourceAccessCount</span></span>|<span data-ttu-id="3d0ab-121">Int32</span><span class="sxs-lookup"><span data-stu-id="3d0ab-121">Int32</span></span>|<span data-ttu-id="3d0ab-122">Número de dispositivos com o ResourceAccess de Swung.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-122">Number of devices with ResourceAccess swung-over.</span></span> <span data-ttu-id="3d0ab-123">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-123">This property is read-only.</span></span>|
|<span data-ttu-id="3d0ab-124">configurationSettingsCount</span><span class="sxs-lookup"><span data-stu-id="3d0ab-124">configurationSettingsCount</span></span>|<span data-ttu-id="3d0ab-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3d0ab-125">Int32</span></span>|<span data-ttu-id="3d0ab-126">Número de dispositivos com o ConfigurationSettings de Swung.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-126">Number of devices with ConfigurationSettings swung-over.</span></span> <span data-ttu-id="3d0ab-127">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-127">This property is read-only.</span></span>|
|<span data-ttu-id="3d0ab-128">windowsUpdateForBusinessCount</span><span class="sxs-lookup"><span data-stu-id="3d0ab-128">windowsUpdateForBusinessCount</span></span>|<span data-ttu-id="3d0ab-129">Int32</span><span class="sxs-lookup"><span data-stu-id="3d0ab-129">Int32</span></span>|<span data-ttu-id="3d0ab-130">Número de dispositivos com o WindowsUpdateForBusiness de Swung.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-130">Number of devices with WindowsUpdateForBusiness swung-over.</span></span> <span data-ttu-id="3d0ab-131">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-131">This property is read-only.</span></span>|
|<span data-ttu-id="3d0ab-132">endpointProtectionCount</span><span class="sxs-lookup"><span data-stu-id="3d0ab-132">endpointProtectionCount</span></span>|<span data-ttu-id="3d0ab-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3d0ab-133">Int32</span></span>|<span data-ttu-id="3d0ab-134">Número de dispositivos com o EndpointProtection de Swung.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-134">Number of devices with EndpointProtection swung-over.</span></span> <span data-ttu-id="3d0ab-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-135">This property is read-only.</span></span>|
|<span data-ttu-id="3d0ab-136">modernAppsCount</span><span class="sxs-lookup"><span data-stu-id="3d0ab-136">modernAppsCount</span></span>|<span data-ttu-id="3d0ab-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3d0ab-137">Int32</span></span>|<span data-ttu-id="3d0ab-138">Número de dispositivos com o ModernApps de Swung.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-138">Number of devices with ModernApps swung-over.</span></span> <span data-ttu-id="3d0ab-139">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-139">This property is read-only.</span></span>|
|<span data-ttu-id="3d0ab-140">officeAppsCount</span><span class="sxs-lookup"><span data-stu-id="3d0ab-140">officeAppsCount</span></span>|<span data-ttu-id="3d0ab-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3d0ab-141">Int32</span></span>|<span data-ttu-id="3d0ab-142">Número de dispositivos com o Officetreinamento de Swung.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-142">Number of devices with OfficeApps swung-over.</span></span> <span data-ttu-id="3d0ab-143">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-143">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d0ab-144">Relações</span><span class="sxs-lookup"><span data-stu-id="3d0ab-144">Relationships</span></span>
<span data-ttu-id="3d0ab-145">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3d0ab-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d0ab-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d0ab-146">JSON Representation</span></span>
<span data-ttu-id="3d0ab-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d0ab-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagedDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagedDevicesSummary",
  "inventoryCount": 1024,
  "compliancePolicyCount": 1024,
  "resourceAccessCount": 1024,
  "configurationSettingsCount": 1024,
  "windowsUpdateForBusinessCount": 1024,
  "endpointProtectionCount": 1024,
  "modernAppsCount": 1024,
  "officeAppsCount": 1024
}
```



