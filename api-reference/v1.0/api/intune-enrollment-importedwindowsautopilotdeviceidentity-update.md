---
title: Atualizar importedWindowsAutopilotDeviceIdentity
description: Atualizar as propriedades de um objeto importedWindowsAutopilotDeviceIdentity.
ms.openlocfilehash: ec784e6f0032e0167c9b9339d65568d923ee3c74
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007135"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="72796-103">Atualizar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="72796-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="72796-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="72796-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72796-105">Atualizar as propriedades de um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="72796-105">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72796-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72796-106">Prerequisites</span></span>
<span data-ttu-id="72796-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72796-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72796-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72796-109">Permission type</span></span>|<span data-ttu-id="72796-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72796-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72796-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72796-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72796-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72796-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="72796-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72796-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72796-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72796-114">Not supported.</span></span>|
|<span data-ttu-id="72796-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72796-115">Application</span></span>|<span data-ttu-id="72796-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72796-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72796-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72796-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="72796-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72796-118">Request headers</span></span>
|<span data-ttu-id="72796-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72796-119">Header</span></span>|<span data-ttu-id="72796-120">Valor</span><span class="sxs-lookup"><span data-stu-id="72796-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72796-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="72796-121">Authorization</span></span>|<span data-ttu-id="72796-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72796-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72796-123">Accept</span><span class="sxs-lookup"><span data-stu-id="72796-123">Accept</span></span>|<span data-ttu-id="72796-124">application/json</span><span class="sxs-lookup"><span data-stu-id="72796-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72796-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72796-125">Request body</span></span>
<span data-ttu-id="72796-126">No corpo da solicitação, forneça uma representação JSON do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="72796-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="72796-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="72796-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="72796-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72796-128">Property</span></span>|<span data-ttu-id="72796-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="72796-129">Type</span></span>|<span data-ttu-id="72796-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="72796-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72796-131">id</span><span class="sxs-lookup"><span data-stu-id="72796-131">id</span></span>|<span data-ttu-id="72796-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72796-132">String</span></span>|<span data-ttu-id="72796-133">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="72796-133">The GUID for the object</span></span>|
|<span data-ttu-id="72796-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="72796-134">orderIdentifier</span></span>|<span data-ttu-id="72796-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72796-135">String</span></span>|<span data-ttu-id="72796-136">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="72796-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="72796-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="72796-137">serialNumber</span></span>|<span data-ttu-id="72796-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72796-138">String</span></span>|<span data-ttu-id="72796-139">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="72796-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="72796-140">productKey</span><span class="sxs-lookup"><span data-stu-id="72796-140">productKey</span></span>|<span data-ttu-id="72796-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72796-141">String</span></span>|<span data-ttu-id="72796-142">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="72796-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="72796-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="72796-143">hardwareIdentifier</span></span>|<span data-ttu-id="72796-144">Binária</span><span class="sxs-lookup"><span data-stu-id="72796-144">Binary</span></span>|<span data-ttu-id="72796-145">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="72796-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="72796-146">state</span><span class="sxs-lookup"><span data-stu-id="72796-146">state</span></span>|[<span data-ttu-id="72796-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="72796-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="72796-148">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="72796-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="72796-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="72796-149">Response</span></span>
<span data-ttu-id="72796-150">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [plannerTask](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72796-150">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72796-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72796-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="72796-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72796-152">Request</span></span>
<span data-ttu-id="72796-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72796-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 541

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```

### <a name="response"></a><span data-ttu-id="72796-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="72796-154">Response</span></span>
<span data-ttu-id="72796-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72796-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```



