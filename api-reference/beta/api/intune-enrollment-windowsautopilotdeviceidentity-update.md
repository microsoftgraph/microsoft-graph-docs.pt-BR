---
title: Atualizar windowsAutopilotDeviceIdentity
description: Atualiza as propriedades de um objeto windowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16b2f4dec305a2f721ffb785e82045410e089c60
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908071"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="50ba9-103">Atualizar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="50ba9-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="50ba9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50ba9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50ba9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50ba9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50ba9-106">Atualiza as propriedades de um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="50ba9-106">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50ba9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50ba9-107">Prerequisites</span></span>
<span data-ttu-id="50ba9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50ba9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50ba9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50ba9-110">Permission type</span></span>|<span data-ttu-id="50ba9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50ba9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50ba9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50ba9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50ba9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50ba9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="50ba9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50ba9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50ba9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50ba9-115">Not supported.</span></span>|
|<span data-ttu-id="50ba9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50ba9-116">Application</span></span>|<span data-ttu-id="50ba9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50ba9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50ba9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50ba9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="50ba9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50ba9-119">Request headers</span></span>
|<span data-ttu-id="50ba9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50ba9-120">Header</span></span>|<span data-ttu-id="50ba9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="50ba9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50ba9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="50ba9-122">Authorization</span></span>|<span data-ttu-id="50ba9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50ba9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50ba9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50ba9-124">Accept</span></span>|<span data-ttu-id="50ba9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50ba9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50ba9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50ba9-126">Request body</span></span>
<span data-ttu-id="50ba9-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="50ba9-127">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="50ba9-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="50ba9-128">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="50ba9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50ba9-129">Property</span></span>|<span data-ttu-id="50ba9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="50ba9-130">Type</span></span>|<span data-ttu-id="50ba9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="50ba9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50ba9-132">id</span><span class="sxs-lookup"><span data-stu-id="50ba9-132">id</span></span>|<span data-ttu-id="50ba9-133">String</span><span class="sxs-lookup"><span data-stu-id="50ba9-133">String</span></span>|<span data-ttu-id="50ba9-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="50ba9-134">The GUID for the object</span></span>|
|<span data-ttu-id="50ba9-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="50ba9-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="50ba9-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="50ba9-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="50ba9-137">Status de atribuição de perfil do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="50ba9-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="50ba9-138">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="50ba9-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="50ba9-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="50ba9-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="50ba9-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="50ba9-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="50ba9-141">Atribuição de perfil status detalhado do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="50ba9-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="50ba9-142">Os valores possíveis são: `none` e `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="50ba9-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="50ba9-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="50ba9-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="50ba9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50ba9-144">DateTimeOffset</span></span>|<span data-ttu-id="50ba9-145">Hora do conjunto de perfis do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="50ba9-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="50ba9-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="50ba9-146">orderIdentifier</span></span>|<span data-ttu-id="50ba9-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-147">String</span></span>|<span data-ttu-id="50ba9-148">Identificador de pedidos do dispositivo do Windows AutoPilot-preterido</span><span class="sxs-lookup"><span data-stu-id="50ba9-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="50ba9-149">groupTag</span><span class="sxs-lookup"><span data-stu-id="50ba9-149">groupTag</span></span>|<span data-ttu-id="50ba9-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-150">String</span></span>|<span data-ttu-id="50ba9-151">Marca de grupo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="50ba9-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="50ba9-152">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="50ba9-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="50ba9-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-153">String</span></span>|<span data-ttu-id="50ba9-154">Identificador de ordem de compra do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="50ba9-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="50ba9-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="50ba9-155">serialNumber</span></span>|<span data-ttu-id="50ba9-156">String</span><span class="sxs-lookup"><span data-stu-id="50ba9-156">String</span></span>|<span data-ttu-id="50ba9-157">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="50ba9-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="50ba9-158">productKey</span><span class="sxs-lookup"><span data-stu-id="50ba9-158">productKey</span></span>|<span data-ttu-id="50ba9-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-159">String</span></span>|<span data-ttu-id="50ba9-160">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="50ba9-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="50ba9-161">fabricante</span><span class="sxs-lookup"><span data-stu-id="50ba9-161">manufacturer</span></span>|<span data-ttu-id="50ba9-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-162">String</span></span>|<span data-ttu-id="50ba9-163">Fabricante OEM do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="50ba9-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="50ba9-164">modelo</span><span class="sxs-lookup"><span data-stu-id="50ba9-164">model</span></span>|<span data-ttu-id="50ba9-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-165">String</span></span>|<span data-ttu-id="50ba9-166">Nome do modelo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="50ba9-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="50ba9-167">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="50ba9-167">enrollmentState</span></span>|[<span data-ttu-id="50ba9-168">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="50ba9-168">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="50ba9-169">Estado de registro do Intune do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="50ba9-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="50ba9-170">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="50ba9-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="50ba9-171">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="50ba9-171">lastContactedDateTime</span></span>|<span data-ttu-id="50ba9-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50ba9-172">DateTimeOffset</span></span>|<span data-ttu-id="50ba9-173">Data e hora do último contato do Intune para o dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="50ba9-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="50ba9-174">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="50ba9-174">addressableUserName</span></span>|<span data-ttu-id="50ba9-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-175">String</span></span>|<span data-ttu-id="50ba9-176">Nome de usuário endereçável.</span><span class="sxs-lookup"><span data-stu-id="50ba9-176">Addressable user name.</span></span>|
|<span data-ttu-id="50ba9-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="50ba9-177">userPrincipalName</span></span>|<span data-ttu-id="50ba9-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-178">String</span></span>|<span data-ttu-id="50ba9-179">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="50ba9-179">User Principal Name.</span></span>|
|<span data-ttu-id="50ba9-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="50ba9-180">resourceName</span></span>|<span data-ttu-id="50ba9-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-181">String</span></span>|<span data-ttu-id="50ba9-182">Nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="50ba9-182">Resource Name.</span></span>|
|<span data-ttu-id="50ba9-183">skuNumber</span><span class="sxs-lookup"><span data-stu-id="50ba9-183">skuNumber</span></span>|<span data-ttu-id="50ba9-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-184">String</span></span>|<span data-ttu-id="50ba9-185">Número de SKU</span><span class="sxs-lookup"><span data-stu-id="50ba9-185">SKU Number</span></span>|
|<span data-ttu-id="50ba9-186">systemFamily</span><span class="sxs-lookup"><span data-stu-id="50ba9-186">systemFamily</span></span>|<span data-ttu-id="50ba9-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-187">String</span></span>|<span data-ttu-id="50ba9-188">Família de sistema</span><span class="sxs-lookup"><span data-stu-id="50ba9-188">System Family</span></span>|
|<span data-ttu-id="50ba9-189">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="50ba9-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="50ba9-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-190">String</span></span>|<span data-ttu-id="50ba9-191">ID de dispositivo do AAD</span><span class="sxs-lookup"><span data-stu-id="50ba9-191">AAD Device ID</span></span>|
|<span data-ttu-id="50ba9-192">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="50ba9-192">managedDeviceId</span></span>|<span data-ttu-id="50ba9-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ba9-193">String</span></span>|<span data-ttu-id="50ba9-194">ID do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="50ba9-194">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="50ba9-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="50ba9-195">Response</span></span>
<span data-ttu-id="50ba9-196">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50ba9-196">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50ba9-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50ba9-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="50ba9-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50ba9-198">Request</span></span>
<span data-ttu-id="50ba9-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50ba9-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 1035

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="50ba9-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="50ba9-200">Response</span></span>
<span data-ttu-id="50ba9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50ba9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1084

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value"
}
```




