---
title: Criar windowsAutopilotDeviceIdentity
description: Crie um novo objeto de windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 56d200bd53e94715ba102f6c96bba3e3b5dd892b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919096"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="58528-103">Criar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="58528-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="58528-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="58528-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58528-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="58528-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58528-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="58528-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58528-107">Crie um novo objeto de [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="58528-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58528-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58528-108">Prerequisites</span></span>
<span data-ttu-id="58528-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58528-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58528-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58528-111">Permission type</span></span>|<span data-ttu-id="58528-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58528-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58528-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58528-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58528-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58528-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="58528-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58528-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58528-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58528-116">Not supported.</span></span>|
|<span data-ttu-id="58528-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58528-117">Application</span></span>|<span data-ttu-id="58528-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58528-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58528-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58528-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="58528-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58528-120">Request headers</span></span>
|<span data-ttu-id="58528-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58528-121">Header</span></span>|<span data-ttu-id="58528-122">Valor</span><span class="sxs-lookup"><span data-stu-id="58528-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58528-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="58528-123">Authorization</span></span>|<span data-ttu-id="58528-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58528-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58528-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58528-125">Accept</span></span>|<span data-ttu-id="58528-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58528-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58528-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58528-127">Request body</span></span>
<span data-ttu-id="58528-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="58528-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="58528-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="58528-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="58528-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58528-130">Property</span></span>|<span data-ttu-id="58528-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="58528-131">Type</span></span>|<span data-ttu-id="58528-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="58528-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58528-133">id</span><span class="sxs-lookup"><span data-stu-id="58528-133">id</span></span>|<span data-ttu-id="58528-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58528-134">String</span></span>|<span data-ttu-id="58528-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="58528-135">The GUID for the object</span></span>|
|<span data-ttu-id="58528-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="58528-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="58528-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="58528-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="58528-138">Status de atribuição de perfil do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="58528-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="58528-139">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="58528-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="58528-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="58528-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="58528-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="58528-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="58528-142">Atribuição de perfil detalhadas de status do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="58528-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="58528-143">Os valores possíveis são: `none` e `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="58528-143">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="58528-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="58528-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="58528-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58528-145">DateTimeOffset</span></span>|<span data-ttu-id="58528-146">Perfil definir a hora do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="58528-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58528-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="58528-147">orderIdentifier</span></span>|<span data-ttu-id="58528-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58528-148">String</span></span>|<span data-ttu-id="58528-149">Ordem o identificador do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="58528-149">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58528-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="58528-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="58528-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58528-151">String</span></span>|<span data-ttu-id="58528-152">Identificador de ordem de compra do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="58528-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58528-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="58528-153">serialNumber</span></span>|<span data-ttu-id="58528-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58528-154">String</span></span>|<span data-ttu-id="58528-155">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="58528-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58528-156">productKey</span><span class="sxs-lookup"><span data-stu-id="58528-156">productKey</span></span>|<span data-ttu-id="58528-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58528-157">String</span></span>|<span data-ttu-id="58528-158">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="58528-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58528-159">fabricante</span><span class="sxs-lookup"><span data-stu-id="58528-159">manufacturer</span></span>|<span data-ttu-id="58528-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58528-160">String</span></span>|<span data-ttu-id="58528-161">OEM do fabricante do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="58528-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58528-162">modelo</span><span class="sxs-lookup"><span data-stu-id="58528-162">model</span></span>|<span data-ttu-id="58528-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58528-163">String</span></span>|<span data-ttu-id="58528-164">Nome do modelo do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="58528-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58528-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="58528-165">enrollmentState</span></span>|[<span data-ttu-id="58528-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="58528-166">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="58528-167">Estado de inscrição Intune do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="58528-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="58528-168">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="58528-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="58528-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="58528-169">lastContactedDateTime</span></span>|<span data-ttu-id="58528-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58528-170">DateTimeOffset</span></span>|<span data-ttu-id="58528-171">Intune última contatado data hora do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="58528-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58528-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="58528-172">addressableUserName</span></span>|<span data-ttu-id="58528-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58528-173">String</span></span>|<span data-ttu-id="58528-174">Nome de usuário endereçável.</span><span class="sxs-lookup"><span data-stu-id="58528-174">Addressable user name.</span></span>|
|<span data-ttu-id="58528-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="58528-175">userPrincipalName</span></span>|<span data-ttu-id="58528-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58528-176">String</span></span>|<span data-ttu-id="58528-177">Nome Principal de usuário.</span><span class="sxs-lookup"><span data-stu-id="58528-177">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="58528-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="58528-178">Response</span></span>
<span data-ttu-id="58528-179">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58528-179">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58528-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58528-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="58528-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58528-181">Request</span></span>
<span data-ttu-id="58528-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58528-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58528-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="58528-183">Response</span></span>
<span data-ttu-id="58528-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58528-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





