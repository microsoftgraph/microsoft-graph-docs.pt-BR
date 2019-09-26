---
title: Atualizar windowsAutopilotDeviceIdentity
description: Atualiza as propriedades de um objeto windowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ce444f603db5bb33dcda1a1ce0d02d6bf9fa716b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187632"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="1f875-103">Atualizar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="1f875-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="1f875-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1f875-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f875-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f875-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f875-106">Atualiza as propriedades de um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="1f875-106">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f875-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1f875-107">Prerequisites</span></span>
<span data-ttu-id="1f875-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f875-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f875-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f875-110">Permission type</span></span>|<span data-ttu-id="1f875-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1f875-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f875-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f875-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f875-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f875-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1f875-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f875-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f875-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f875-115">Not supported.</span></span>|
|<span data-ttu-id="1f875-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f875-116">Application</span></span>|<span data-ttu-id="1f875-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f875-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f875-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f875-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="1f875-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f875-119">Request headers</span></span>
|<span data-ttu-id="1f875-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f875-120">Header</span></span>|<span data-ttu-id="1f875-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1f875-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f875-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f875-122">Authorization</span></span>|<span data-ttu-id="1f875-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f875-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f875-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1f875-124">Accept</span></span>|<span data-ttu-id="1f875-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f875-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f875-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f875-126">Request body</span></span>
<span data-ttu-id="1f875-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="1f875-127">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="1f875-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="1f875-128">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="1f875-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f875-129">Property</span></span>|<span data-ttu-id="1f875-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f875-130">Type</span></span>|<span data-ttu-id="1f875-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f875-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f875-132">id</span><span class="sxs-lookup"><span data-stu-id="1f875-132">id</span></span>|<span data-ttu-id="1f875-133">String</span><span class="sxs-lookup"><span data-stu-id="1f875-133">String</span></span>|<span data-ttu-id="1f875-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="1f875-134">The GUID for the object</span></span>|
|<span data-ttu-id="1f875-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="1f875-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="1f875-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="1f875-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="1f875-137">Status de atribuição de perfil do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="1f875-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="1f875-138">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="1f875-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="1f875-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="1f875-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="1f875-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="1f875-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="1f875-141">Atribuição de perfil status detalhado do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="1f875-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="1f875-142">Os valores possíveis são: `none` e `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="1f875-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="1f875-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f875-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="1f875-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f875-144">DateTimeOffset</span></span>|<span data-ttu-id="1f875-145">Hora do conjunto de perfis do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="1f875-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f875-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="1f875-146">orderIdentifier</span></span>|<span data-ttu-id="1f875-147">String</span><span class="sxs-lookup"><span data-stu-id="1f875-147">String</span></span>|<span data-ttu-id="1f875-148">Identificador de pedidos do dispositivo do Windows AutoPilot-preterido</span><span class="sxs-lookup"><span data-stu-id="1f875-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="1f875-149">groupTag</span><span class="sxs-lookup"><span data-stu-id="1f875-149">groupTag</span></span>|<span data-ttu-id="1f875-150">String</span><span class="sxs-lookup"><span data-stu-id="1f875-150">String</span></span>|<span data-ttu-id="1f875-151">Marca de grupo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="1f875-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f875-152">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="1f875-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="1f875-153">String</span><span class="sxs-lookup"><span data-stu-id="1f875-153">String</span></span>|<span data-ttu-id="1f875-154">Identificador de ordem de compra do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="1f875-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f875-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1f875-155">serialNumber</span></span>|<span data-ttu-id="1f875-156">String</span><span class="sxs-lookup"><span data-stu-id="1f875-156">String</span></span>|<span data-ttu-id="1f875-157">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="1f875-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f875-158">productKey</span><span class="sxs-lookup"><span data-stu-id="1f875-158">productKey</span></span>|<span data-ttu-id="1f875-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f875-159">String</span></span>|<span data-ttu-id="1f875-160">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="1f875-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f875-161">fabricante</span><span class="sxs-lookup"><span data-stu-id="1f875-161">manufacturer</span></span>|<span data-ttu-id="1f875-162">String</span><span class="sxs-lookup"><span data-stu-id="1f875-162">String</span></span>|<span data-ttu-id="1f875-163">Fabricante OEM do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="1f875-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f875-164">modelo</span><span class="sxs-lookup"><span data-stu-id="1f875-164">model</span></span>|<span data-ttu-id="1f875-165">String</span><span class="sxs-lookup"><span data-stu-id="1f875-165">String</span></span>|<span data-ttu-id="1f875-166">Nome do modelo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="1f875-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f875-167">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="1f875-167">enrollmentState</span></span>|[<span data-ttu-id="1f875-168">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="1f875-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="1f875-169">Estado de registro do Intune do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="1f875-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="1f875-170">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="1f875-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="1f875-171">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f875-171">lastContactedDateTime</span></span>|<span data-ttu-id="1f875-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f875-172">DateTimeOffset</span></span>|<span data-ttu-id="1f875-173">Data e hora do último contato do Intune para o dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="1f875-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f875-174">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="1f875-174">addressableUserName</span></span>|<span data-ttu-id="1f875-175">String</span><span class="sxs-lookup"><span data-stu-id="1f875-175">String</span></span>|<span data-ttu-id="1f875-176">Nome de usuário endereçável.</span><span class="sxs-lookup"><span data-stu-id="1f875-176">Addressable user name.</span></span>|
|<span data-ttu-id="1f875-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1f875-177">userPrincipalName</span></span>|<span data-ttu-id="1f875-178">String</span><span class="sxs-lookup"><span data-stu-id="1f875-178">String</span></span>|<span data-ttu-id="1f875-179">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="1f875-179">User Principal Name.</span></span>|
|<span data-ttu-id="1f875-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="1f875-180">resourceName</span></span>|<span data-ttu-id="1f875-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f875-181">String</span></span>|<span data-ttu-id="1f875-182">Nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f875-182">Resource Name.</span></span>|
|<span data-ttu-id="1f875-183">skuNumber</span><span class="sxs-lookup"><span data-stu-id="1f875-183">skuNumber</span></span>|<span data-ttu-id="1f875-184">String</span><span class="sxs-lookup"><span data-stu-id="1f875-184">String</span></span>|<span data-ttu-id="1f875-185">Número de SKU</span><span class="sxs-lookup"><span data-stu-id="1f875-185">SKU Number</span></span>|
|<span data-ttu-id="1f875-186">systemFamily</span><span class="sxs-lookup"><span data-stu-id="1f875-186">systemFamily</span></span>|<span data-ttu-id="1f875-187">String</span><span class="sxs-lookup"><span data-stu-id="1f875-187">String</span></span>|<span data-ttu-id="1f875-188">Família de sistema</span><span class="sxs-lookup"><span data-stu-id="1f875-188">System Family</span></span>|
|<span data-ttu-id="1f875-189">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="1f875-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="1f875-190">String</span><span class="sxs-lookup"><span data-stu-id="1f875-190">String</span></span>|<span data-ttu-id="1f875-191">ID de dispositivo do AAD</span><span class="sxs-lookup"><span data-stu-id="1f875-191">AAD Device ID</span></span>|
|<span data-ttu-id="1f875-192">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="1f875-192">managedDeviceId</span></span>|<span data-ttu-id="1f875-193">String</span><span class="sxs-lookup"><span data-stu-id="1f875-193">String</span></span>|<span data-ttu-id="1f875-194">ID do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="1f875-194">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="1f875-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f875-195">Response</span></span>
<span data-ttu-id="1f875-196">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f875-196">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f875-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f875-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f875-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f875-198">Request</span></span>
<span data-ttu-id="1f875-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f875-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f875-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f875-200">Response</span></span>
<span data-ttu-id="1f875-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f875-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




