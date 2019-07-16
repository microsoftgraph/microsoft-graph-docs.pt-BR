---
title: Atualizar importedWindowsAutopilotDeviceIdentity
description: Atualizar as propriedades de um objeto importedWindowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 45665498ceb3b1ec52fa7f56bb3e4abd6013cae5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729989"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="02477-103">Atualizar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="02477-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="02477-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02477-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02477-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02477-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02477-106">Atualizar as propriedades de um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="02477-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02477-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02477-107">Prerequisites</span></span>
<span data-ttu-id="02477-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02477-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02477-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02477-110">Permission type</span></span>|<span data-ttu-id="02477-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02477-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02477-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02477-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02477-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02477-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="02477-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02477-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02477-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02477-115">Not supported.</span></span>|
|<span data-ttu-id="02477-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02477-116">Application</span></span>|<span data-ttu-id="02477-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02477-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02477-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02477-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="02477-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02477-119">Request headers</span></span>
|<span data-ttu-id="02477-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02477-120">Header</span></span>|<span data-ttu-id="02477-121">Valor</span><span class="sxs-lookup"><span data-stu-id="02477-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02477-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02477-122">Authorization</span></span>|<span data-ttu-id="02477-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02477-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02477-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02477-124">Accept</span></span>|<span data-ttu-id="02477-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02477-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02477-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02477-126">Request body</span></span>
<span data-ttu-id="02477-127">No corpo da solicitação, forneça uma representação JSON do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="02477-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="02477-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="02477-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="02477-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02477-129">Property</span></span>|<span data-ttu-id="02477-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="02477-130">Type</span></span>|<span data-ttu-id="02477-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="02477-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02477-132">id</span><span class="sxs-lookup"><span data-stu-id="02477-132">id</span></span>|<span data-ttu-id="02477-133">String</span><span class="sxs-lookup"><span data-stu-id="02477-133">String</span></span>|<span data-ttu-id="02477-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="02477-134">The GUID for the object</span></span>|
|<span data-ttu-id="02477-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="02477-135">orderIdentifier</span></span>|<span data-ttu-id="02477-136">String</span><span class="sxs-lookup"><span data-stu-id="02477-136">String</span></span>|<span data-ttu-id="02477-137">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="02477-137">Order Id of the Windows autopilot device.</span></span> <span data-ttu-id="02477-138">– Substituir</span><span class="sxs-lookup"><span data-stu-id="02477-138">- Deprecate</span></span>|
|<span data-ttu-id="02477-139">groupTag</span><span class="sxs-lookup"><span data-stu-id="02477-139">groupTag</span></span>|<span data-ttu-id="02477-140">String</span><span class="sxs-lookup"><span data-stu-id="02477-140">String</span></span>|<span data-ttu-id="02477-141">Marca de grupo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="02477-141">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="02477-142">serialNumber</span><span class="sxs-lookup"><span data-stu-id="02477-142">serialNumber</span></span>|<span data-ttu-id="02477-143">String</span><span class="sxs-lookup"><span data-stu-id="02477-143">String</span></span>|<span data-ttu-id="02477-144">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="02477-144">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="02477-145">productKey</span><span class="sxs-lookup"><span data-stu-id="02477-145">productKey</span></span>|<span data-ttu-id="02477-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02477-146">String</span></span>|<span data-ttu-id="02477-147">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="02477-147">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="02477-148">importid</span><span class="sxs-lookup"><span data-stu-id="02477-148">importId</span></span>|<span data-ttu-id="02477-149">String</span><span class="sxs-lookup"><span data-stu-id="02477-149">String</span></span>|<span data-ttu-id="02477-150">A ID de importação do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="02477-150">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="02477-151">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="02477-151">hardwareIdentifier</span></span>|<span data-ttu-id="02477-152">Binária</span><span class="sxs-lookup"><span data-stu-id="02477-152">Binary</span></span>|<span data-ttu-id="02477-153">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="02477-153">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="02477-154">state</span><span class="sxs-lookup"><span data-stu-id="02477-154">state</span></span>|[<span data-ttu-id="02477-155">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="02477-155">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="02477-156">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="02477-156">Current state of the imported device.</span></span>|
|<span data-ttu-id="02477-157">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="02477-157">assignedUserPrincipalName</span></span>|<span data-ttu-id="02477-158">String</span><span class="sxs-lookup"><span data-stu-id="02477-158">String</span></span>|<span data-ttu-id="02477-159">UPN do usuário que o dispositivo será atribuído</span><span class="sxs-lookup"><span data-stu-id="02477-159">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="02477-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="02477-160">Response</span></span>
<span data-ttu-id="02477-161">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [plannerTask](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02477-161">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02477-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02477-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="02477-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02477-163">Request</span></span>
<span data-ttu-id="02477-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02477-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 679

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "importId": "Import Id value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  },
  "assignedUserPrincipalName": "Assigned User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="02477-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="02477-165">Response</span></span>
<span data-ttu-id="02477-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02477-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 728

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "importId": "Import Id value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  },
  "assignedUserPrincipalName": "Assigned User Principal Name value"
}
```





