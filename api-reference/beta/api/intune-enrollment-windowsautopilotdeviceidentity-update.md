---
title: Atualizar windowsAutopilotDeviceIdentity
description: Atualiza as propriedades de um objeto windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8d1afaa0b810d2559daa358c9d7af0895e5ac2d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159518"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="f2135-103">Atualizar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f2135-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="f2135-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2135-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2135-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2135-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2135-106">Atualiza as propriedades de um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="f2135-106">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2135-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2135-107">Prerequisites</span></span>
<span data-ttu-id="f2135-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2135-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f2135-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2135-110">Permission type</span></span>|<span data-ttu-id="f2135-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2135-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2135-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2135-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2135-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2135-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f2135-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2135-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2135-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2135-115">Not supported.</span></span>|
|<span data-ttu-id="f2135-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2135-116">Application</span></span>|<span data-ttu-id="f2135-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2135-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2135-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2135-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="f2135-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2135-119">Request headers</span></span>
|<span data-ttu-id="f2135-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2135-120">Header</span></span>|<span data-ttu-id="f2135-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f2135-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2135-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2135-122">Authorization</span></span>|<span data-ttu-id="f2135-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2135-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2135-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2135-124">Accept</span></span>|<span data-ttu-id="f2135-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f2135-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2135-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2135-126">Request body</span></span>
<span data-ttu-id="f2135-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="f2135-127">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="f2135-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="f2135-128">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="f2135-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2135-129">Property</span></span>|<span data-ttu-id="f2135-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2135-130">Type</span></span>|<span data-ttu-id="f2135-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2135-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2135-132">id</span><span class="sxs-lookup"><span data-stu-id="f2135-132">id</span></span>|<span data-ttu-id="f2135-133">String</span><span class="sxs-lookup"><span data-stu-id="f2135-133">String</span></span>|<span data-ttu-id="f2135-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="f2135-134">The GUID for the object</span></span>|
|<span data-ttu-id="f2135-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="f2135-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="f2135-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="f2135-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="f2135-137">Status de atribuição de perfil do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f2135-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="f2135-138">Os valores possíveis são: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="f2135-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="f2135-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="f2135-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="f2135-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="f2135-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="f2135-141">Atribuição de perfil status detalhado do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f2135-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="f2135-142">Os valores possíveis são: `none` e `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="f2135-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="f2135-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2135-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="f2135-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2135-144">DateTimeOffset</span></span>|<span data-ttu-id="f2135-145">Hora do conjunto de perfis do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f2135-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f2135-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2135-146">orderIdentifier</span></span>|<span data-ttu-id="f2135-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2135-147">String</span></span>|<span data-ttu-id="f2135-148">Identificador de pedidos do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f2135-148">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f2135-149">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2135-149">purchaseOrderIdentifier</span></span>|<span data-ttu-id="f2135-150">String</span><span class="sxs-lookup"><span data-stu-id="f2135-150">String</span></span>|<span data-ttu-id="f2135-151">Identificador de ordem de compra do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f2135-151">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f2135-152">serialNumber</span><span class="sxs-lookup"><span data-stu-id="f2135-152">serialNumber</span></span>|<span data-ttu-id="f2135-153">String</span><span class="sxs-lookup"><span data-stu-id="f2135-153">String</span></span>|<span data-ttu-id="f2135-154">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f2135-154">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f2135-155">productKey</span><span class="sxs-lookup"><span data-stu-id="f2135-155">productKey</span></span>|<span data-ttu-id="f2135-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2135-156">String</span></span>|<span data-ttu-id="f2135-157">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f2135-157">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f2135-158">fabricante</span><span class="sxs-lookup"><span data-stu-id="f2135-158">manufacturer</span></span>|<span data-ttu-id="f2135-159">String</span><span class="sxs-lookup"><span data-stu-id="f2135-159">String</span></span>|<span data-ttu-id="f2135-160">Fabricante OEM do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f2135-160">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f2135-161">modelo</span><span class="sxs-lookup"><span data-stu-id="f2135-161">model</span></span>|<span data-ttu-id="f2135-162">String</span><span class="sxs-lookup"><span data-stu-id="f2135-162">String</span></span>|<span data-ttu-id="f2135-163">Nome do modelo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f2135-163">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f2135-164">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="f2135-164">enrollmentState</span></span>|[<span data-ttu-id="f2135-165">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="f2135-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="f2135-166">Estado de registro do Intune do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f2135-166">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="f2135-167">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="f2135-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="f2135-168">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2135-168">lastContactedDateTime</span></span>|<span data-ttu-id="f2135-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2135-169">DateTimeOffset</span></span>|<span data-ttu-id="f2135-170">Data e hora do último contato do Intune para o dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="f2135-170">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f2135-171">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="f2135-171">addressableUserName</span></span>|<span data-ttu-id="f2135-172">String</span><span class="sxs-lookup"><span data-stu-id="f2135-172">String</span></span>|<span data-ttu-id="f2135-173">Nome de usuário endereçável.</span><span class="sxs-lookup"><span data-stu-id="f2135-173">Addressable user name.</span></span>|
|<span data-ttu-id="f2135-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f2135-174">userPrincipalName</span></span>|<span data-ttu-id="f2135-175">String</span><span class="sxs-lookup"><span data-stu-id="f2135-175">String</span></span>|<span data-ttu-id="f2135-176">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="f2135-176">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="f2135-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2135-177">Response</span></span>
<span data-ttu-id="f2135-178">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2135-178">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2135-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2135-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2135-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2135-180">Request</span></span>
<span data-ttu-id="f2135-181">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2135-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="f2135-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2135-182">Response</span></span>
<span data-ttu-id="f2135-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2135-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




