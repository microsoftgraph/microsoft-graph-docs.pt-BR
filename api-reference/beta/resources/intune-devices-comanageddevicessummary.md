---
title: tipo de recurso comanagedDevicesSummary
description: Dados de resumo para dispositivos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b25820e4356fadaa4f991c103500a8ef8f5c0122
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214845"
---
# <a name="comanageddevicessummary-resource-type"></a><span data-ttu-id="756c6-103">tipo de recurso comanagedDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="756c6-103">comanagedDevicesSummary resource type</span></span>

<span data-ttu-id="756c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="756c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="756c6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="756c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="756c6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="756c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="756c6-107">Dados de resumo para dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="756c6-107">Summary data for co managed devices</span></span>

## <a name="properties"></a><span data-ttu-id="756c6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="756c6-108">Properties</span></span>
|<span data-ttu-id="756c6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="756c6-109">Property</span></span>|<span data-ttu-id="756c6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="756c6-110">Type</span></span>|<span data-ttu-id="756c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="756c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="756c6-112">inventoryCount</span><span class="sxs-lookup"><span data-stu-id="756c6-112">inventoryCount</span></span>|<span data-ttu-id="756c6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="756c6-113">Int32</span></span>|<span data-ttu-id="756c6-114">Número de dispositivos com Swung de inventário.</span><span class="sxs-lookup"><span data-stu-id="756c6-114">Number of devices with Inventory swung-over.</span></span> <span data-ttu-id="756c6-115">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="756c6-115">This property is read-only.</span></span>|
|<span data-ttu-id="756c6-116">compliancePolicyCount</span><span class="sxs-lookup"><span data-stu-id="756c6-116">compliancePolicyCount</span></span>|<span data-ttu-id="756c6-117">Int32</span><span class="sxs-lookup"><span data-stu-id="756c6-117">Int32</span></span>|<span data-ttu-id="756c6-118">Número de dispositivos com o CompliancePolicy de Swung.</span><span class="sxs-lookup"><span data-stu-id="756c6-118">Number of devices with CompliancePolicy swung-over.</span></span> <span data-ttu-id="756c6-119">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="756c6-119">This property is read-only.</span></span>|
|<span data-ttu-id="756c6-120">resourceAccessCount</span><span class="sxs-lookup"><span data-stu-id="756c6-120">resourceAccessCount</span></span>|<span data-ttu-id="756c6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="756c6-121">Int32</span></span>|<span data-ttu-id="756c6-122">Número de dispositivos com o ResourceAccess de Swung.</span><span class="sxs-lookup"><span data-stu-id="756c6-122">Number of devices with ResourceAccess swung-over.</span></span> <span data-ttu-id="756c6-123">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="756c6-123">This property is read-only.</span></span>|
|<span data-ttu-id="756c6-124">configurationSettingsCount</span><span class="sxs-lookup"><span data-stu-id="756c6-124">configurationSettingsCount</span></span>|<span data-ttu-id="756c6-125">Int32</span><span class="sxs-lookup"><span data-stu-id="756c6-125">Int32</span></span>|<span data-ttu-id="756c6-126">Número de dispositivos com o ConfigurationSettings de Swung.</span><span class="sxs-lookup"><span data-stu-id="756c6-126">Number of devices with ConfigurationSettings swung-over.</span></span> <span data-ttu-id="756c6-127">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="756c6-127">This property is read-only.</span></span>|
|<span data-ttu-id="756c6-128">windowsUpdateForBusinessCount</span><span class="sxs-lookup"><span data-stu-id="756c6-128">windowsUpdateForBusinessCount</span></span>|<span data-ttu-id="756c6-129">Int32</span><span class="sxs-lookup"><span data-stu-id="756c6-129">Int32</span></span>|<span data-ttu-id="756c6-130">Número de dispositivos com o WindowsUpdateForBusiness de Swung.</span><span class="sxs-lookup"><span data-stu-id="756c6-130">Number of devices with WindowsUpdateForBusiness swung-over.</span></span> <span data-ttu-id="756c6-131">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="756c6-131">This property is read-only.</span></span>|
|<span data-ttu-id="756c6-132">endpointProtectionCount</span><span class="sxs-lookup"><span data-stu-id="756c6-132">endpointProtectionCount</span></span>|<span data-ttu-id="756c6-133">Int32</span><span class="sxs-lookup"><span data-stu-id="756c6-133">Int32</span></span>|<span data-ttu-id="756c6-134">Número de dispositivos com o EndpointProtection de Swung.</span><span class="sxs-lookup"><span data-stu-id="756c6-134">Number of devices with EndpointProtection swung-over.</span></span> <span data-ttu-id="756c6-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="756c6-135">This property is read-only.</span></span>|
|<span data-ttu-id="756c6-136">modernAppsCount</span><span class="sxs-lookup"><span data-stu-id="756c6-136">modernAppsCount</span></span>|<span data-ttu-id="756c6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="756c6-137">Int32</span></span>|<span data-ttu-id="756c6-138">Número de dispositivos com o ModernApps de Swung.</span><span class="sxs-lookup"><span data-stu-id="756c6-138">Number of devices with ModernApps swung-over.</span></span> <span data-ttu-id="756c6-139">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="756c6-139">This property is read-only.</span></span>|
|<span data-ttu-id="756c6-140">officeAppsCount</span><span class="sxs-lookup"><span data-stu-id="756c6-140">officeAppsCount</span></span>|<span data-ttu-id="756c6-141">Int32</span><span class="sxs-lookup"><span data-stu-id="756c6-141">Int32</span></span>|<span data-ttu-id="756c6-142">Número de dispositivos com o Officetreinamento de Swung.</span><span class="sxs-lookup"><span data-stu-id="756c6-142">Number of devices with OfficeApps swung-over.</span></span> <span data-ttu-id="756c6-143">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="756c6-143">This property is read-only.</span></span>|
|<span data-ttu-id="756c6-144">totalComanagedCount</span><span class="sxs-lookup"><span data-stu-id="756c6-144">totalComanagedCount</span></span>|<span data-ttu-id="756c6-145">Int32</span><span class="sxs-lookup"><span data-stu-id="756c6-145">Int32</span></span>|<span data-ttu-id="756c6-146">Número de dispositivos de Co-Managed.</span><span class="sxs-lookup"><span data-stu-id="756c6-146">Number of Co-Managed Devices.</span></span> <span data-ttu-id="756c6-147">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="756c6-147">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="756c6-148">Relações</span><span class="sxs-lookup"><span data-stu-id="756c6-148">Relationships</span></span>
<span data-ttu-id="756c6-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="756c6-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="756c6-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="756c6-150">JSON Representation</span></span>
<span data-ttu-id="756c6-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="756c6-151">Here is a JSON representation of the resource.</span></span>
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




