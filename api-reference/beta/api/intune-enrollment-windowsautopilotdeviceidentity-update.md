---
title: Atualizar windowsAutopilotDeviceIdentity
description: Atualiza as propriedades de um objeto windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ed1e8159b91aed11cc631e26aa02d79dbb4cce4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532510"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="eda54-103">Atualizar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eda54-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="eda54-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eda54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eda54-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eda54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eda54-106">Atualiza as propriedades de um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="eda54-106">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eda54-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eda54-107">Prerequisites</span></span>
<span data-ttu-id="eda54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eda54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eda54-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eda54-110">Permission type</span></span>|<span data-ttu-id="eda54-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eda54-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eda54-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eda54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eda54-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eda54-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eda54-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eda54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eda54-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eda54-115">Not supported.</span></span>|
|<span data-ttu-id="eda54-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eda54-116">Application</span></span>|<span data-ttu-id="eda54-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eda54-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eda54-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eda54-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="eda54-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eda54-119">Request headers</span></span>
|<span data-ttu-id="eda54-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eda54-120">Header</span></span>|<span data-ttu-id="eda54-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eda54-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eda54-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eda54-122">Authorization</span></span>|<span data-ttu-id="eda54-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eda54-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eda54-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eda54-124">Accept</span></span>|<span data-ttu-id="eda54-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eda54-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eda54-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eda54-126">Request body</span></span>
<span data-ttu-id="eda54-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="eda54-127">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="eda54-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="eda54-128">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="eda54-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eda54-129">Property</span></span>|<span data-ttu-id="eda54-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eda54-130">Type</span></span>|<span data-ttu-id="eda54-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eda54-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eda54-132">id</span><span class="sxs-lookup"><span data-stu-id="eda54-132">id</span></span>|<span data-ttu-id="eda54-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eda54-133">String</span></span>|<span data-ttu-id="eda54-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="eda54-134">The GUID for the object</span></span>|
|<span data-ttu-id="eda54-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="eda54-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="eda54-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="eda54-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="eda54-137">Status de atribuição de perfil do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="eda54-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="eda54-138">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="eda54-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="eda54-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="eda54-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="eda54-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="eda54-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="eda54-141">Atribuição de perfil status detalhado do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="eda54-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="eda54-142">Os valores possíveis são: `none` e `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="eda54-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="eda54-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="eda54-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="eda54-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eda54-144">DateTimeOffset</span></span>|<span data-ttu-id="eda54-145">Hora do conjunto de perfis do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="eda54-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="eda54-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="eda54-146">orderIdentifier</span></span>|<span data-ttu-id="eda54-147">String</span><span class="sxs-lookup"><span data-stu-id="eda54-147">String</span></span>|<span data-ttu-id="eda54-148">Identificador de pedidos do dispositivo do Windows AutoPilot-preTerido</span><span class="sxs-lookup"><span data-stu-id="eda54-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="eda54-149">groupTag</span><span class="sxs-lookup"><span data-stu-id="eda54-149">groupTag</span></span>|<span data-ttu-id="eda54-150">String</span><span class="sxs-lookup"><span data-stu-id="eda54-150">String</span></span>|<span data-ttu-id="eda54-151">Marca de grupo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="eda54-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="eda54-152">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="eda54-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="eda54-153">String</span><span class="sxs-lookup"><span data-stu-id="eda54-153">String</span></span>|<span data-ttu-id="eda54-154">Identificador de ordem de compra do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="eda54-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="eda54-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="eda54-155">serialNumber</span></span>|<span data-ttu-id="eda54-156">String</span><span class="sxs-lookup"><span data-stu-id="eda54-156">String</span></span>|<span data-ttu-id="eda54-157">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="eda54-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="eda54-158">productKey</span><span class="sxs-lookup"><span data-stu-id="eda54-158">productKey</span></span>|<span data-ttu-id="eda54-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eda54-159">String</span></span>|<span data-ttu-id="eda54-160">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="eda54-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="eda54-161">fabricante</span><span class="sxs-lookup"><span data-stu-id="eda54-161">manufacturer</span></span>|<span data-ttu-id="eda54-162">String</span><span class="sxs-lookup"><span data-stu-id="eda54-162">String</span></span>|<span data-ttu-id="eda54-163">Fabricante OEM do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="eda54-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="eda54-164">modelo</span><span class="sxs-lookup"><span data-stu-id="eda54-164">model</span></span>|<span data-ttu-id="eda54-165">String</span><span class="sxs-lookup"><span data-stu-id="eda54-165">String</span></span>|<span data-ttu-id="eda54-166">Nome do modelo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="eda54-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="eda54-167">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="eda54-167">enrollmentState</span></span>|[<span data-ttu-id="eda54-168">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="eda54-168">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="eda54-169">Estado de registro do Intune do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="eda54-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="eda54-170">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="eda54-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="eda54-171">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="eda54-171">lastContactedDateTime</span></span>|<span data-ttu-id="eda54-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eda54-172">DateTimeOffset</span></span>|<span data-ttu-id="eda54-173">Data e hora do último contato do Intune para o dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="eda54-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="eda54-174">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="eda54-174">addressableUserName</span></span>|<span data-ttu-id="eda54-175">String</span><span class="sxs-lookup"><span data-stu-id="eda54-175">String</span></span>|<span data-ttu-id="eda54-176">Nome de usuário endereçável.</span><span class="sxs-lookup"><span data-stu-id="eda54-176">Addressable user name.</span></span>|
|<span data-ttu-id="eda54-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eda54-177">userPrincipalName</span></span>|<span data-ttu-id="eda54-178">String</span><span class="sxs-lookup"><span data-stu-id="eda54-178">String</span></span>|<span data-ttu-id="eda54-179">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="eda54-179">User Principal Name.</span></span>|
|<span data-ttu-id="eda54-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="eda54-180">resourceName</span></span>|<span data-ttu-id="eda54-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eda54-181">String</span></span>|<span data-ttu-id="eda54-182">Nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="eda54-182">Resource Name.</span></span>|
|<span data-ttu-id="eda54-183">skuNumber</span><span class="sxs-lookup"><span data-stu-id="eda54-183">skuNumber</span></span>|<span data-ttu-id="eda54-184">String</span><span class="sxs-lookup"><span data-stu-id="eda54-184">String</span></span>|<span data-ttu-id="eda54-185">Número de SKU</span><span class="sxs-lookup"><span data-stu-id="eda54-185">SKU Number</span></span>|
|<span data-ttu-id="eda54-186">systemFamily</span><span class="sxs-lookup"><span data-stu-id="eda54-186">systemFamily</span></span>|<span data-ttu-id="eda54-187">String</span><span class="sxs-lookup"><span data-stu-id="eda54-187">String</span></span>|<span data-ttu-id="eda54-188">Família de sistema</span><span class="sxs-lookup"><span data-stu-id="eda54-188">System Family</span></span>|
|<span data-ttu-id="eda54-189">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="eda54-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="eda54-190">String</span><span class="sxs-lookup"><span data-stu-id="eda54-190">String</span></span>|<span data-ttu-id="eda54-191">ID de dispositivo do AAD</span><span class="sxs-lookup"><span data-stu-id="eda54-191">AAD Device ID</span></span>|
|<span data-ttu-id="eda54-192">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="eda54-192">managedDeviceId</span></span>|<span data-ttu-id="eda54-193">String</span><span class="sxs-lookup"><span data-stu-id="eda54-193">String</span></span>|<span data-ttu-id="eda54-194">ID do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="eda54-194">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="eda54-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="eda54-195">Response</span></span>
<span data-ttu-id="eda54-196">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eda54-196">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eda54-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eda54-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="eda54-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eda54-198">Request</span></span>
<span data-ttu-id="eda54-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eda54-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eda54-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="eda54-200">Response</span></span>
<span data-ttu-id="eda54-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eda54-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





