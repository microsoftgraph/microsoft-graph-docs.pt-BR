---
title: Criar windowsAutopilotDeviceIdentity
description: Criar um novo objeto windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b29da1f5a9552aa14e51d9ef88c52b143144885c
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571505"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="5ee1d-103">Criar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5ee1d-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="5ee1d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ee1d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ee1d-106">Criar um novo objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="5ee1d-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ee1d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ee1d-107">Prerequisites</span></span>
<span data-ttu-id="5ee1d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5ee1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5ee1d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ee1d-110">Permission type</span></span>|<span data-ttu-id="5ee1d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ee1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ee1d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ee1d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ee1d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee1d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5ee1d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ee1d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ee1d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-115">Not supported.</span></span>|
|<span data-ttu-id="5ee1d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ee1d-116">Application</span></span>|<span data-ttu-id="5ee1d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ee1d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee1d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="5ee1d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee1d-119">Request headers</span></span>
|<span data-ttu-id="5ee1d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ee1d-120">Header</span></span>|<span data-ttu-id="5ee1d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5ee1d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ee1d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ee1d-122">Authorization</span></span>|<span data-ttu-id="5ee1d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ee1d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ee1d-124">Accept</span></span>|<span data-ttu-id="5ee1d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ee1d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ee1d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee1d-126">Request body</span></span>
<span data-ttu-id="5ee1d-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="5ee1d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="5ee1d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ee1d-129">Property</span></span>|<span data-ttu-id="5ee1d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ee1d-130">Type</span></span>|<span data-ttu-id="5ee1d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ee1d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ee1d-132">id</span><span class="sxs-lookup"><span data-stu-id="5ee1d-132">id</span></span>|<span data-ttu-id="5ee1d-133">String</span><span class="sxs-lookup"><span data-stu-id="5ee1d-133">String</span></span>|<span data-ttu-id="5ee1d-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-134">The GUID for the object</span></span>|
|<span data-ttu-id="5ee1d-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="5ee1d-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="5ee1d-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="5ee1d-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="5ee1d-137">Status de atribuição de perfil do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="5ee1d-138">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="5ee1d-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="5ee1d-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="5ee1d-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="5ee1d-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="5ee1d-141">Atribuição de perfil status detalhado do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="5ee1d-142">Os valores possíveis são: `none` e `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="5ee1d-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee1d-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="5ee1d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee1d-144">DateTimeOffset</span></span>|<span data-ttu-id="5ee1d-145">Hora do conjunto de perfis do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5ee1d-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="5ee1d-146">orderIdentifier</span></span>|<span data-ttu-id="5ee1d-147">String</span><span class="sxs-lookup"><span data-stu-id="5ee1d-147">String</span></span>|<span data-ttu-id="5ee1d-148">Identificador de pedidos do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-148">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5ee1d-149">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="5ee1d-149">purchaseOrderIdentifier</span></span>|<span data-ttu-id="5ee1d-150">String</span><span class="sxs-lookup"><span data-stu-id="5ee1d-150">String</span></span>|<span data-ttu-id="5ee1d-151">Identificador de ordem de compra do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-151">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5ee1d-152">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5ee1d-152">serialNumber</span></span>|<span data-ttu-id="5ee1d-153">String</span><span class="sxs-lookup"><span data-stu-id="5ee1d-153">String</span></span>|<span data-ttu-id="5ee1d-154">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-154">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5ee1d-155">productKey</span><span class="sxs-lookup"><span data-stu-id="5ee1d-155">productKey</span></span>|<span data-ttu-id="5ee1d-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ee1d-156">String</span></span>|<span data-ttu-id="5ee1d-157">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-157">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5ee1d-158">fabricante</span><span class="sxs-lookup"><span data-stu-id="5ee1d-158">manufacturer</span></span>|<span data-ttu-id="5ee1d-159">String</span><span class="sxs-lookup"><span data-stu-id="5ee1d-159">String</span></span>|<span data-ttu-id="5ee1d-160">Fabricante OEM do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-160">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5ee1d-161">modelo</span><span class="sxs-lookup"><span data-stu-id="5ee1d-161">model</span></span>|<span data-ttu-id="5ee1d-162">String</span><span class="sxs-lookup"><span data-stu-id="5ee1d-162">String</span></span>|<span data-ttu-id="5ee1d-163">Nome do modelo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-163">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5ee1d-164">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="5ee1d-164">enrollmentState</span></span>|[<span data-ttu-id="5ee1d-165">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="5ee1d-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="5ee1d-166">Estado de registro do Intune do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-166">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="5ee1d-167">Os valores possíveis são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="5ee1d-168">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee1d-168">lastContactedDateTime</span></span>|<span data-ttu-id="5ee1d-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee1d-169">DateTimeOffset</span></span>|<span data-ttu-id="5ee1d-170">Data e hora do último contato do Intune para o dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-170">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5ee1d-171">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="5ee1d-171">addressableUserName</span></span>|<span data-ttu-id="5ee1d-172">String</span><span class="sxs-lookup"><span data-stu-id="5ee1d-172">String</span></span>|<span data-ttu-id="5ee1d-173">Nome de usuário endereçável.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-173">Addressable user name.</span></span>|
|<span data-ttu-id="5ee1d-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5ee1d-174">userPrincipalName</span></span>|<span data-ttu-id="5ee1d-175">String</span><span class="sxs-lookup"><span data-stu-id="5ee1d-175">String</span></span>|<span data-ttu-id="5ee1d-176">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-176">User Principal Name.</span></span>|
|<span data-ttu-id="5ee1d-177">resourceName</span><span class="sxs-lookup"><span data-stu-id="5ee1d-177">resourceName</span></span>|<span data-ttu-id="5ee1d-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ee1d-178">String</span></span>|<span data-ttu-id="5ee1d-179">Nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-179">Resource Name.</span></span>|
|<span data-ttu-id="5ee1d-180">skuNumber</span><span class="sxs-lookup"><span data-stu-id="5ee1d-180">skuNumber</span></span>|<span data-ttu-id="5ee1d-181">String</span><span class="sxs-lookup"><span data-stu-id="5ee1d-181">String</span></span>|<span data-ttu-id="5ee1d-182">Número de SKU</span><span class="sxs-lookup"><span data-stu-id="5ee1d-182">SKU Number</span></span>|
|<span data-ttu-id="5ee1d-183">systemFamily</span><span class="sxs-lookup"><span data-stu-id="5ee1d-183">systemFamily</span></span>|<span data-ttu-id="5ee1d-184">String</span><span class="sxs-lookup"><span data-stu-id="5ee1d-184">String</span></span>|<span data-ttu-id="5ee1d-185">Família de sistema</span><span class="sxs-lookup"><span data-stu-id="5ee1d-185">System Family</span></span>|
|<span data-ttu-id="5ee1d-186">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="5ee1d-186">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="5ee1d-187">String</span><span class="sxs-lookup"><span data-stu-id="5ee1d-187">String</span></span>|<span data-ttu-id="5ee1d-188">ID de dispositivo do AAD</span><span class="sxs-lookup"><span data-stu-id="5ee1d-188">AAD Device ID</span></span>|
|<span data-ttu-id="5ee1d-189">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="5ee1d-189">managedDeviceId</span></span>|<span data-ttu-id="5ee1d-190">String</span><span class="sxs-lookup"><span data-stu-id="5ee1d-190">String</span></span>|<span data-ttu-id="5ee1d-191">ID do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5ee1d-191">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="5ee1d-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee1d-192">Response</span></span>
<span data-ttu-id="5ee1d-193">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-193">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ee1d-194">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ee1d-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ee1d-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee1d-195">Request</span></span>
<span data-ttu-id="5ee1d-196">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-196">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 1001

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
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

### <a name="response"></a><span data-ttu-id="5ee1d-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee1d-197">Response</span></span>
<span data-ttu-id="5ee1d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ee1d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1050

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
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




