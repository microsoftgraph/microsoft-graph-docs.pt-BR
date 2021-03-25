---
title: Criar windowsAutopilotDeviceIdentity
description: Crie um novo objeto windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 725d6d5c0cb0f03c9fcb1b2c161959a4242e2a13
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153850"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="402fe-103">Criar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="402fe-103">Create windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="402fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="402fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="402fe-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="402fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="402fe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="402fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="402fe-107">Crie um novo [objeto windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="402fe-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="402fe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="402fe-108">Prerequisites</span></span>
<span data-ttu-id="402fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="402fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="402fe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="402fe-111">Permission type</span></span>|<span data-ttu-id="402fe-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="402fe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="402fe-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="402fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="402fe-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="402fe-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="402fe-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="402fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="402fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="402fe-116">Not supported.</span></span>|
|<span data-ttu-id="402fe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="402fe-117">Application</span></span>|<span data-ttu-id="402fe-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="402fe-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="402fe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="402fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="402fe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="402fe-120">Request headers</span></span>
|<span data-ttu-id="402fe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="402fe-121">Header</span></span>|<span data-ttu-id="402fe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="402fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="402fe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="402fe-123">Authorization</span></span>|<span data-ttu-id="402fe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="402fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="402fe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="402fe-125">Accept</span></span>|<span data-ttu-id="402fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="402fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="402fe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="402fe-127">Request body</span></span>
<span data-ttu-id="402fe-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="402fe-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="402fe-129">A tabela a seguir mostra as propriedades necessárias ao criar o windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="402fe-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="402fe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="402fe-130">Property</span></span>|<span data-ttu-id="402fe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="402fe-131">Type</span></span>|<span data-ttu-id="402fe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="402fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="402fe-133">id</span><span class="sxs-lookup"><span data-stu-id="402fe-133">id</span></span>|<span data-ttu-id="402fe-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-134">String</span></span>|<span data-ttu-id="402fe-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="402fe-135">The GUID for the object</span></span>|
|<span data-ttu-id="402fe-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="402fe-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="402fe-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="402fe-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="402fe-138">Status da atribuição de perfil do dispositivo de piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="402fe-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="402fe-139">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="402fe-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="402fe-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="402fe-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="402fe-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="402fe-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="402fe-142">Status detalhado da atribuição de perfil do dispositivo de piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="402fe-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="402fe-143">Os valores possíveis são: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span><span class="sxs-lookup"><span data-stu-id="402fe-143">Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span></span>|
|<span data-ttu-id="402fe-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="402fe-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="402fe-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="402fe-145">DateTimeOffset</span></span>|<span data-ttu-id="402fe-146">Hora do conjunto de perfis do dispositivo de piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="402fe-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="402fe-147">groupTag</span><span class="sxs-lookup"><span data-stu-id="402fe-147">groupTag</span></span>|<span data-ttu-id="402fe-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-148">String</span></span>|<span data-ttu-id="402fe-149">Marca de grupo do dispositivo de piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="402fe-149">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="402fe-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="402fe-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="402fe-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-151">String</span></span>|<span data-ttu-id="402fe-152">Purchase Order Identifier of the Windows autopilot device.</span><span class="sxs-lookup"><span data-stu-id="402fe-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="402fe-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="402fe-153">serialNumber</span></span>|<span data-ttu-id="402fe-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-154">String</span></span>|<span data-ttu-id="402fe-155">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="402fe-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="402fe-156">productKey</span><span class="sxs-lookup"><span data-stu-id="402fe-156">productKey</span></span>|<span data-ttu-id="402fe-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-157">String</span></span>|<span data-ttu-id="402fe-158">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="402fe-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="402fe-159">fabricante</span><span class="sxs-lookup"><span data-stu-id="402fe-159">manufacturer</span></span>|<span data-ttu-id="402fe-160">String</span><span class="sxs-lookup"><span data-stu-id="402fe-160">String</span></span>|<span data-ttu-id="402fe-161">Fabricante do Oem do dispositivo de piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="402fe-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="402fe-162">modelo</span><span class="sxs-lookup"><span data-stu-id="402fe-162">model</span></span>|<span data-ttu-id="402fe-163">String</span><span class="sxs-lookup"><span data-stu-id="402fe-163">String</span></span>|<span data-ttu-id="402fe-164">Nome do modelo do dispositivo de piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="402fe-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="402fe-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="402fe-165">enrollmentState</span></span>|[<span data-ttu-id="402fe-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="402fe-166">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="402fe-167">Estado de registro do Intune do dispositivo de piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="402fe-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="402fe-168">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="402fe-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="402fe-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="402fe-169">lastContactedDateTime</span></span>|<span data-ttu-id="402fe-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="402fe-170">DateTimeOffset</span></span>|<span data-ttu-id="402fe-171">Intune Última Data Contada Hora do dispositivo de piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="402fe-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="402fe-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="402fe-172">addressableUserName</span></span>|<span data-ttu-id="402fe-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-173">String</span></span>|<span data-ttu-id="402fe-174">Nome de usuário acessível.</span><span class="sxs-lookup"><span data-stu-id="402fe-174">Addressable user name.</span></span>|
|<span data-ttu-id="402fe-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="402fe-175">userPrincipalName</span></span>|<span data-ttu-id="402fe-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-176">String</span></span>|<span data-ttu-id="402fe-177">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="402fe-177">User Principal Name.</span></span>|
|<span data-ttu-id="402fe-178">resourceName</span><span class="sxs-lookup"><span data-stu-id="402fe-178">resourceName</span></span>|<span data-ttu-id="402fe-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-179">String</span></span>|<span data-ttu-id="402fe-180">Nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="402fe-180">Resource Name.</span></span>|
|<span data-ttu-id="402fe-181">skuNumber</span><span class="sxs-lookup"><span data-stu-id="402fe-181">skuNumber</span></span>|<span data-ttu-id="402fe-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-182">String</span></span>|<span data-ttu-id="402fe-183">Número SKU</span><span class="sxs-lookup"><span data-stu-id="402fe-183">SKU Number</span></span>|
|<span data-ttu-id="402fe-184">systemFamily</span><span class="sxs-lookup"><span data-stu-id="402fe-184">systemFamily</span></span>|<span data-ttu-id="402fe-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-185">String</span></span>|<span data-ttu-id="402fe-186">Família do Sistema</span><span class="sxs-lookup"><span data-stu-id="402fe-186">System Family</span></span>|
|<span data-ttu-id="402fe-187">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="402fe-187">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="402fe-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-188">String</span></span>|<span data-ttu-id="402fe-189">ID do dispositivo AAD - a ser preterida</span><span class="sxs-lookup"><span data-stu-id="402fe-189">AAD Device ID - to be deprecated</span></span>|
|<span data-ttu-id="402fe-190">azureAdDeviceId</span><span class="sxs-lookup"><span data-stu-id="402fe-190">azureAdDeviceId</span></span>|<span data-ttu-id="402fe-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-191">String</span></span>|<span data-ttu-id="402fe-192">ID do dispositivo AAD</span><span class="sxs-lookup"><span data-stu-id="402fe-192">AAD Device ID</span></span>|
|<span data-ttu-id="402fe-193">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="402fe-193">managedDeviceId</span></span>|<span data-ttu-id="402fe-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-194">String</span></span>|<span data-ttu-id="402fe-195">ID de dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="402fe-195">Managed Device ID</span></span>|
|<span data-ttu-id="402fe-196">displayName</span><span class="sxs-lookup"><span data-stu-id="402fe-196">displayName</span></span>|<span data-ttu-id="402fe-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="402fe-197">String</span></span>|<span data-ttu-id="402fe-198">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="402fe-198">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="402fe-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="402fe-199">Response</span></span>
<span data-ttu-id="402fe-200">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="402fe-200">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="402fe-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="402fe-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="402fe-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="402fe-202">Request</span></span>
<span data-ttu-id="402fe-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="402fe-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 1077

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
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
  "azureAdDeviceId": "Azure Ad Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="402fe-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="402fe-204">Response</span></span>
<span data-ttu-id="402fe-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="402fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
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
  "azureAdDeviceId": "Azure Ad Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```




