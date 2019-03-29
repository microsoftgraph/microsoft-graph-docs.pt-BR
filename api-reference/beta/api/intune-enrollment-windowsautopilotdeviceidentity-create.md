---
title: Criar windowsAutopilotDeviceIdentity
description: Criar um novo objeto windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1165fbd0ce159cc1c8717df2ed64431aac26f722
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958442"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="2f96c-103">Criar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2f96c-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="2f96c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f96c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f96c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f96c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f96c-106">Criar um novo objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="2f96c-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f96c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f96c-107">Prerequisites</span></span>
<span data-ttu-id="2f96c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f96c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f96c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f96c-110">Permission type</span></span>|<span data-ttu-id="2f96c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f96c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f96c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f96c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f96c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f96c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2f96c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f96c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f96c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f96c-115">Not supported.</span></span>|
|<span data-ttu-id="2f96c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f96c-116">Application</span></span>|<span data-ttu-id="2f96c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f96c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f96c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f96c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="2f96c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f96c-119">Request headers</span></span>
|<span data-ttu-id="2f96c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f96c-120">Header</span></span>|<span data-ttu-id="2f96c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2f96c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f96c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f96c-122">Authorization</span></span>|<span data-ttu-id="2f96c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f96c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f96c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f96c-124">Accept</span></span>|<span data-ttu-id="2f96c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f96c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f96c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f96c-126">Request body</span></span>
<span data-ttu-id="2f96c-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="2f96c-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="2f96c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="2f96c-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="2f96c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f96c-129">Property</span></span>|<span data-ttu-id="2f96c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f96c-130">Type</span></span>|<span data-ttu-id="2f96c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f96c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f96c-132">id</span><span class="sxs-lookup"><span data-stu-id="2f96c-132">id</span></span>|<span data-ttu-id="2f96c-133">String</span><span class="sxs-lookup"><span data-stu-id="2f96c-133">String</span></span>|<span data-ttu-id="2f96c-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="2f96c-134">The GUID for the object</span></span>|
|<span data-ttu-id="2f96c-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="2f96c-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="2f96c-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="2f96c-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="2f96c-137">Status de atribuição de perfil do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2f96c-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="2f96c-138">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2f96c-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="2f96c-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="2f96c-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="2f96c-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="2f96c-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="2f96c-141">Atribuição de perfil status detalhado do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2f96c-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="2f96c-142">Os valores possíveis são: `none` e `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="2f96c-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="2f96c-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f96c-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="2f96c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f96c-144">DateTimeOffset</span></span>|<span data-ttu-id="2f96c-145">Hora do conjunto de perfis do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2f96c-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f96c-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="2f96c-146">orderIdentifier</span></span>|<span data-ttu-id="2f96c-147">String</span><span class="sxs-lookup"><span data-stu-id="2f96c-147">String</span></span>|<span data-ttu-id="2f96c-148">Identificador de pedidos do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2f96c-148">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f96c-149">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="2f96c-149">purchaseOrderIdentifier</span></span>|<span data-ttu-id="2f96c-150">String</span><span class="sxs-lookup"><span data-stu-id="2f96c-150">String</span></span>|<span data-ttu-id="2f96c-151">Identificador de ordem de compra do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2f96c-151">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f96c-152">serialNumber</span><span class="sxs-lookup"><span data-stu-id="2f96c-152">serialNumber</span></span>|<span data-ttu-id="2f96c-153">String</span><span class="sxs-lookup"><span data-stu-id="2f96c-153">String</span></span>|<span data-ttu-id="2f96c-154">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2f96c-154">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f96c-155">productKey</span><span class="sxs-lookup"><span data-stu-id="2f96c-155">productKey</span></span>|<span data-ttu-id="2f96c-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f96c-156">String</span></span>|<span data-ttu-id="2f96c-157">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2f96c-157">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f96c-158">fabricante</span><span class="sxs-lookup"><span data-stu-id="2f96c-158">manufacturer</span></span>|<span data-ttu-id="2f96c-159">String</span><span class="sxs-lookup"><span data-stu-id="2f96c-159">String</span></span>|<span data-ttu-id="2f96c-160">Fabricante OEM do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2f96c-160">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f96c-161">modelo</span><span class="sxs-lookup"><span data-stu-id="2f96c-161">model</span></span>|<span data-ttu-id="2f96c-162">String</span><span class="sxs-lookup"><span data-stu-id="2f96c-162">String</span></span>|<span data-ttu-id="2f96c-163">Nome do modelo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2f96c-163">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f96c-164">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="2f96c-164">enrollmentState</span></span>|[<span data-ttu-id="2f96c-165">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="2f96c-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="2f96c-166">Estado de registro do Intune do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2f96c-166">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="2f96c-167">Os valores possíveis são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="2f96c-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="2f96c-168">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f96c-168">lastContactedDateTime</span></span>|<span data-ttu-id="2f96c-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f96c-169">DateTimeOffset</span></span>|<span data-ttu-id="2f96c-170">Data e hora do último contato do Intune para o dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2f96c-170">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f96c-171">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="2f96c-171">addressableUserName</span></span>|<span data-ttu-id="2f96c-172">String</span><span class="sxs-lookup"><span data-stu-id="2f96c-172">String</span></span>|<span data-ttu-id="2f96c-173">Nome de usuário endereçável.</span><span class="sxs-lookup"><span data-stu-id="2f96c-173">Addressable user name.</span></span>|
|<span data-ttu-id="2f96c-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2f96c-174">userPrincipalName</span></span>|<span data-ttu-id="2f96c-175">String</span><span class="sxs-lookup"><span data-stu-id="2f96c-175">String</span></span>|<span data-ttu-id="2f96c-176">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="2f96c-176">User Principal Name.</span></span>|
|<span data-ttu-id="2f96c-177">resourceName</span><span class="sxs-lookup"><span data-stu-id="2f96c-177">resourceName</span></span>|<span data-ttu-id="2f96c-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f96c-178">String</span></span>|<span data-ttu-id="2f96c-179">Nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f96c-179">Resource Name.</span></span>|
|<span data-ttu-id="2f96c-180">skuNumber</span><span class="sxs-lookup"><span data-stu-id="2f96c-180">skuNumber</span></span>|<span data-ttu-id="2f96c-181">String</span><span class="sxs-lookup"><span data-stu-id="2f96c-181">String</span></span>|<span data-ttu-id="2f96c-182">Número de SKU</span><span class="sxs-lookup"><span data-stu-id="2f96c-182">SKU Number</span></span>|
|<span data-ttu-id="2f96c-183">systemFamily</span><span class="sxs-lookup"><span data-stu-id="2f96c-183">systemFamily</span></span>|<span data-ttu-id="2f96c-184">String</span><span class="sxs-lookup"><span data-stu-id="2f96c-184">String</span></span>|<span data-ttu-id="2f96c-185">Família de sistema</span><span class="sxs-lookup"><span data-stu-id="2f96c-185">System Family</span></span>|
|<span data-ttu-id="2f96c-186">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="2f96c-186">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="2f96c-187">String</span><span class="sxs-lookup"><span data-stu-id="2f96c-187">String</span></span>|<span data-ttu-id="2f96c-188">ID de dispositivo do AAD</span><span class="sxs-lookup"><span data-stu-id="2f96c-188">AAD Device ID</span></span>|
|<span data-ttu-id="2f96c-189">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="2f96c-189">managedDeviceId</span></span>|<span data-ttu-id="2f96c-190">String</span><span class="sxs-lookup"><span data-stu-id="2f96c-190">String</span></span>|<span data-ttu-id="2f96c-191">ID do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="2f96c-191">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="2f96c-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f96c-192">Response</span></span>
<span data-ttu-id="2f96c-193">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f96c-193">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f96c-194">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f96c-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f96c-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f96c-195">Request</span></span>
<span data-ttu-id="2f96c-196">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f96c-196">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f96c-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f96c-197">Response</span></span>
<span data-ttu-id="2f96c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f96c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




