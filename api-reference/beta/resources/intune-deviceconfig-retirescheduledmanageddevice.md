---
title: tipo de recurso retireScheduledManagedDevice
description: ManagedDevices que estão agendados para desativação
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8b79f0541450f4d3c00e4f89f02405cd74545b49
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955515"
---
# <a name="retirescheduledmanageddevice-resource-type"></a><span data-ttu-id="932f3-103">tipo de recurso retireScheduledManagedDevice</span><span class="sxs-lookup"><span data-stu-id="932f3-103">retireScheduledManagedDevice resource type</span></span>

> <span data-ttu-id="932f3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="932f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="932f3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="932f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="932f3-106">ManagedDevices que estão agendados para desativação</span><span class="sxs-lookup"><span data-stu-id="932f3-106">ManagedDevices that are scheduled for retire</span></span>

## <a name="properties"></a><span data-ttu-id="932f3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="932f3-107">Properties</span></span>
|<span data-ttu-id="932f3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="932f3-108">Property</span></span>|<span data-ttu-id="932f3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="932f3-109">Type</span></span>|<span data-ttu-id="932f3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="932f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="932f3-111">id</span><span class="sxs-lookup"><span data-stu-id="932f3-111">id</span></span>|<span data-ttu-id="932f3-112">String</span><span class="sxs-lookup"><span data-stu-id="932f3-112">String</span></span>|<span data-ttu-id="932f3-113">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="932f3-113">Key of the entity.</span></span>|
|<span data-ttu-id="932f3-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="932f3-114">managedDeviceId</span></span>|<span data-ttu-id="932f3-115">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="932f3-115">String</span></span>|<span data-ttu-id="932f3-116">DeviceID gerenciado</span><span class="sxs-lookup"><span data-stu-id="932f3-116">Managed DeviceId</span></span>|
|<span data-ttu-id="932f3-117">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="932f3-117">managedDeviceName</span></span>|<span data-ttu-id="932f3-118">String</span><span class="sxs-lookup"><span data-stu-id="932f3-118">String</span></span>|<span data-ttu-id="932f3-119">Nome do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="932f3-119">Managed Device Name</span></span>|
|<span data-ttu-id="932f3-120">deviceType</span><span class="sxs-lookup"><span data-stu-id="932f3-120">deviceType</span></span>|[<span data-ttu-id="932f3-121">deviceType</span><span class="sxs-lookup"><span data-stu-id="932f3-121">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="932f3-122">Tipo de dispositivo de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="932f3-122">Managed Device Device Type.</span></span> <span data-ttu-id="932f3-123">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="932f3-123">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="932f3-124">complianceState</span><span class="sxs-lookup"><span data-stu-id="932f3-124">complianceState</span></span>|[<span data-ttu-id="932f3-125">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="932f3-125">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="932f3-126">ComplianceStatus de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="932f3-126">Managed Device ComplianceStatus.</span></span> <span data-ttu-id="932f3-127">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="932f3-127">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="932f3-128">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="932f3-128">retireAfterDateTime</span></span>|<span data-ttu-id="932f3-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="932f3-129">DateTimeOffset</span></span>|<span data-ttu-id="932f3-130">Desativação de dispositivo gerenciado após DateTime</span><span class="sxs-lookup"><span data-stu-id="932f3-130">Managed Device Retire After DateTime</span></span>|
|<span data-ttu-id="932f3-131">managementAgent</span><span class="sxs-lookup"><span data-stu-id="932f3-131">managementAgent</span></span>|[<span data-ttu-id="932f3-132">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="932f3-132">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="932f3-133">ManagementAgentType de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="932f3-133">Managed Device ManagementAgentType.</span></span> <span data-ttu-id="932f3-134">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="932f3-134">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="932f3-135">ownerType</span><span class="sxs-lookup"><span data-stu-id="932f3-135">ownerType</span></span>|[<span data-ttu-id="932f3-136">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="932f3-136">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="932f3-137">ManagedDeviceOwnerType de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="932f3-137">Managed Device ManagedDeviceOwnerType.</span></span> <span data-ttu-id="932f3-138">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="932f3-138">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="932f3-139">deviceCompliancePolicyName</span><span class="sxs-lookup"><span data-stu-id="932f3-139">deviceCompliancePolicyName</span></span>|<span data-ttu-id="932f3-140">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="932f3-140">String</span></span>|<span data-ttu-id="932f3-141">Nome da política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="932f3-141">Device Compliance Policy Name</span></span>|
|<span data-ttu-id="932f3-142">deviceCompliancePolicyId</span><span class="sxs-lookup"><span data-stu-id="932f3-142">deviceCompliancePolicyId</span></span>|<span data-ttu-id="932f3-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="932f3-143">String</span></span>|<span data-ttu-id="932f3-144">Política de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="932f3-144">Device Compliance PolicyId</span></span>|

## <a name="relationships"></a><span data-ttu-id="932f3-145">Relações</span><span class="sxs-lookup"><span data-stu-id="932f3-145">Relationships</span></span>
<span data-ttu-id="932f3-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="932f3-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="932f3-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="932f3-147">JSON Representation</span></span>
<span data-ttu-id="932f3-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="932f3-148">Here is a JSON representation of the resource.</span></span>
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



