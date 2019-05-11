---
title: Atualizar importedWindowsAutopilotDeviceIdentity
description: Atualizar as propriedades de um objeto importedWindowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e073cabe69b9415aae67deaa8b3d482efd12b3cb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908347"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="10947-103">Atualizar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="10947-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="10947-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10947-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10947-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10947-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10947-106">Atualizar as propriedades de um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="10947-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10947-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10947-107">Prerequisites</span></span>
<span data-ttu-id="10947-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10947-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10947-110">Permission type</span></span>|<span data-ttu-id="10947-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10947-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10947-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10947-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10947-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10947-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10947-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10947-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10947-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10947-115">Not supported.</span></span>|
|<span data-ttu-id="10947-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10947-116">Application</span></span>|<span data-ttu-id="10947-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10947-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10947-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10947-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="10947-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10947-119">Request headers</span></span>
|<span data-ttu-id="10947-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10947-120">Header</span></span>|<span data-ttu-id="10947-121">Valor</span><span class="sxs-lookup"><span data-stu-id="10947-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10947-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="10947-122">Authorization</span></span>|<span data-ttu-id="10947-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10947-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10947-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10947-124">Accept</span></span>|<span data-ttu-id="10947-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10947-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10947-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10947-126">Request body</span></span>
<span data-ttu-id="10947-127">No corpo da solicitação, forneça uma representação JSON do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="10947-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="10947-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="10947-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="10947-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10947-129">Property</span></span>|<span data-ttu-id="10947-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="10947-130">Type</span></span>|<span data-ttu-id="10947-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="10947-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10947-132">id</span><span class="sxs-lookup"><span data-stu-id="10947-132">id</span></span>|<span data-ttu-id="10947-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10947-133">String</span></span>|<span data-ttu-id="10947-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="10947-134">The GUID for the object</span></span>|
|<span data-ttu-id="10947-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="10947-135">orderIdentifier</span></span>|<span data-ttu-id="10947-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10947-136">String</span></span>|<span data-ttu-id="10947-137">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="10947-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="10947-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="10947-138">serialNumber</span></span>|<span data-ttu-id="10947-139">String</span><span class="sxs-lookup"><span data-stu-id="10947-139">String</span></span>|<span data-ttu-id="10947-140">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="10947-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="10947-141">productKey</span><span class="sxs-lookup"><span data-stu-id="10947-141">productKey</span></span>|<span data-ttu-id="10947-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10947-142">String</span></span>|<span data-ttu-id="10947-143">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="10947-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="10947-144">importid</span><span class="sxs-lookup"><span data-stu-id="10947-144">importId</span></span>|<span data-ttu-id="10947-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10947-145">String</span></span>|<span data-ttu-id="10947-146">A ID de importação do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="10947-146">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="10947-147">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="10947-147">hardwareIdentifier</span></span>|<span data-ttu-id="10947-148">Binária</span><span class="sxs-lookup"><span data-stu-id="10947-148">Binary</span></span>|<span data-ttu-id="10947-149">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="10947-149">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="10947-150">state</span><span class="sxs-lookup"><span data-stu-id="10947-150">state</span></span>|[<span data-ttu-id="10947-151">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="10947-151">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="10947-152">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="10947-152">Current state of the imported device.</span></span>|
|<span data-ttu-id="10947-153">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="10947-153">assignedUserPrincipalName</span></span>|<span data-ttu-id="10947-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10947-154">String</span></span>|<span data-ttu-id="10947-155">UPN do usuário que o dispositivo será atribuído</span><span class="sxs-lookup"><span data-stu-id="10947-155">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="10947-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="10947-156">Response</span></span>
<span data-ttu-id="10947-157">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [plannerTask](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10947-157">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10947-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10947-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="10947-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10947-159">Request</span></span>
<span data-ttu-id="10947-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10947-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
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

### <a name="response"></a><span data-ttu-id="10947-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="10947-161">Response</span></span>
<span data-ttu-id="10947-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10947-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 694

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
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




