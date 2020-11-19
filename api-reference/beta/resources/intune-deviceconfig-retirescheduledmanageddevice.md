---
title: tipo de recurso retireScheduledManagedDevice
description: ManagedDevices que estão agendados para desativação
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c15eb75f5298094ef4ac86690c446625ce1d1419
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293889"
---
# <a name="retirescheduledmanageddevice-resource-type"></a><span data-ttu-id="90cfe-103">tipo de recurso retireScheduledManagedDevice</span><span class="sxs-lookup"><span data-stu-id="90cfe-103">retireScheduledManagedDevice resource type</span></span>

<span data-ttu-id="90cfe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90cfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90cfe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90cfe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90cfe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90cfe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90cfe-107">ManagedDevices que estão agendados para desativação</span><span class="sxs-lookup"><span data-stu-id="90cfe-107">ManagedDevices that are scheduled for retire</span></span>

## <a name="properties"></a><span data-ttu-id="90cfe-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90cfe-108">Properties</span></span>
|<span data-ttu-id="90cfe-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90cfe-109">Property</span></span>|<span data-ttu-id="90cfe-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="90cfe-110">Type</span></span>|<span data-ttu-id="90cfe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="90cfe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90cfe-112">id</span><span class="sxs-lookup"><span data-stu-id="90cfe-112">id</span></span>|<span data-ttu-id="90cfe-113">String</span><span class="sxs-lookup"><span data-stu-id="90cfe-113">String</span></span>|<span data-ttu-id="90cfe-114">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="90cfe-114">Key of the entity.</span></span>|
|<span data-ttu-id="90cfe-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="90cfe-115">managedDeviceId</span></span>|<span data-ttu-id="90cfe-116">String</span><span class="sxs-lookup"><span data-stu-id="90cfe-116">String</span></span>|<span data-ttu-id="90cfe-117">DeviceID gerenciado</span><span class="sxs-lookup"><span data-stu-id="90cfe-117">Managed DeviceId</span></span>|
|<span data-ttu-id="90cfe-118">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="90cfe-118">managedDeviceName</span></span>|<span data-ttu-id="90cfe-119">String</span><span class="sxs-lookup"><span data-stu-id="90cfe-119">String</span></span>|<span data-ttu-id="90cfe-120">Nome do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="90cfe-120">Managed Device Name</span></span>|
|<span data-ttu-id="90cfe-121">deviceType</span><span class="sxs-lookup"><span data-stu-id="90cfe-121">deviceType</span></span>|[<span data-ttu-id="90cfe-122">deviceType</span><span class="sxs-lookup"><span data-stu-id="90cfe-122">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="90cfe-123">Tipo de dispositivo de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="90cfe-123">Managed Device Device Type.</span></span> <span data-ttu-id="90cfe-124">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` , `androidForWork` , `androidEnterprise` , `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` `unknown` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="90cfe-124">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="90cfe-125">complianceState</span><span class="sxs-lookup"><span data-stu-id="90cfe-125">complianceState</span></span>|[<span data-ttu-id="90cfe-126">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="90cfe-126">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="90cfe-127">ComplianceStatus de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="90cfe-127">Managed Device ComplianceStatus.</span></span> <span data-ttu-id="90cfe-128">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="90cfe-128">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="90cfe-129">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="90cfe-129">retireAfterDateTime</span></span>|<span data-ttu-id="90cfe-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90cfe-130">DateTimeOffset</span></span>|<span data-ttu-id="90cfe-131">Desativação de dispositivo gerenciado após DateTime</span><span class="sxs-lookup"><span data-stu-id="90cfe-131">Managed Device Retire After DateTime</span></span>|
|<span data-ttu-id="90cfe-132">managementAgent</span><span class="sxs-lookup"><span data-stu-id="90cfe-132">managementAgent</span></span>|[<span data-ttu-id="90cfe-133">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="90cfe-133">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="90cfe-134">ManagementAgentType de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="90cfe-134">Managed Device ManagementAgentType.</span></span> <span data-ttu-id="90cfe-135">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="90cfe-135">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="90cfe-136">ownerType</span><span class="sxs-lookup"><span data-stu-id="90cfe-136">ownerType</span></span>|[<span data-ttu-id="90cfe-137">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="90cfe-137">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="90cfe-138">ManagedDeviceOwnerType de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="90cfe-138">Managed Device ManagedDeviceOwnerType.</span></span> <span data-ttu-id="90cfe-139">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="90cfe-139">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="90cfe-140">deviceCompliancePolicyName</span><span class="sxs-lookup"><span data-stu-id="90cfe-140">deviceCompliancePolicyName</span></span>|<span data-ttu-id="90cfe-141">String</span><span class="sxs-lookup"><span data-stu-id="90cfe-141">String</span></span>|<span data-ttu-id="90cfe-142">Nome da política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="90cfe-142">Device Compliance Policy Name</span></span>|
|<span data-ttu-id="90cfe-143">deviceCompliancePolicyId</span><span class="sxs-lookup"><span data-stu-id="90cfe-143">deviceCompliancePolicyId</span></span>|<span data-ttu-id="90cfe-144">String</span><span class="sxs-lookup"><span data-stu-id="90cfe-144">String</span></span>|<span data-ttu-id="90cfe-145">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="90cfe-145">Device Compliance PolicyId</span></span>|
|<span data-ttu-id="90cfe-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90cfe-146">roleScopeTagIds</span></span>|<span data-ttu-id="90cfe-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="90cfe-147">String collection</span></span>|<span data-ttu-id="90cfe-148">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="90cfe-148">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90cfe-149">Relações</span><span class="sxs-lookup"><span data-stu-id="90cfe-149">Relationships</span></span>
<span data-ttu-id="90cfe-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90cfe-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90cfe-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90cfe-151">JSON Representation</span></span>
<span data-ttu-id="90cfe-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90cfe-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.retireScheduledManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.retireScheduledManagedDevice",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "deviceType": "String",
  "complianceState": "String",
  "retireAfterDateTime": "String (timestamp)",
  "managementAgent": "String",
  "ownerType": "String",
  "deviceCompliancePolicyName": "String",
  "deviceCompliancePolicyId": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




