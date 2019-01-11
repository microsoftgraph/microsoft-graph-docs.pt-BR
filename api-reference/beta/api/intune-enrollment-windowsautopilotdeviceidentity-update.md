---
title: Atualizar windowsAutopilotDeviceIdentity
description: Atualize as propriedades de um objeto windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ea1200951231b43b2d2fd9242c241a54518fb1c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853533"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="ddceb-103">Atualizar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="ddceb-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="ddceb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ddceb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddceb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ddceb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ddceb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ddceb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddceb-107">Atualize as propriedades de um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="ddceb-107">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ddceb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ddceb-108">Prerequisites</span></span>
<span data-ttu-id="ddceb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddceb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddceb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddceb-111">Permission type</span></span>|<span data-ttu-id="ddceb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ddceb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddceb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddceb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ddceb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddceb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ddceb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddceb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddceb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddceb-116">Not supported.</span></span>|
|<span data-ttu-id="ddceb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddceb-117">Application</span></span>|<span data-ttu-id="ddceb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddceb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddceb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddceb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="ddceb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddceb-120">Request headers</span></span>
|<span data-ttu-id="ddceb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ddceb-121">Header</span></span>|<span data-ttu-id="ddceb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ddceb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddceb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddceb-123">Authorization</span></span>|<span data-ttu-id="ddceb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddceb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddceb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ddceb-125">Accept</span></span>|<span data-ttu-id="ddceb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ddceb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddceb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddceb-127">Request body</span></span>
<span data-ttu-id="ddceb-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="ddceb-128">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="ddceb-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="ddceb-129">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="ddceb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddceb-130">Property</span></span>|<span data-ttu-id="ddceb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddceb-131">Type</span></span>|<span data-ttu-id="ddceb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddceb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddceb-133">id</span><span class="sxs-lookup"><span data-stu-id="ddceb-133">id</span></span>|<span data-ttu-id="ddceb-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddceb-134">String</span></span>|<span data-ttu-id="ddceb-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="ddceb-135">The GUID for the object</span></span>|
|<span data-ttu-id="ddceb-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="ddceb-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="ddceb-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="ddceb-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="ddceb-138">Status de atribuição de perfil do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="ddceb-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="ddceb-139">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ddceb-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="ddceb-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="ddceb-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="ddceb-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="ddceb-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="ddceb-142">Atribuição de perfil detalhadas de status do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="ddceb-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="ddceb-143">Os valores possíveis são: `none` e `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="ddceb-143">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="ddceb-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddceb-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="ddceb-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddceb-145">DateTimeOffset</span></span>|<span data-ttu-id="ddceb-146">Perfil definir a hora do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="ddceb-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ddceb-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="ddceb-147">orderIdentifier</span></span>|<span data-ttu-id="ddceb-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddceb-148">String</span></span>|<span data-ttu-id="ddceb-149">Ordem o identificador do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="ddceb-149">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ddceb-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="ddceb-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="ddceb-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddceb-151">String</span></span>|<span data-ttu-id="ddceb-152">Identificador de ordem de compra do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="ddceb-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ddceb-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ddceb-153">serialNumber</span></span>|<span data-ttu-id="ddceb-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddceb-154">String</span></span>|<span data-ttu-id="ddceb-155">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="ddceb-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ddceb-156">productKey</span><span class="sxs-lookup"><span data-stu-id="ddceb-156">productKey</span></span>|<span data-ttu-id="ddceb-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddceb-157">String</span></span>|<span data-ttu-id="ddceb-158">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="ddceb-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ddceb-159">fabricante</span><span class="sxs-lookup"><span data-stu-id="ddceb-159">manufacturer</span></span>|<span data-ttu-id="ddceb-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddceb-160">String</span></span>|<span data-ttu-id="ddceb-161">OEM do fabricante do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="ddceb-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ddceb-162">modelo</span><span class="sxs-lookup"><span data-stu-id="ddceb-162">model</span></span>|<span data-ttu-id="ddceb-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddceb-163">String</span></span>|<span data-ttu-id="ddceb-164">Nome do modelo do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="ddceb-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ddceb-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ddceb-165">enrollmentState</span></span>|[<span data-ttu-id="ddceb-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ddceb-166">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="ddceb-167">Estado de inscrição Intune do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="ddceb-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="ddceb-168">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="ddceb-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="ddceb-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddceb-169">lastContactedDateTime</span></span>|<span data-ttu-id="ddceb-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddceb-170">DateTimeOffset</span></span>|<span data-ttu-id="ddceb-171">Intune última contatado data hora do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="ddceb-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ddceb-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="ddceb-172">addressableUserName</span></span>|<span data-ttu-id="ddceb-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddceb-173">String</span></span>|<span data-ttu-id="ddceb-174">Nome de usuário endereçável.</span><span class="sxs-lookup"><span data-stu-id="ddceb-174">Addressable user name.</span></span>|
|<span data-ttu-id="ddceb-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ddceb-175">userPrincipalName</span></span>|<span data-ttu-id="ddceb-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddceb-176">String</span></span>|<span data-ttu-id="ddceb-177">Nome Principal de usuário.</span><span class="sxs-lookup"><span data-stu-id="ddceb-177">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="ddceb-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddceb-178">Response</span></span>
<span data-ttu-id="ddceb-179">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddceb-179">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddceb-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddceb-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="ddceb-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddceb-181">Request</span></span>
<span data-ttu-id="ddceb-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddceb-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 686

{
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

### <a name="response"></a><span data-ttu-id="ddceb-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddceb-183">Response</span></span>
<span data-ttu-id="ddceb-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddceb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





