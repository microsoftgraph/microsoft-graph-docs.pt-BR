---
title: tipo de recurso comanagementEligibleDeviceEntity
description: tipo de recurso comanagementEligibleDeviceEntity
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5ad068a348eabaceafd9ca736f27cf6fda3218e
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636550"
---
# <a name="comanagementeligibledeviceentity-resource-type"></a><span data-ttu-id="fecf6-103">tipo de recurso comanagementEligibleDeviceEntity</span><span class="sxs-lookup"><span data-stu-id="fecf6-103">comanagementEligibleDeviceEntity resource type</span></span>

> <span data-ttu-id="fecf6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fecf6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fecf6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fecf6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fecf6-106">Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fecf6-106">Managed Device Mobile App Configuration State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="fecf6-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fecf6-107">Methods</span></span>
|<span data-ttu-id="fecf6-108">Método</span><span class="sxs-lookup"><span data-stu-id="fecf6-108">Method</span></span>|<span data-ttu-id="fecf6-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fecf6-109">Return Type</span></span>|<span data-ttu-id="fecf6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fecf6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fecf6-111">Listar comanagementEligibleDeviceEntity</span><span class="sxs-lookup"><span data-stu-id="fecf6-111">List comanagementEligibleDeviceEntity</span></span>](../api/intune-device-comanagementEligibleDeviceEntity-list.md)|<span data-ttu-id="fecf6-112">coleção [comanagementEligibleDeviceEntity](../resources/intune-device-comanagementEligibleDeviceEntity.md)</span><span class="sxs-lookup"><span data-stu-id="fecf6-112">[comanagementEligibleDeviceEntity](../resources/intune-device-comanagementEligibleDeviceEntity.md) collection</span></span>|<span data-ttu-id="fecf6-113">Listar Propriedades e relações dos objetos [comanagementEligibleDeviceEntity](../resources/intune-device-comanagementEligibleDeviceEntity.md) .</span><span class="sxs-lookup"><span data-stu-id="fecf6-113">List properties and relationships of the [comanagementEligibleDeviceEntity](../resources/intune-device-comanagementEligibleDeviceEntity.md) objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="fecf6-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fecf6-114">Properties</span></span>
|<span data-ttu-id="fecf6-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fecf6-115">Property</span></span>|<span data-ttu-id="fecf6-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="fecf6-116">Type</span></span>|<span data-ttu-id="fecf6-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="fecf6-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fecf6-118">id</span><span class="sxs-lookup"><span data-stu-id="fecf6-118">id</span></span>|<span data-ttu-id="fecf6-119">String</span><span class="sxs-lookup"><span data-stu-id="fecf6-119">String</span></span>|<span data-ttu-id="fecf6-120">ID exclusiva do EligibleDeviceEntity</span><span class="sxs-lookup"><span data-stu-id="fecf6-120">Unique Id of the EligibleDeviceEntity</span></span>|
|<span data-ttu-id="fecf6-121">deviceId</span><span class="sxs-lookup"><span data-stu-id="fecf6-121">deviceId</span></span>|<span data-ttu-id="fecf6-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fecf6-122">String</span></span>|<span data-ttu-id="fecf6-123">DeviceId</span><span class="sxs-lookup"><span data-stu-id="fecf6-123">DeviceId</span></span>|
|<span data-ttu-id="fecf6-124">deviceName</span><span class="sxs-lookup"><span data-stu-id="fecf6-124">deviceName</span></span>|<span data-ttu-id="fecf6-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fecf6-125">String</span></span>|<span data-ttu-id="fecf6-126">DeviceName</span><span class="sxs-lookup"><span data-stu-id="fecf6-126">DeviceName</span></span>|
|<span data-ttu-id="fecf6-127">deviceType</span><span class="sxs-lookup"><span data-stu-id="fecf6-127">deviceType</span></span>|<span data-ttu-id="fecf6-128">String</span><span class="sxs-lookup"><span data-stu-id="fecf6-128">String</span></span>|<span data-ttu-id="fecf6-129">DeviceType</span><span class="sxs-lookup"><span data-stu-id="fecf6-129">DeviceType</span></span>|
|<span data-ttu-id="fecf6-130">clientRegistrationStatus</span><span class="sxs-lookup"><span data-stu-id="fecf6-130">clientRegistrationStatus</span></span>|[<span data-ttu-id="fecf6-131">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="fecf6-131">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="fecf6-132">ClientRegistrationStatus.</span><span class="sxs-lookup"><span data-stu-id="fecf6-132">ClientRegistrationStatus.</span></span> <span data-ttu-id="fecf6-133">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="fecf6-133">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="fecf6-134">ownerType</span><span class="sxs-lookup"><span data-stu-id="fecf6-134">ownerType</span></span>|[<span data-ttu-id="fecf6-135">ownerType</span><span class="sxs-lookup"><span data-stu-id="fecf6-135">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="fecf6-136">OwnerType.</span><span class="sxs-lookup"><span data-stu-id="fecf6-136">OwnerType.</span></span> <span data-ttu-id="fecf6-137">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="fecf6-137">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="fecf6-138">managementAgents</span><span class="sxs-lookup"><span data-stu-id="fecf6-138">managementAgents</span></span>|[<span data-ttu-id="fecf6-139">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="fecf6-139">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="fecf6-140">ManagementAgentType.</span><span class="sxs-lookup"><span data-stu-id="fecf6-140">ManagementAgentType.</span></span> <span data-ttu-id="fecf6-141">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="fecf6-141">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="fecf6-142">ManagementState</span><span class="sxs-lookup"><span data-stu-id="fecf6-142">managementState</span></span>|[<span data-ttu-id="fecf6-143">ManagementState</span><span class="sxs-lookup"><span data-stu-id="fecf6-143">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="fecf6-144">ManagementState.</span><span class="sxs-lookup"><span data-stu-id="fecf6-144">ManagementState.</span></span> <span data-ttu-id="fecf6-145">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="fecf6-145">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="fecf6-146">referenceId</span><span class="sxs-lookup"><span data-stu-id="fecf6-146">referenceId</span></span>|<span data-ttu-id="fecf6-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fecf6-147">String</span></span>|<span data-ttu-id="fecf6-148">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="fecf6-148">ReferenceId</span></span>|
|<span data-ttu-id="fecf6-149">mdmStatus</span><span class="sxs-lookup"><span data-stu-id="fecf6-149">mdmStatus</span></span>|<span data-ttu-id="fecf6-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fecf6-150">String</span></span>|<span data-ttu-id="fecf6-151">MDMStatus</span><span class="sxs-lookup"><span data-stu-id="fecf6-151">MDMStatus</span></span>|
|<span data-ttu-id="fecf6-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="fecf6-152">osVersion</span></span>|<span data-ttu-id="fecf6-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fecf6-153">String</span></span>|<span data-ttu-id="fecf6-154">OSVersion</span><span class="sxs-lookup"><span data-stu-id="fecf6-154">OSVersion</span></span>|
|<span data-ttu-id="fecf6-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="fecf6-155">serialNumber</span></span>|<span data-ttu-id="fecf6-156">String</span><span class="sxs-lookup"><span data-stu-id="fecf6-156">String</span></span>|<span data-ttu-id="fecf6-157">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="fecf6-157">SerialNumber</span></span>|
|<span data-ttu-id="fecf6-158">fabricante</span><span class="sxs-lookup"><span data-stu-id="fecf6-158">manufacturer</span></span>|<span data-ttu-id="fecf6-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fecf6-159">String</span></span>|<span data-ttu-id="fecf6-160">Fabricantes</span><span class="sxs-lookup"><span data-stu-id="fecf6-160">Manufacturer</span></span>|
|<span data-ttu-id="fecf6-161">modelo</span><span class="sxs-lookup"><span data-stu-id="fecf6-161">model</span></span>|<span data-ttu-id="fecf6-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fecf6-162">String</span></span>|<span data-ttu-id="fecf6-163">Modelo</span><span class="sxs-lookup"><span data-stu-id="fecf6-163">Model</span></span>|
|<span data-ttu-id="fecf6-164">osDescription</span><span class="sxs-lookup"><span data-stu-id="fecf6-164">osDescription</span></span>|<span data-ttu-id="fecf6-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fecf6-165">String</span></span>|<span data-ttu-id="fecf6-166">OSDescription</span><span class="sxs-lookup"><span data-stu-id="fecf6-166">OSDescription</span></span>|
|<span data-ttu-id="fecf6-167">EntityName</span><span class="sxs-lookup"><span data-stu-id="fecf6-167">entitySource</span></span>|<span data-ttu-id="fecf6-168">Int32</span><span class="sxs-lookup"><span data-stu-id="fecf6-168">Int32</span></span>|<span data-ttu-id="fecf6-169">EntityName</span><span class="sxs-lookup"><span data-stu-id="fecf6-169">EntitySource</span></span>|
|<span data-ttu-id="fecf6-170">userId</span><span class="sxs-lookup"><span data-stu-id="fecf6-170">userId</span></span>|<span data-ttu-id="fecf6-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fecf6-171">String</span></span>|<span data-ttu-id="fecf6-172">UserId</span><span class="sxs-lookup"><span data-stu-id="fecf6-172">UserId</span></span>|
|<span data-ttu-id="fecf6-173">UPN</span><span class="sxs-lookup"><span data-stu-id="fecf6-173">upn</span></span>|<span data-ttu-id="fecf6-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fecf6-174">String</span></span>|<span data-ttu-id="fecf6-175">UPN</span><span class="sxs-lookup"><span data-stu-id="fecf6-175">UPN</span></span>|
|<span data-ttu-id="fecf6-176">userEmail</span><span class="sxs-lookup"><span data-stu-id="fecf6-176">userEmail</span></span>|<span data-ttu-id="fecf6-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fecf6-177">String</span></span>|<span data-ttu-id="fecf6-178">UserEmail</span><span class="sxs-lookup"><span data-stu-id="fecf6-178">UserEmail</span></span>|
|<span data-ttu-id="fecf6-179">userName</span><span class="sxs-lookup"><span data-stu-id="fecf6-179">userName</span></span>|<span data-ttu-id="fecf6-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fecf6-180">String</span></span>|<span data-ttu-id="fecf6-181">UserName</span><span class="sxs-lookup"><span data-stu-id="fecf6-181">UserName</span></span>|
|<span data-ttu-id="fecf6-182">coManageEligibleStatus</span><span class="sxs-lookup"><span data-stu-id="fecf6-182">coManageEligibleStatus</span></span>|[<span data-ttu-id="fecf6-183">coManagementEligibleType</span><span class="sxs-lookup"><span data-stu-id="fecf6-183">coManagementEligibleType</span></span>](../resources/intune-devices-comanagementeligibletype.md)|<span data-ttu-id="fecf6-184">CoManagementEligibleType.</span><span class="sxs-lookup"><span data-stu-id="fecf6-184">CoManagementEligibleType.</span></span> <span data-ttu-id="fecf6-185">Os valores possíveis são: `coManaged`, `eligible`, `eligibleButNotAadJoined`, `needsOSUpdate`.</span><span class="sxs-lookup"><span data-stu-id="fecf6-185">Possible values are: `coManaged`, `eligible`, `eligibleButNotAadJoined`, `needsOSUpdate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fecf6-186">Relações</span><span class="sxs-lookup"><span data-stu-id="fecf6-186">Relationships</span></span>
<span data-ttu-id="fecf6-187">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fecf6-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fecf6-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fecf6-188">JSON Representation</span></span>
<span data-ttu-id="fecf6-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fecf6-189">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleDeviceEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDeviceEntity",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "deviceType": "String",
  "clientRegistrationStatus": "String",
  "ownerType": "String",
  "managementAgents": "String",
  "managementState": "String",
  "referenceId": "String",
  "mdmStatus": "String",
  "osVersion": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "osDescription": "String",
  "entitySource": 1024,
  "userId": "String",
  "upn": "String",
  "userEmail": "String",
  "userName": "String",
  "coManageEligibleStatus": "String"
}
```

