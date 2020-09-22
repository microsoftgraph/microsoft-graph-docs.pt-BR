---
title: Criar windowsAutopilotDeviceIdentity
description: Criar um novo objeto windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b10e378fa294d35d343487b96fa4627aba50ae8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062649"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="93823-103">Criar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="93823-103">Create windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="93823-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93823-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93823-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93823-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93823-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93823-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93823-107">Criar um novo objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="93823-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93823-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93823-108">Prerequisites</span></span>
<span data-ttu-id="93823-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93823-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93823-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93823-111">Permission type</span></span>|<span data-ttu-id="93823-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="93823-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93823-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93823-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93823-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93823-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="93823-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93823-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93823-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93823-116">Not supported.</span></span>|
|<span data-ttu-id="93823-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93823-117">Application</span></span>|<span data-ttu-id="93823-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93823-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93823-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93823-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="93823-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93823-120">Request headers</span></span>
|<span data-ttu-id="93823-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93823-121">Header</span></span>|<span data-ttu-id="93823-122">Valor</span><span class="sxs-lookup"><span data-stu-id="93823-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93823-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="93823-123">Authorization</span></span>|<span data-ttu-id="93823-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93823-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93823-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="93823-125">Accept</span></span>|<span data-ttu-id="93823-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93823-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93823-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93823-127">Request body</span></span>
<span data-ttu-id="93823-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="93823-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="93823-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="93823-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="93823-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93823-130">Property</span></span>|<span data-ttu-id="93823-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="93823-131">Type</span></span>|<span data-ttu-id="93823-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="93823-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93823-133">id</span><span class="sxs-lookup"><span data-stu-id="93823-133">id</span></span>|<span data-ttu-id="93823-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-134">String</span></span>|<span data-ttu-id="93823-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="93823-135">The GUID for the object</span></span>|
|<span data-ttu-id="93823-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="93823-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="93823-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="93823-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="93823-138">Status de atribuição de perfil do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="93823-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="93823-139">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="93823-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="93823-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="93823-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="93823-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="93823-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="93823-142">Atribuição de perfil status detalhado do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="93823-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="93823-143">Os valores possíveis são: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span><span class="sxs-lookup"><span data-stu-id="93823-143">Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span></span>|
|<span data-ttu-id="93823-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="93823-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="93823-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93823-145">DateTimeOffset</span></span>|<span data-ttu-id="93823-146">Hora do conjunto de perfis do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="93823-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93823-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="93823-147">orderIdentifier</span></span>|<span data-ttu-id="93823-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-148">String</span></span>|<span data-ttu-id="93823-149">Identificador de pedidos do dispositivo do Windows AutoPilot-preterido</span><span class="sxs-lookup"><span data-stu-id="93823-149">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="93823-150">groupTag</span><span class="sxs-lookup"><span data-stu-id="93823-150">groupTag</span></span>|<span data-ttu-id="93823-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-151">String</span></span>|<span data-ttu-id="93823-152">Marca de grupo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="93823-152">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93823-153">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="93823-153">purchaseOrderIdentifier</span></span>|<span data-ttu-id="93823-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-154">String</span></span>|<span data-ttu-id="93823-155">Identificador de ordem de compra do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="93823-155">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93823-156">serialNumber</span><span class="sxs-lookup"><span data-stu-id="93823-156">serialNumber</span></span>|<span data-ttu-id="93823-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-157">String</span></span>|<span data-ttu-id="93823-158">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="93823-158">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93823-159">productKey</span><span class="sxs-lookup"><span data-stu-id="93823-159">productKey</span></span>|<span data-ttu-id="93823-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-160">String</span></span>|<span data-ttu-id="93823-161">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="93823-161">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93823-162">fabricante</span><span class="sxs-lookup"><span data-stu-id="93823-162">manufacturer</span></span>|<span data-ttu-id="93823-163">String</span><span class="sxs-lookup"><span data-stu-id="93823-163">String</span></span>|<span data-ttu-id="93823-164">Fabricante OEM do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="93823-164">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93823-165">modelo</span><span class="sxs-lookup"><span data-stu-id="93823-165">model</span></span>|<span data-ttu-id="93823-166">String</span><span class="sxs-lookup"><span data-stu-id="93823-166">String</span></span>|<span data-ttu-id="93823-167">Nome do modelo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="93823-167">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93823-168">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="93823-168">enrollmentState</span></span>|[<span data-ttu-id="93823-169">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="93823-169">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="93823-170">Estado de registro do Intune do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="93823-170">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="93823-171">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="93823-171">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="93823-172">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="93823-172">lastContactedDateTime</span></span>|<span data-ttu-id="93823-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93823-173">DateTimeOffset</span></span>|<span data-ttu-id="93823-174">Data e hora do último contato do Intune para o dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="93823-174">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93823-175">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="93823-175">addressableUserName</span></span>|<span data-ttu-id="93823-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-176">String</span></span>|<span data-ttu-id="93823-177">Nome de usuário endereçável.</span><span class="sxs-lookup"><span data-stu-id="93823-177">Addressable user name.</span></span>|
|<span data-ttu-id="93823-178">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="93823-178">userPrincipalName</span></span>|<span data-ttu-id="93823-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-179">String</span></span>|<span data-ttu-id="93823-180">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="93823-180">User Principal Name.</span></span>|
|<span data-ttu-id="93823-181">resourceName</span><span class="sxs-lookup"><span data-stu-id="93823-181">resourceName</span></span>|<span data-ttu-id="93823-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-182">String</span></span>|<span data-ttu-id="93823-183">Nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="93823-183">Resource Name.</span></span>|
|<span data-ttu-id="93823-184">skuNumber</span><span class="sxs-lookup"><span data-stu-id="93823-184">skuNumber</span></span>|<span data-ttu-id="93823-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-185">String</span></span>|<span data-ttu-id="93823-186">Número de SKU</span><span class="sxs-lookup"><span data-stu-id="93823-186">SKU Number</span></span>|
|<span data-ttu-id="93823-187">systemFamily</span><span class="sxs-lookup"><span data-stu-id="93823-187">systemFamily</span></span>|<span data-ttu-id="93823-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-188">String</span></span>|<span data-ttu-id="93823-189">Família de sistema</span><span class="sxs-lookup"><span data-stu-id="93823-189">System Family</span></span>|
|<span data-ttu-id="93823-190">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="93823-190">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="93823-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-191">String</span></span>|<span data-ttu-id="93823-192">ID de dispositivo do AAD</span><span class="sxs-lookup"><span data-stu-id="93823-192">AAD Device ID</span></span>|
|<span data-ttu-id="93823-193">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="93823-193">managedDeviceId</span></span>|<span data-ttu-id="93823-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-194">String</span></span>|<span data-ttu-id="93823-195">ID do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="93823-195">Managed Device ID</span></span>|
|<span data-ttu-id="93823-196">displayName</span><span class="sxs-lookup"><span data-stu-id="93823-196">displayName</span></span>|<span data-ttu-id="93823-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93823-197">String</span></span>|<span data-ttu-id="93823-198">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="93823-198">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="93823-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="93823-199">Response</span></span>
<span data-ttu-id="93823-200">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93823-200">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93823-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93823-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="93823-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93823-202">Request</span></span>
<span data-ttu-id="93823-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93823-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="93823-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="93823-204">Response</span></span>
<span data-ttu-id="93823-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93823-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






