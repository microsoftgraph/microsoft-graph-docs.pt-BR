---
title: Criar importedWindowsAutopilotDeviceIdentity
description: Crie um novo objeto importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 486bdecbbfc425b2f1bcf6458e25677bd79fdb06
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877354"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="e1d7c-103">Criar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="e1d7c-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="e1d7c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1d7c-105">Criar um novo objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="e1d7c-105">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1d7c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1d7c-106">Prerequisites</span></span>
<span data-ttu-id="e1d7c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1d7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1d7c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1d7c-109">Permission type</span></span>|<span data-ttu-id="e1d7c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1d7c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1d7c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1d7c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1d7c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1d7c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e1d7c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1d7c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1d7c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-114">Not supported.</span></span>|
|<span data-ttu-id="e1d7c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1d7c-115">Application</span></span>|<span data-ttu-id="e1d7c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1d7c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1d7c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="e1d7c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1d7c-118">Request headers</span></span>
|<span data-ttu-id="e1d7c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1d7c-119">Header</span></span>|<span data-ttu-id="e1d7c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e1d7c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1d7c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1d7c-121">Authorization</span></span>|<span data-ttu-id="e1d7c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1d7c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1d7c-123">Accept</span></span>|<span data-ttu-id="e1d7c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e1d7c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1d7c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1d7c-125">Request body</span></span>
<span data-ttu-id="e1d7c-126">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="e1d7c-127">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="e1d7c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1d7c-128">Property</span></span>|<span data-ttu-id="e1d7c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1d7c-129">Type</span></span>|<span data-ttu-id="e1d7c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1d7c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1d7c-131">id</span><span class="sxs-lookup"><span data-stu-id="e1d7c-131">id</span></span>|<span data-ttu-id="e1d7c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1d7c-132">String</span></span>|<span data-ttu-id="e1d7c-133">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-133">The GUID for the object</span></span>|
|<span data-ttu-id="e1d7c-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="e1d7c-134">orderIdentifier</span></span>|<span data-ttu-id="e1d7c-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1d7c-135">String</span></span>|<span data-ttu-id="e1d7c-136">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e1d7c-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="e1d7c-137">serialNumber</span></span>|<span data-ttu-id="e1d7c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1d7c-138">String</span></span>|<span data-ttu-id="e1d7c-139">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e1d7c-140">productKey</span><span class="sxs-lookup"><span data-stu-id="e1d7c-140">productKey</span></span>|<span data-ttu-id="e1d7c-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1d7c-141">String</span></span>|<span data-ttu-id="e1d7c-142">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e1d7c-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="e1d7c-143">hardwareIdentifier</span></span>|<span data-ttu-id="e1d7c-144">Binária</span><span class="sxs-lookup"><span data-stu-id="e1d7c-144">Binary</span></span>|<span data-ttu-id="e1d7c-145">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e1d7c-146">state</span><span class="sxs-lookup"><span data-stu-id="e1d7c-146">state</span></span>|[<span data-ttu-id="e1d7c-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="e1d7c-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="e1d7c-148">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="e1d7c-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1d7c-149">Response</span></span>
<span data-ttu-id="e1d7c-150">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-150">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1d7c-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1d7c-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1d7c-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1d7c-152">Request</span></span>
<span data-ttu-id="e1d7c-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="e1d7c-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1d7c-154">Response</span></span>
<span data-ttu-id="e1d7c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1d7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



