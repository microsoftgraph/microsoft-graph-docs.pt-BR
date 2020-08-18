---
title: tipo de recurso comanagedDevicesSummary
description: Dados de resumo para dispositivos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e12a946db3e568faa171fa53299e6ec3546d455
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791789"
---
# <a name="comanageddevicessummary-resource-type"></a><span data-ttu-id="76409-103">tipo de recurso comanagedDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="76409-103">comanagedDevicesSummary resource type</span></span>

<span data-ttu-id="76409-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76409-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76409-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76409-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76409-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76409-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76409-107">Dados de resumo para dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="76409-107">Summary data for co managed devices</span></span>

## <a name="properties"></a><span data-ttu-id="76409-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76409-108">Properties</span></span>
|<span data-ttu-id="76409-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76409-109">Property</span></span>|<span data-ttu-id="76409-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="76409-110">Type</span></span>|<span data-ttu-id="76409-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="76409-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76409-112">inventoryCount</span><span class="sxs-lookup"><span data-stu-id="76409-112">inventoryCount</span></span>|<span data-ttu-id="76409-113">Int32</span><span class="sxs-lookup"><span data-stu-id="76409-113">Int32</span></span>|<span data-ttu-id="76409-114">Número de dispositivos com Swung de inventário.</span><span class="sxs-lookup"><span data-stu-id="76409-114">Number of devices with Inventory swung-over.</span></span> <span data-ttu-id="76409-115">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76409-115">This property is read-only.</span></span>|
|<span data-ttu-id="76409-116">compliancePolicyCount</span><span class="sxs-lookup"><span data-stu-id="76409-116">compliancePolicyCount</span></span>|<span data-ttu-id="76409-117">Int32</span><span class="sxs-lookup"><span data-stu-id="76409-117">Int32</span></span>|<span data-ttu-id="76409-118">Número de dispositivos com o CompliancePolicy de Swung.</span><span class="sxs-lookup"><span data-stu-id="76409-118">Number of devices with CompliancePolicy swung-over.</span></span> <span data-ttu-id="76409-119">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76409-119">This property is read-only.</span></span>|
|<span data-ttu-id="76409-120">resourceAccessCount</span><span class="sxs-lookup"><span data-stu-id="76409-120">resourceAccessCount</span></span>|<span data-ttu-id="76409-121">Int32</span><span class="sxs-lookup"><span data-stu-id="76409-121">Int32</span></span>|<span data-ttu-id="76409-122">Número de dispositivos com o ResourceAccess de Swung.</span><span class="sxs-lookup"><span data-stu-id="76409-122">Number of devices with ResourceAccess swung-over.</span></span> <span data-ttu-id="76409-123">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76409-123">This property is read-only.</span></span>|
|<span data-ttu-id="76409-124">configurationSettingsCount</span><span class="sxs-lookup"><span data-stu-id="76409-124">configurationSettingsCount</span></span>|<span data-ttu-id="76409-125">Int32</span><span class="sxs-lookup"><span data-stu-id="76409-125">Int32</span></span>|<span data-ttu-id="76409-126">Número de dispositivos com o ConfigurationSettings de Swung.</span><span class="sxs-lookup"><span data-stu-id="76409-126">Number of devices with ConfigurationSettings swung-over.</span></span> <span data-ttu-id="76409-127">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76409-127">This property is read-only.</span></span>|
|<span data-ttu-id="76409-128">windowsUpdateForBusinessCount</span><span class="sxs-lookup"><span data-stu-id="76409-128">windowsUpdateForBusinessCount</span></span>|<span data-ttu-id="76409-129">Int32</span><span class="sxs-lookup"><span data-stu-id="76409-129">Int32</span></span>|<span data-ttu-id="76409-130">Número de dispositivos com o WindowsUpdateForBusiness de Swung.</span><span class="sxs-lookup"><span data-stu-id="76409-130">Number of devices with WindowsUpdateForBusiness swung-over.</span></span> <span data-ttu-id="76409-131">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76409-131">This property is read-only.</span></span>|
|<span data-ttu-id="76409-132">endpointProtectionCount</span><span class="sxs-lookup"><span data-stu-id="76409-132">endpointProtectionCount</span></span>|<span data-ttu-id="76409-133">Int32</span><span class="sxs-lookup"><span data-stu-id="76409-133">Int32</span></span>|<span data-ttu-id="76409-134">Número de dispositivos com o EndpointProtection de Swung.</span><span class="sxs-lookup"><span data-stu-id="76409-134">Number of devices with EndpointProtection swung-over.</span></span> <span data-ttu-id="76409-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76409-135">This property is read-only.</span></span>|
|<span data-ttu-id="76409-136">modernAppsCount</span><span class="sxs-lookup"><span data-stu-id="76409-136">modernAppsCount</span></span>|<span data-ttu-id="76409-137">Int32</span><span class="sxs-lookup"><span data-stu-id="76409-137">Int32</span></span>|<span data-ttu-id="76409-138">Número de dispositivos com o ModernApps de Swung.</span><span class="sxs-lookup"><span data-stu-id="76409-138">Number of devices with ModernApps swung-over.</span></span> <span data-ttu-id="76409-139">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76409-139">This property is read-only.</span></span>|
|<span data-ttu-id="76409-140">officeAppsCount</span><span class="sxs-lookup"><span data-stu-id="76409-140">officeAppsCount</span></span>|<span data-ttu-id="76409-141">Int32</span><span class="sxs-lookup"><span data-stu-id="76409-141">Int32</span></span>|<span data-ttu-id="76409-142">Número de dispositivos com o Officetreinamento de Swung.</span><span class="sxs-lookup"><span data-stu-id="76409-142">Number of devices with OfficeApps swung-over.</span></span> <span data-ttu-id="76409-143">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76409-143">This property is read-only.</span></span>|
|<span data-ttu-id="76409-144">totalComanagedCount</span><span class="sxs-lookup"><span data-stu-id="76409-144">totalComanagedCount</span></span>|<span data-ttu-id="76409-145">Int32</span><span class="sxs-lookup"><span data-stu-id="76409-145">Int32</span></span>|<span data-ttu-id="76409-146">Número de dispositivos co-gerenciados.</span><span class="sxs-lookup"><span data-stu-id="76409-146">Number of Co-Managed Devices.</span></span> <span data-ttu-id="76409-147">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76409-147">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76409-148">Relações</span><span class="sxs-lookup"><span data-stu-id="76409-148">Relationships</span></span>
<span data-ttu-id="76409-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76409-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76409-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76409-150">JSON Representation</span></span>
<span data-ttu-id="76409-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76409-151">Here is a JSON representation of the resource.</span></span>
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
  "officeAppsCount": 1024,
  "totalComanagedCount": 1024
}
```



