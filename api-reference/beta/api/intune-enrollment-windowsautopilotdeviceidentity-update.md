---
title: Atualizar windowsAutopilotDeviceIdentity
description: Atualiza as propriedades de um objeto windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4132ebc9d93eae71712b04479c1139e1942a9979
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958729"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="14554-103">Atualizar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="14554-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="14554-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14554-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14554-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14554-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14554-106">Atualiza as propriedades de um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="14554-106">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14554-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14554-107">Prerequisites</span></span>
<span data-ttu-id="14554-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14554-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14554-110">Permission type</span></span>|<span data-ttu-id="14554-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14554-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14554-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14554-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14554-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14554-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="14554-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14554-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14554-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14554-115">Not supported.</span></span>|
|<span data-ttu-id="14554-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14554-116">Application</span></span>|<span data-ttu-id="14554-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14554-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14554-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14554-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="14554-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14554-119">Request headers</span></span>
|<span data-ttu-id="14554-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14554-120">Header</span></span>|<span data-ttu-id="14554-121">Valor</span><span class="sxs-lookup"><span data-stu-id="14554-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14554-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="14554-122">Authorization</span></span>|<span data-ttu-id="14554-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14554-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14554-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14554-124">Accept</span></span>|<span data-ttu-id="14554-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14554-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14554-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14554-126">Request body</span></span>
<span data-ttu-id="14554-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="14554-127">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="14554-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="14554-128">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="14554-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14554-129">Property</span></span>|<span data-ttu-id="14554-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="14554-130">Type</span></span>|<span data-ttu-id="14554-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="14554-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14554-132">id</span><span class="sxs-lookup"><span data-stu-id="14554-132">id</span></span>|<span data-ttu-id="14554-133">String</span><span class="sxs-lookup"><span data-stu-id="14554-133">String</span></span>|<span data-ttu-id="14554-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="14554-134">The GUID for the object</span></span>|
|<span data-ttu-id="14554-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="14554-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="14554-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="14554-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="14554-137">Status de atribuição de perfil do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="14554-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="14554-138">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="14554-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="14554-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="14554-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="14554-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="14554-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="14554-141">Atribuição de perfil status detalhado do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="14554-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="14554-142">Os valores possíveis são: `none` e `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="14554-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="14554-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="14554-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="14554-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14554-144">DateTimeOffset</span></span>|<span data-ttu-id="14554-145">Hora do conjunto de perfis do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="14554-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14554-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="14554-146">orderIdentifier</span></span>|<span data-ttu-id="14554-147">String</span><span class="sxs-lookup"><span data-stu-id="14554-147">String</span></span>|<span data-ttu-id="14554-148">Identificador de pedidos do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="14554-148">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14554-149">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="14554-149">purchaseOrderIdentifier</span></span>|<span data-ttu-id="14554-150">String</span><span class="sxs-lookup"><span data-stu-id="14554-150">String</span></span>|<span data-ttu-id="14554-151">Identificador de ordem de compra do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="14554-151">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14554-152">serialNumber</span><span class="sxs-lookup"><span data-stu-id="14554-152">serialNumber</span></span>|<span data-ttu-id="14554-153">String</span><span class="sxs-lookup"><span data-stu-id="14554-153">String</span></span>|<span data-ttu-id="14554-154">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="14554-154">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14554-155">productKey</span><span class="sxs-lookup"><span data-stu-id="14554-155">productKey</span></span>|<span data-ttu-id="14554-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14554-156">String</span></span>|<span data-ttu-id="14554-157">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="14554-157">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14554-158">fabricante</span><span class="sxs-lookup"><span data-stu-id="14554-158">manufacturer</span></span>|<span data-ttu-id="14554-159">String</span><span class="sxs-lookup"><span data-stu-id="14554-159">String</span></span>|<span data-ttu-id="14554-160">Fabricante OEM do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="14554-160">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14554-161">modelo</span><span class="sxs-lookup"><span data-stu-id="14554-161">model</span></span>|<span data-ttu-id="14554-162">String</span><span class="sxs-lookup"><span data-stu-id="14554-162">String</span></span>|<span data-ttu-id="14554-163">Nome do modelo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="14554-163">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14554-164">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="14554-164">enrollmentState</span></span>|[<span data-ttu-id="14554-165">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="14554-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="14554-166">Estado de registro do Intune do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="14554-166">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="14554-167">Os valores possíveis são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="14554-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="14554-168">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="14554-168">lastContactedDateTime</span></span>|<span data-ttu-id="14554-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14554-169">DateTimeOffset</span></span>|<span data-ttu-id="14554-170">Data e hora do último contato do Intune para o dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="14554-170">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14554-171">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="14554-171">addressableUserName</span></span>|<span data-ttu-id="14554-172">String</span><span class="sxs-lookup"><span data-stu-id="14554-172">String</span></span>|<span data-ttu-id="14554-173">Nome de usuário endereçável.</span><span class="sxs-lookup"><span data-stu-id="14554-173">Addressable user name.</span></span>|
|<span data-ttu-id="14554-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="14554-174">userPrincipalName</span></span>|<span data-ttu-id="14554-175">String</span><span class="sxs-lookup"><span data-stu-id="14554-175">String</span></span>|<span data-ttu-id="14554-176">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="14554-176">User Principal Name.</span></span>|
|<span data-ttu-id="14554-177">resourceName</span><span class="sxs-lookup"><span data-stu-id="14554-177">resourceName</span></span>|<span data-ttu-id="14554-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14554-178">String</span></span>|<span data-ttu-id="14554-179">Nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="14554-179">Resource Name.</span></span>|
|<span data-ttu-id="14554-180">skuNumber</span><span class="sxs-lookup"><span data-stu-id="14554-180">skuNumber</span></span>|<span data-ttu-id="14554-181">String</span><span class="sxs-lookup"><span data-stu-id="14554-181">String</span></span>|<span data-ttu-id="14554-182">Número de SKU</span><span class="sxs-lookup"><span data-stu-id="14554-182">SKU Number</span></span>|
|<span data-ttu-id="14554-183">systemFamily</span><span class="sxs-lookup"><span data-stu-id="14554-183">systemFamily</span></span>|<span data-ttu-id="14554-184">String</span><span class="sxs-lookup"><span data-stu-id="14554-184">String</span></span>|<span data-ttu-id="14554-185">Família de sistema</span><span class="sxs-lookup"><span data-stu-id="14554-185">System Family</span></span>|
|<span data-ttu-id="14554-186">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="14554-186">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="14554-187">String</span><span class="sxs-lookup"><span data-stu-id="14554-187">String</span></span>|<span data-ttu-id="14554-188">ID de dispositivo do AAD</span><span class="sxs-lookup"><span data-stu-id="14554-188">AAD Device ID</span></span>|
|<span data-ttu-id="14554-189">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="14554-189">managedDeviceId</span></span>|<span data-ttu-id="14554-190">String</span><span class="sxs-lookup"><span data-stu-id="14554-190">String</span></span>|<span data-ttu-id="14554-191">ID do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="14554-191">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="14554-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="14554-192">Response</span></span>
<span data-ttu-id="14554-193">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14554-193">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14554-194">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14554-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="14554-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14554-195">Request</span></span>
<span data-ttu-id="14554-196">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14554-196">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="14554-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="14554-197">Response</span></span>
<span data-ttu-id="14554-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14554-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




