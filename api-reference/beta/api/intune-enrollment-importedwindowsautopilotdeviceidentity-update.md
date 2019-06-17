---
title: Atualizar importedWindowsAutopilotDeviceIdentity
description: Atualizar as propriedades de um objeto importedWindowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8edb384dcac050778d61bb9d6a496f9a8074761a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981675"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="17c70-103">Atualizar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="17c70-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="17c70-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17c70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17c70-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17c70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17c70-106">Atualizar as propriedades de um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="17c70-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17c70-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17c70-107">Prerequisites</span></span>
<span data-ttu-id="17c70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17c70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17c70-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17c70-110">Permission type</span></span>|<span data-ttu-id="17c70-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17c70-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17c70-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17c70-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17c70-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17c70-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="17c70-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17c70-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17c70-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17c70-115">Not supported.</span></span>|
|<span data-ttu-id="17c70-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17c70-116">Application</span></span>|<span data-ttu-id="17c70-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17c70-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17c70-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17c70-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="17c70-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17c70-119">Request headers</span></span>
|<span data-ttu-id="17c70-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17c70-120">Header</span></span>|<span data-ttu-id="17c70-121">Valor</span><span class="sxs-lookup"><span data-stu-id="17c70-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17c70-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="17c70-122">Authorization</span></span>|<span data-ttu-id="17c70-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17c70-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17c70-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17c70-124">Accept</span></span>|<span data-ttu-id="17c70-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17c70-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17c70-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17c70-126">Request body</span></span>
<span data-ttu-id="17c70-127">No corpo da solicitação, forneça uma representação JSON do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="17c70-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="17c70-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="17c70-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="17c70-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17c70-129">Property</span></span>|<span data-ttu-id="17c70-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="17c70-130">Type</span></span>|<span data-ttu-id="17c70-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="17c70-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17c70-132">id</span><span class="sxs-lookup"><span data-stu-id="17c70-132">id</span></span>|<span data-ttu-id="17c70-133">String</span><span class="sxs-lookup"><span data-stu-id="17c70-133">String</span></span>|<span data-ttu-id="17c70-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="17c70-134">The GUID for the object</span></span>|
|<span data-ttu-id="17c70-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="17c70-135">orderIdentifier</span></span>|<span data-ttu-id="17c70-136">String</span><span class="sxs-lookup"><span data-stu-id="17c70-136">String</span></span>|<span data-ttu-id="17c70-137">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="17c70-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="17c70-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="17c70-138">serialNumber</span></span>|<span data-ttu-id="17c70-139">String</span><span class="sxs-lookup"><span data-stu-id="17c70-139">String</span></span>|<span data-ttu-id="17c70-140">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="17c70-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="17c70-141">productKey</span><span class="sxs-lookup"><span data-stu-id="17c70-141">productKey</span></span>|<span data-ttu-id="17c70-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17c70-142">String</span></span>|<span data-ttu-id="17c70-143">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="17c70-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="17c70-144">importid</span><span class="sxs-lookup"><span data-stu-id="17c70-144">importId</span></span>|<span data-ttu-id="17c70-145">String</span><span class="sxs-lookup"><span data-stu-id="17c70-145">String</span></span>|<span data-ttu-id="17c70-146">A ID de importação do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="17c70-146">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="17c70-147">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="17c70-147">hardwareIdentifier</span></span>|<span data-ttu-id="17c70-148">Binária</span><span class="sxs-lookup"><span data-stu-id="17c70-148">Binary</span></span>|<span data-ttu-id="17c70-149">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="17c70-149">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="17c70-150">state</span><span class="sxs-lookup"><span data-stu-id="17c70-150">state</span></span>|[<span data-ttu-id="17c70-151">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="17c70-151">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="17c70-152">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="17c70-152">Current state of the imported device.</span></span>|
|<span data-ttu-id="17c70-153">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="17c70-153">assignedUserPrincipalName</span></span>|<span data-ttu-id="17c70-154">String</span><span class="sxs-lookup"><span data-stu-id="17c70-154">String</span></span>|<span data-ttu-id="17c70-155">UPN do usuário que o dispositivo será atribuído</span><span class="sxs-lookup"><span data-stu-id="17c70-155">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="17c70-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="17c70-156">Response</span></span>
<span data-ttu-id="17c70-157">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [plannerTask](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17c70-157">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17c70-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17c70-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="17c70-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17c70-159">Request</span></span>
<span data-ttu-id="17c70-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17c70-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="17c70-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="17c70-161">Response</span></span>
<span data-ttu-id="17c70-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17c70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





