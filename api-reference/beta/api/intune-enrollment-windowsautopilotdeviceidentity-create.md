---
title: Criar windowsAutopilotDeviceIdentity
description: Crie um novo objeto de windowsAutopilotDeviceIdentity.
author: tfitzmac
ms.openlocfilehash: 1e4a9d43755fff787efa08a8c727e6ddc35fa904
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316013"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="082ae-103">Criar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="082ae-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="082ae-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="082ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="082ae-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="082ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="082ae-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="082ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="082ae-107">Crie um novo objeto de [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="082ae-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="082ae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="082ae-108">Prerequisites</span></span>
<span data-ttu-id="082ae-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="082ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="082ae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="082ae-111">Permission type</span></span>|<span data-ttu-id="082ae-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="082ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="082ae-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="082ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="082ae-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="082ae-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="082ae-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="082ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="082ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="082ae-116">Not supported.</span></span>|
|<span data-ttu-id="082ae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="082ae-117">Application</span></span>|<span data-ttu-id="082ae-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="082ae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="082ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="082ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="082ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="082ae-120">Request headers</span></span>
|<span data-ttu-id="082ae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="082ae-121">Header</span></span>|<span data-ttu-id="082ae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="082ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="082ae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="082ae-123">Authorization</span></span>|<span data-ttu-id="082ae-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="082ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="082ae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="082ae-125">Accept</span></span>|<span data-ttu-id="082ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="082ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="082ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="082ae-127">Request body</span></span>
<span data-ttu-id="082ae-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="082ae-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="082ae-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="082ae-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="082ae-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="082ae-130">Property</span></span>|<span data-ttu-id="082ae-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="082ae-131">Type</span></span>|<span data-ttu-id="082ae-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="082ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="082ae-133">id</span><span class="sxs-lookup"><span data-stu-id="082ae-133">id</span></span>|<span data-ttu-id="082ae-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="082ae-134">String</span></span>|<span data-ttu-id="082ae-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="082ae-135">The GUID for the object</span></span>|
|<span data-ttu-id="082ae-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="082ae-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="082ae-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="082ae-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="082ae-138">Status de atribuição de perfil do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="082ae-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="082ae-139">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="082ae-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="082ae-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="082ae-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="082ae-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="082ae-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="082ae-142">Atribuição de perfil detalhadas de status do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="082ae-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="082ae-143">Os valores possíveis são: `none` e `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="082ae-143">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="082ae-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="082ae-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="082ae-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="082ae-145">DateTimeOffset</span></span>|<span data-ttu-id="082ae-146">Perfil definir a hora do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="082ae-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="082ae-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="082ae-147">orderIdentifier</span></span>|<span data-ttu-id="082ae-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="082ae-148">String</span></span>|<span data-ttu-id="082ae-149">Ordem o identificador do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="082ae-149">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="082ae-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="082ae-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="082ae-151">String</span><span class="sxs-lookup"><span data-stu-id="082ae-151">String</span></span>|<span data-ttu-id="082ae-152">Identificador de ordem de compra do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="082ae-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="082ae-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="082ae-153">serialNumber</span></span>|<span data-ttu-id="082ae-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="082ae-154">String</span></span>|<span data-ttu-id="082ae-155">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="082ae-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="082ae-156">productKey</span><span class="sxs-lookup"><span data-stu-id="082ae-156">productKey</span></span>|<span data-ttu-id="082ae-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="082ae-157">String</span></span>|<span data-ttu-id="082ae-158">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="082ae-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="082ae-159">fabricante</span><span class="sxs-lookup"><span data-stu-id="082ae-159">manufacturer</span></span>|<span data-ttu-id="082ae-160">String</span><span class="sxs-lookup"><span data-stu-id="082ae-160">String</span></span>|<span data-ttu-id="082ae-161">OEM do fabricante do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="082ae-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="082ae-162">modelo</span><span class="sxs-lookup"><span data-stu-id="082ae-162">model</span></span>|<span data-ttu-id="082ae-163">String</span><span class="sxs-lookup"><span data-stu-id="082ae-163">String</span></span>|<span data-ttu-id="082ae-164">Nome do modelo do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="082ae-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="082ae-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="082ae-165">enrollmentState</span></span>|[<span data-ttu-id="082ae-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="082ae-166">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="082ae-167">Estado de inscrição Intune do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="082ae-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="082ae-168">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="082ae-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="082ae-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="082ae-169">lastContactedDateTime</span></span>|<span data-ttu-id="082ae-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="082ae-170">DateTimeOffset</span></span>|<span data-ttu-id="082ae-171">Intune última contatado data hora do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="082ae-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="082ae-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="082ae-172">addressableUserName</span></span>|<span data-ttu-id="082ae-173">String</span><span class="sxs-lookup"><span data-stu-id="082ae-173">String</span></span>|<span data-ttu-id="082ae-174">Nome de usuário endereçável.</span><span class="sxs-lookup"><span data-stu-id="082ae-174">Addressable user name.</span></span>|
|<span data-ttu-id="082ae-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="082ae-175">userPrincipalName</span></span>|<span data-ttu-id="082ae-176">String</span><span class="sxs-lookup"><span data-stu-id="082ae-176">String</span></span>|<span data-ttu-id="082ae-177">Nome Principal de usuário.</span><span class="sxs-lookup"><span data-stu-id="082ae-177">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="082ae-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="082ae-178">Response</span></span>
<span data-ttu-id="082ae-179">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="082ae-179">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="082ae-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="082ae-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="082ae-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="082ae-181">Request</span></span>
<span data-ttu-id="082ae-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="082ae-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 755

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
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="082ae-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="082ae-183">Response</span></span>
<span data-ttu-id="082ae-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="082ae-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 804

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
  "userPrincipalName": "User Principal Name value"
}
```





