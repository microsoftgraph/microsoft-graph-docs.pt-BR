---
title: Criar windowsAutopilotDeviceIdentity
description: Criar um novo objeto windowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0761094989125a9b5026fa4529eb3d5eb7f703b5
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160015"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="26189-103">Criar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="26189-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="26189-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26189-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26189-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26189-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26189-106">Criar um novo objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="26189-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26189-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26189-107">Prerequisites</span></span>
<span data-ttu-id="26189-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26189-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26189-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26189-110">Permission type</span></span>|<span data-ttu-id="26189-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26189-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26189-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26189-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26189-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26189-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="26189-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26189-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26189-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26189-115">Not supported.</span></span>|
|<span data-ttu-id="26189-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26189-116">Application</span></span>|<span data-ttu-id="26189-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26189-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26189-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26189-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="26189-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26189-119">Request headers</span></span>
|<span data-ttu-id="26189-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26189-120">Header</span></span>|<span data-ttu-id="26189-121">Valor</span><span class="sxs-lookup"><span data-stu-id="26189-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26189-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26189-122">Authorization</span></span>|<span data-ttu-id="26189-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26189-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26189-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26189-124">Accept</span></span>|<span data-ttu-id="26189-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26189-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26189-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26189-126">Request body</span></span>
<span data-ttu-id="26189-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="26189-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="26189-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="26189-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="26189-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26189-129">Property</span></span>|<span data-ttu-id="26189-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="26189-130">Type</span></span>|<span data-ttu-id="26189-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="26189-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26189-132">id</span><span class="sxs-lookup"><span data-stu-id="26189-132">id</span></span>|<span data-ttu-id="26189-133">String</span><span class="sxs-lookup"><span data-stu-id="26189-133">String</span></span>|<span data-ttu-id="26189-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="26189-134">The GUID for the object</span></span>|
|<span data-ttu-id="26189-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="26189-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="26189-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="26189-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="26189-137">Status de atribuição de perfil do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="26189-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="26189-138">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="26189-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="26189-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="26189-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="26189-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="26189-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="26189-141">Atribuição de perfil status detalhado do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="26189-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="26189-142">Os valores possíveis são: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span><span class="sxs-lookup"><span data-stu-id="26189-142">Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span></span>|
|<span data-ttu-id="26189-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="26189-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="26189-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26189-144">DateTimeOffset</span></span>|<span data-ttu-id="26189-145">Hora do conjunto de perfis do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="26189-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="26189-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="26189-146">orderIdentifier</span></span>|<span data-ttu-id="26189-147">String</span><span class="sxs-lookup"><span data-stu-id="26189-147">String</span></span>|<span data-ttu-id="26189-148">Identificador de pedidos do dispositivo do Windows AutoPilot-preterido</span><span class="sxs-lookup"><span data-stu-id="26189-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="26189-149">groupTag</span><span class="sxs-lookup"><span data-stu-id="26189-149">groupTag</span></span>|<span data-ttu-id="26189-150">String</span><span class="sxs-lookup"><span data-stu-id="26189-150">String</span></span>|<span data-ttu-id="26189-151">Marca de grupo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="26189-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="26189-152">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="26189-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="26189-153">String</span><span class="sxs-lookup"><span data-stu-id="26189-153">String</span></span>|<span data-ttu-id="26189-154">Identificador de ordem de compra do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="26189-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="26189-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="26189-155">serialNumber</span></span>|<span data-ttu-id="26189-156">String</span><span class="sxs-lookup"><span data-stu-id="26189-156">String</span></span>|<span data-ttu-id="26189-157">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="26189-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="26189-158">productKey</span><span class="sxs-lookup"><span data-stu-id="26189-158">productKey</span></span>|<span data-ttu-id="26189-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26189-159">String</span></span>|<span data-ttu-id="26189-160">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="26189-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="26189-161">fabricante</span><span class="sxs-lookup"><span data-stu-id="26189-161">manufacturer</span></span>|<span data-ttu-id="26189-162">String</span><span class="sxs-lookup"><span data-stu-id="26189-162">String</span></span>|<span data-ttu-id="26189-163">Fabricante OEM do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="26189-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="26189-164">modelo</span><span class="sxs-lookup"><span data-stu-id="26189-164">model</span></span>|<span data-ttu-id="26189-165">String</span><span class="sxs-lookup"><span data-stu-id="26189-165">String</span></span>|<span data-ttu-id="26189-166">Nome do modelo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="26189-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="26189-167">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="26189-167">enrollmentState</span></span>|[<span data-ttu-id="26189-168">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="26189-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="26189-169">Estado de registro do Intune do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="26189-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="26189-170">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="26189-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="26189-171">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="26189-171">lastContactedDateTime</span></span>|<span data-ttu-id="26189-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26189-172">DateTimeOffset</span></span>|<span data-ttu-id="26189-173">Data e hora do último contato do Intune para o dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="26189-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="26189-174">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="26189-174">addressableUserName</span></span>|<span data-ttu-id="26189-175">String</span><span class="sxs-lookup"><span data-stu-id="26189-175">String</span></span>|<span data-ttu-id="26189-176">Nome de usuário endereçável.</span><span class="sxs-lookup"><span data-stu-id="26189-176">Addressable user name.</span></span>|
|<span data-ttu-id="26189-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="26189-177">userPrincipalName</span></span>|<span data-ttu-id="26189-178">String</span><span class="sxs-lookup"><span data-stu-id="26189-178">String</span></span>|<span data-ttu-id="26189-179">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="26189-179">User Principal Name.</span></span>|
|<span data-ttu-id="26189-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="26189-180">resourceName</span></span>|<span data-ttu-id="26189-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26189-181">String</span></span>|<span data-ttu-id="26189-182">Nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="26189-182">Resource Name.</span></span>|
|<span data-ttu-id="26189-183">skuNumber</span><span class="sxs-lookup"><span data-stu-id="26189-183">skuNumber</span></span>|<span data-ttu-id="26189-184">String</span><span class="sxs-lookup"><span data-stu-id="26189-184">String</span></span>|<span data-ttu-id="26189-185">Número de SKU</span><span class="sxs-lookup"><span data-stu-id="26189-185">SKU Number</span></span>|
|<span data-ttu-id="26189-186">systemFamily</span><span class="sxs-lookup"><span data-stu-id="26189-186">systemFamily</span></span>|<span data-ttu-id="26189-187">String</span><span class="sxs-lookup"><span data-stu-id="26189-187">String</span></span>|<span data-ttu-id="26189-188">Família de sistema</span><span class="sxs-lookup"><span data-stu-id="26189-188">System Family</span></span>|
|<span data-ttu-id="26189-189">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="26189-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="26189-190">String</span><span class="sxs-lookup"><span data-stu-id="26189-190">String</span></span>|<span data-ttu-id="26189-191">ID de dispositivo do AAD</span><span class="sxs-lookup"><span data-stu-id="26189-191">AAD Device ID</span></span>|
|<span data-ttu-id="26189-192">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="26189-192">managedDeviceId</span></span>|<span data-ttu-id="26189-193">String</span><span class="sxs-lookup"><span data-stu-id="26189-193">String</span></span>|<span data-ttu-id="26189-194">ID do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="26189-194">Managed Device ID</span></span>|
|<span data-ttu-id="26189-195">displayName</span><span class="sxs-lookup"><span data-stu-id="26189-195">displayName</span></span>|<span data-ttu-id="26189-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26189-196">String</span></span>|<span data-ttu-id="26189-197">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="26189-197">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="26189-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="26189-198">Response</span></span>
<span data-ttu-id="26189-199">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26189-199">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26189-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26189-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="26189-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26189-201">Request</span></span>
<span data-ttu-id="26189-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26189-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 1075

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
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="26189-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="26189-203">Response</span></span>
<span data-ttu-id="26189-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26189-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1124

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
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```





