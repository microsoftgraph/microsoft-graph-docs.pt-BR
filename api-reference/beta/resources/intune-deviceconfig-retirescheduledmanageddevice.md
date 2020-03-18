---
title: tipo de recurso retireScheduledManagedDevice
description: ManagedDevices que estão agendados para desativação
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9557780ffbf2d82edecdcdcaa747fe3cbd1bf8c3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787597"
---
# <a name="retirescheduledmanageddevice-resource-type"></a><span data-ttu-id="70c34-103">tipo de recurso retireScheduledManagedDevice</span><span class="sxs-lookup"><span data-stu-id="70c34-103">retireScheduledManagedDevice resource type</span></span>

> <span data-ttu-id="70c34-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="70c34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70c34-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70c34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70c34-106">ManagedDevices que estão agendados para desativação</span><span class="sxs-lookup"><span data-stu-id="70c34-106">ManagedDevices that are scheduled for retire</span></span>

## <a name="properties"></a><span data-ttu-id="70c34-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70c34-107">Properties</span></span>
|<span data-ttu-id="70c34-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70c34-108">Property</span></span>|<span data-ttu-id="70c34-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="70c34-109">Type</span></span>|<span data-ttu-id="70c34-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="70c34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70c34-111">id</span><span class="sxs-lookup"><span data-stu-id="70c34-111">id</span></span>|<span data-ttu-id="70c34-112">String</span><span class="sxs-lookup"><span data-stu-id="70c34-112">String</span></span>|<span data-ttu-id="70c34-113">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="70c34-113">Key of the entity.</span></span>|
|<span data-ttu-id="70c34-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="70c34-114">managedDeviceId</span></span>|<span data-ttu-id="70c34-115">String</span><span class="sxs-lookup"><span data-stu-id="70c34-115">String</span></span>|<span data-ttu-id="70c34-116">DeviceID gerenciado</span><span class="sxs-lookup"><span data-stu-id="70c34-116">Managed DeviceId</span></span>|
|<span data-ttu-id="70c34-117">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="70c34-117">managedDeviceName</span></span>|<span data-ttu-id="70c34-118">String</span><span class="sxs-lookup"><span data-stu-id="70c34-118">String</span></span>|<span data-ttu-id="70c34-119">Nome do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="70c34-119">Managed Device Name</span></span>|
|<span data-ttu-id="70c34-120">deviceType</span><span class="sxs-lookup"><span data-stu-id="70c34-120">deviceType</span></span>|[<span data-ttu-id="70c34-121">deviceType</span><span class="sxs-lookup"><span data-stu-id="70c34-121">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="70c34-122">Tipo de dispositivo de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="70c34-122">Managed Device Device Type.</span></span> <span data-ttu-id="70c34-123">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="70c34-123">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="70c34-124">complianceState</span><span class="sxs-lookup"><span data-stu-id="70c34-124">complianceState</span></span>|[<span data-ttu-id="70c34-125">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="70c34-125">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="70c34-126">ComplianceStatus de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="70c34-126">Managed Device ComplianceStatus.</span></span> <span data-ttu-id="70c34-127">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="70c34-127">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="70c34-128">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="70c34-128">retireAfterDateTime</span></span>|<span data-ttu-id="70c34-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70c34-129">DateTimeOffset</span></span>|<span data-ttu-id="70c34-130">Desativação de dispositivo gerenciado após DateTime</span><span class="sxs-lookup"><span data-stu-id="70c34-130">Managed Device Retire After DateTime</span></span>|
|<span data-ttu-id="70c34-131">managementAgent</span><span class="sxs-lookup"><span data-stu-id="70c34-131">managementAgent</span></span>|[<span data-ttu-id="70c34-132">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="70c34-132">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="70c34-133">ManagementAgentType de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="70c34-133">Managed Device ManagementAgentType.</span></span> <span data-ttu-id="70c34-134">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="70c34-134">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="70c34-135">ownerType</span><span class="sxs-lookup"><span data-stu-id="70c34-135">ownerType</span></span>|[<span data-ttu-id="70c34-136">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="70c34-136">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="70c34-137">ManagedDeviceOwnerType de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="70c34-137">Managed Device ManagedDeviceOwnerType.</span></span> <span data-ttu-id="70c34-138">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="70c34-138">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="70c34-139">deviceCompliancePolicyName</span><span class="sxs-lookup"><span data-stu-id="70c34-139">deviceCompliancePolicyName</span></span>|<span data-ttu-id="70c34-140">String</span><span class="sxs-lookup"><span data-stu-id="70c34-140">String</span></span>|<span data-ttu-id="70c34-141">Nome da política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="70c34-141">Device Compliance Policy Name</span></span>|
|<span data-ttu-id="70c34-142">deviceCompliancePolicyId</span><span class="sxs-lookup"><span data-stu-id="70c34-142">deviceCompliancePolicyId</span></span>|<span data-ttu-id="70c34-143">String</span><span class="sxs-lookup"><span data-stu-id="70c34-143">String</span></span>|<span data-ttu-id="70c34-144">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="70c34-144">Device Compliance PolicyId</span></span>|

## <a name="relationships"></a><span data-ttu-id="70c34-145">Relações</span><span class="sxs-lookup"><span data-stu-id="70c34-145">Relationships</span></span>
<span data-ttu-id="70c34-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70c34-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70c34-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70c34-147">JSON Representation</span></span>
<span data-ttu-id="70c34-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70c34-148">Here is a JSON representation of the resource.</span></span>
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
  "deviceCompliancePolicyId": "String"
}
```



