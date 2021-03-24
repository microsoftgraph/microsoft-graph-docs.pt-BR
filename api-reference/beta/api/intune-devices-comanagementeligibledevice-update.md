---
title: Atualizar comanagementEligibleDevice
description: Atualize as propriedades de um objeto comanagementEligibleDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6322b31ac8a9e998e4a9a7c10ce5e9276c7fcbc9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146563"
---
# <a name="update-comanagementeligibledevice"></a><span data-ttu-id="cb4fc-103">Atualizar comanagementEligibleDevice</span><span class="sxs-lookup"><span data-stu-id="cb4fc-103">Update comanagementEligibleDevice</span></span>

<span data-ttu-id="cb4fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb4fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb4fc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb4fc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb4fc-107">Atualize as propriedades de [um objeto comanagementEligibleDevice.](../resources/intune-devices-comanagementeligibledevice.md)</span><span class="sxs-lookup"><span data-stu-id="cb4fc-107">Update the properties of a [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb4fc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb4fc-108">Prerequisites</span></span>
<span data-ttu-id="cb4fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb4fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb4fc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb4fc-111">Permission type</span></span>|<span data-ttu-id="cb4fc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb4fc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb4fc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb4fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb4fc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb4fc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cb4fc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb4fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb4fc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-116">Not supported.</span></span>|
|<span data-ttu-id="cb4fc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb4fc-117">Application</span></span>|<span data-ttu-id="cb4fc-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb4fc-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb4fc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb4fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="cb4fc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb4fc-120">Request headers</span></span>
|<span data-ttu-id="cb4fc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb4fc-121">Header</span></span>|<span data-ttu-id="cb4fc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cb4fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb4fc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb4fc-123">Authorization</span></span>|<span data-ttu-id="cb4fc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb4fc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cb4fc-125">Accept</span></span>|<span data-ttu-id="cb4fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb4fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb4fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb4fc-127">Request body</span></span>
<span data-ttu-id="cb4fc-128">No corpo da solicitação, fornece uma representação JSON para o [objeto comanagementEligibleDevice.](../resources/intune-devices-comanagementeligibledevice.md)</span><span class="sxs-lookup"><span data-stu-id="cb4fc-128">In the request body, supply a JSON representation for the [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object.</span></span>

<span data-ttu-id="cb4fc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md).</span><span class="sxs-lookup"><span data-stu-id="cb4fc-129">The following table shows the properties that are required when you create the [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md).</span></span>

|<span data-ttu-id="cb4fc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb4fc-130">Property</span></span>|<span data-ttu-id="cb4fc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb4fc-131">Type</span></span>|<span data-ttu-id="cb4fc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb4fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb4fc-133">id</span><span class="sxs-lookup"><span data-stu-id="cb4fc-133">id</span></span>|<span data-ttu-id="cb4fc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb4fc-134">String</span></span>|<span data-ttu-id="cb4fc-135">ID exclusiva do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cb4fc-135">Unique Id for the device</span></span>|
|<span data-ttu-id="cb4fc-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="cb4fc-136">deviceName</span></span>|<span data-ttu-id="cb4fc-137">String</span><span class="sxs-lookup"><span data-stu-id="cb4fc-137">String</span></span>|<span data-ttu-id="cb4fc-138">DeviceName</span><span class="sxs-lookup"><span data-stu-id="cb4fc-138">DeviceName</span></span>|
|<span data-ttu-id="cb4fc-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="cb4fc-139">deviceType</span></span>|[<span data-ttu-id="cb4fc-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="cb4fc-140">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="cb4fc-141">DeviceType.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-141">DeviceType.</span></span> <span data-ttu-id="cb4fc-142">Os valores possíveis são: `desktop` , , , , , , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC`</span><span class="sxs-lookup"><span data-stu-id="cb4fc-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="cb4fc-143">clientRegistrationStatus</span><span class="sxs-lookup"><span data-stu-id="cb4fc-143">clientRegistrationStatus</span></span>|[<span data-ttu-id="cb4fc-144">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="cb4fc-144">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="cb4fc-145">ClientRegistrationStatus.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-145">ClientRegistrationStatus.</span></span> <span data-ttu-id="cb4fc-146">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-146">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="cb4fc-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="cb4fc-147">ownerType</span></span>|[<span data-ttu-id="cb4fc-148">ownerType</span><span class="sxs-lookup"><span data-stu-id="cb4fc-148">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="cb4fc-149">OwnerType.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-149">OwnerType.</span></span> <span data-ttu-id="cb4fc-150">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="cb4fc-151">managementAgents</span><span class="sxs-lookup"><span data-stu-id="cb4fc-151">managementAgents</span></span>|[<span data-ttu-id="cb4fc-152">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="cb4fc-152">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="cb4fc-153">ManagementAgents.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-153">ManagementAgents.</span></span> <span data-ttu-id="cb4fc-154">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-154">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="cb4fc-155">managementState</span><span class="sxs-lookup"><span data-stu-id="cb4fc-155">managementState</span></span>|[<span data-ttu-id="cb4fc-156">managementState</span><span class="sxs-lookup"><span data-stu-id="cb4fc-156">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="cb4fc-157">ManagementState.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-157">ManagementState.</span></span> <span data-ttu-id="cb4fc-158">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-158">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="cb4fc-159">referenceId</span><span class="sxs-lookup"><span data-stu-id="cb4fc-159">referenceId</span></span>|<span data-ttu-id="cb4fc-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb4fc-160">String</span></span>|<span data-ttu-id="cb4fc-161">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="cb4fc-161">ReferenceId</span></span>|
|<span data-ttu-id="cb4fc-162">mdmStatus</span><span class="sxs-lookup"><span data-stu-id="cb4fc-162">mdmStatus</span></span>|<span data-ttu-id="cb4fc-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb4fc-163">String</span></span>|<span data-ttu-id="cb4fc-164">MDMStatus</span><span class="sxs-lookup"><span data-stu-id="cb4fc-164">MDMStatus</span></span>|
|<span data-ttu-id="cb4fc-165">osVersion</span><span class="sxs-lookup"><span data-stu-id="cb4fc-165">osVersion</span></span>|<span data-ttu-id="cb4fc-166">String</span><span class="sxs-lookup"><span data-stu-id="cb4fc-166">String</span></span>|<span data-ttu-id="cb4fc-167">OSVersion</span><span class="sxs-lookup"><span data-stu-id="cb4fc-167">OSVersion</span></span>|
|<span data-ttu-id="cb4fc-168">serialNumber</span><span class="sxs-lookup"><span data-stu-id="cb4fc-168">serialNumber</span></span>|<span data-ttu-id="cb4fc-169">String</span><span class="sxs-lookup"><span data-stu-id="cb4fc-169">String</span></span>|<span data-ttu-id="cb4fc-170">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="cb4fc-170">SerialNumber</span></span>|
|<span data-ttu-id="cb4fc-171">fabricante</span><span class="sxs-lookup"><span data-stu-id="cb4fc-171">manufacturer</span></span>|<span data-ttu-id="cb4fc-172">String</span><span class="sxs-lookup"><span data-stu-id="cb4fc-172">String</span></span>|<span data-ttu-id="cb4fc-173">Fabricante</span><span class="sxs-lookup"><span data-stu-id="cb4fc-173">Manufacturer</span></span>|
|<span data-ttu-id="cb4fc-174">modelo</span><span class="sxs-lookup"><span data-stu-id="cb4fc-174">model</span></span>|<span data-ttu-id="cb4fc-175">String</span><span class="sxs-lookup"><span data-stu-id="cb4fc-175">String</span></span>|<span data-ttu-id="cb4fc-176">Modelo</span><span class="sxs-lookup"><span data-stu-id="cb4fc-176">Model</span></span>|
|<span data-ttu-id="cb4fc-177">osDescription</span><span class="sxs-lookup"><span data-stu-id="cb4fc-177">osDescription</span></span>|<span data-ttu-id="cb4fc-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb4fc-178">String</span></span>|<span data-ttu-id="cb4fc-179">OSDescription</span><span class="sxs-lookup"><span data-stu-id="cb4fc-179">OSDescription</span></span>|
|<span data-ttu-id="cb4fc-180">entitySource</span><span class="sxs-lookup"><span data-stu-id="cb4fc-180">entitySource</span></span>|<span data-ttu-id="cb4fc-181">Int32</span><span class="sxs-lookup"><span data-stu-id="cb4fc-181">Int32</span></span>|<span data-ttu-id="cb4fc-182">EntitySource</span><span class="sxs-lookup"><span data-stu-id="cb4fc-182">EntitySource</span></span>|
|<span data-ttu-id="cb4fc-183">userId</span><span class="sxs-lookup"><span data-stu-id="cb4fc-183">userId</span></span>|<span data-ttu-id="cb4fc-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb4fc-184">String</span></span>|<span data-ttu-id="cb4fc-185">UserId</span><span class="sxs-lookup"><span data-stu-id="cb4fc-185">UserId</span></span>|
|<span data-ttu-id="cb4fc-186">upn</span><span class="sxs-lookup"><span data-stu-id="cb4fc-186">upn</span></span>|<span data-ttu-id="cb4fc-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb4fc-187">String</span></span>|<span data-ttu-id="cb4fc-188">UPN</span><span class="sxs-lookup"><span data-stu-id="cb4fc-188">UPN</span></span>|
|<span data-ttu-id="cb4fc-189">userEmail</span><span class="sxs-lookup"><span data-stu-id="cb4fc-189">userEmail</span></span>|<span data-ttu-id="cb4fc-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb4fc-190">String</span></span>|<span data-ttu-id="cb4fc-191">UserEmail</span><span class="sxs-lookup"><span data-stu-id="cb4fc-191">UserEmail</span></span>|
|<span data-ttu-id="cb4fc-192">userName</span><span class="sxs-lookup"><span data-stu-id="cb4fc-192">userName</span></span>|<span data-ttu-id="cb4fc-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb4fc-193">String</span></span>|<span data-ttu-id="cb4fc-194">UserName</span><span class="sxs-lookup"><span data-stu-id="cb4fc-194">UserName</span></span>|
|<span data-ttu-id="cb4fc-195">status</span><span class="sxs-lookup"><span data-stu-id="cb4fc-195">status</span></span>|[<span data-ttu-id="cb4fc-196">comanagementEligibleType</span><span class="sxs-lookup"><span data-stu-id="cb4fc-196">comanagementEligibleType</span></span>](../resources/intune-devices-comanagementeligibletype.md)|<span data-ttu-id="cb4fc-197">ComanagementEligibleStatus.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-197">ComanagementEligibleStatus.</span></span> <span data-ttu-id="cb4fc-198">Os valores possíveis são: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-198">Possible values are: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.</span></span>|



## <a name="response"></a><span data-ttu-id="cb4fc-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb4fc-199">Response</span></span>
<span data-ttu-id="cb4fc-200">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-200">If successful, this method returns a `200 OK` response code and an updated [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb4fc-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb4fc-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb4fc-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb4fc-202">Request</span></span>
<span data-ttu-id="cb4fc-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
Content-type: application/json
Content-length: 714

{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "deviceName": "Device Name value",
  "deviceType": "windowsRT",
  "clientRegistrationStatus": "registered",
  "ownerType": "company",
  "managementAgents": "mdm",
  "managementState": "retirePending",
  "referenceId": "Reference Id value",
  "mdmStatus": "Mdm Status value",
  "osVersion": "Os Version value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "osDescription": "Os Description value",
  "entitySource": 12,
  "userId": "User Id value",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "status": "eligible"
}
```

### <a name="response"></a><span data-ttu-id="cb4fc-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb4fc-204">Response</span></span>
<span data-ttu-id="cb4fc-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb4fc-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "id": "ac20683b-683b-ac20-3b68-20ac3b6820ac",
  "deviceName": "Device Name value",
  "deviceType": "windowsRT",
  "clientRegistrationStatus": "registered",
  "ownerType": "company",
  "managementAgents": "mdm",
  "managementState": "retirePending",
  "referenceId": "Reference Id value",
  "mdmStatus": "Mdm Status value",
  "osVersion": "Os Version value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "osDescription": "Os Description value",
  "entitySource": 12,
  "userId": "User Id value",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "status": "eligible"
}
```




