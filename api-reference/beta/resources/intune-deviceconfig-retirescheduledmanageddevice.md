---
title: tipo de recurso retireScheduledManagedDevice
description: ManagedDevices que estão agendados para desativação
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 230d688429bb98361c04ad3d28789e0e886361fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529448"
---
# <a name="retirescheduledmanageddevice-resource-type"></a><span data-ttu-id="4d910-103">tipo de recurso retireScheduledManagedDevice</span><span class="sxs-lookup"><span data-stu-id="4d910-103">retireScheduledManagedDevice resource type</span></span>

<span data-ttu-id="4d910-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4d910-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d910-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4d910-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d910-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4d910-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d910-107">ManagedDevices que estão agendados para desativação</span><span class="sxs-lookup"><span data-stu-id="4d910-107">ManagedDevices that are scheduled for retire</span></span>

## <a name="properties"></a><span data-ttu-id="4d910-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d910-108">Properties</span></span>
|<span data-ttu-id="4d910-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d910-109">Property</span></span>|<span data-ttu-id="4d910-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d910-110">Type</span></span>|<span data-ttu-id="4d910-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d910-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d910-112">id</span><span class="sxs-lookup"><span data-stu-id="4d910-112">id</span></span>|<span data-ttu-id="4d910-113">String</span><span class="sxs-lookup"><span data-stu-id="4d910-113">String</span></span>|<span data-ttu-id="4d910-114">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4d910-114">Key of the entity.</span></span>|
|<span data-ttu-id="4d910-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="4d910-115">managedDeviceId</span></span>|<span data-ttu-id="4d910-116">String</span><span class="sxs-lookup"><span data-stu-id="4d910-116">String</span></span>|<span data-ttu-id="4d910-117">DeviceID gerenciado</span><span class="sxs-lookup"><span data-stu-id="4d910-117">Managed DeviceId</span></span>|
|<span data-ttu-id="4d910-118">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="4d910-118">managedDeviceName</span></span>|<span data-ttu-id="4d910-119">String</span><span class="sxs-lookup"><span data-stu-id="4d910-119">String</span></span>|<span data-ttu-id="4d910-120">Nome do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="4d910-120">Managed Device Name</span></span>|
|<span data-ttu-id="4d910-121">deviceType</span><span class="sxs-lookup"><span data-stu-id="4d910-121">deviceType</span></span>|[<span data-ttu-id="4d910-122">deviceType</span><span class="sxs-lookup"><span data-stu-id="4d910-122">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="4d910-123">Tipo de dispositivo de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="4d910-123">Managed Device Device Type.</span></span> <span data-ttu-id="4d910-124">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="4d910-124">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="4d910-125">complianceState</span><span class="sxs-lookup"><span data-stu-id="4d910-125">complianceState</span></span>|[<span data-ttu-id="4d910-126">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4d910-126">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4d910-127">ComplianceStatus de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="4d910-127">Managed Device ComplianceStatus.</span></span> <span data-ttu-id="4d910-128">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4d910-128">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4d910-129">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="4d910-129">retireAfterDateTime</span></span>|<span data-ttu-id="4d910-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d910-130">DateTimeOffset</span></span>|<span data-ttu-id="4d910-131">Desativação de dispositivo gerenciado após DateTime</span><span class="sxs-lookup"><span data-stu-id="4d910-131">Managed Device Retire After DateTime</span></span>|
|<span data-ttu-id="4d910-132">managementAgent</span><span class="sxs-lookup"><span data-stu-id="4d910-132">managementAgent</span></span>|[<span data-ttu-id="4d910-133">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="4d910-133">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="4d910-134">ManagementAgentType de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="4d910-134">Managed Device ManagementAgentType.</span></span> <span data-ttu-id="4d910-135">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="4d910-135">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="4d910-136">ownerType</span><span class="sxs-lookup"><span data-stu-id="4d910-136">ownerType</span></span>|[<span data-ttu-id="4d910-137">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="4d910-137">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="4d910-138">ManagedDeviceOwnerType de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="4d910-138">Managed Device ManagedDeviceOwnerType.</span></span> <span data-ttu-id="4d910-139">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="4d910-139">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="4d910-140">deviceCompliancePolicyName</span><span class="sxs-lookup"><span data-stu-id="4d910-140">deviceCompliancePolicyName</span></span>|<span data-ttu-id="4d910-141">String</span><span class="sxs-lookup"><span data-stu-id="4d910-141">String</span></span>|<span data-ttu-id="4d910-142">Nome da política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="4d910-142">Device Compliance Policy Name</span></span>|
|<span data-ttu-id="4d910-143">deviceCompliancePolicyId</span><span class="sxs-lookup"><span data-stu-id="4d910-143">deviceCompliancePolicyId</span></span>|<span data-ttu-id="4d910-144">String</span><span class="sxs-lookup"><span data-stu-id="4d910-144">String</span></span>|<span data-ttu-id="4d910-145">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="4d910-145">Device Compliance PolicyId</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d910-146">Relações</span><span class="sxs-lookup"><span data-stu-id="4d910-146">Relationships</span></span>
<span data-ttu-id="4d910-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4d910-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d910-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d910-148">JSON Representation</span></span>
<span data-ttu-id="4d910-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d910-149">Here is a JSON representation of the resource.</span></span>
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



