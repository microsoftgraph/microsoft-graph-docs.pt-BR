---
title: Criar importedWindowsAutopilotDeviceIdentity
description: Criar um novo objeto importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 664b0d52eea5d61918e234c9fa582fa57f50d8b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565853"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="09d84-103">Criar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="09d84-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="09d84-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09d84-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09d84-105">Criar um novo objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="09d84-105">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09d84-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="09d84-106">Prerequisites</span></span>
<span data-ttu-id="09d84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09d84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09d84-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09d84-109">Permission type</span></span>|<span data-ttu-id="09d84-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="09d84-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09d84-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09d84-111">Delegated (work or school account)</span></span>|<span data-ttu-id="09d84-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09d84-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="09d84-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09d84-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09d84-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09d84-114">Not supported.</span></span>|
|<span data-ttu-id="09d84-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09d84-115">Application</span></span>|<span data-ttu-id="09d84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09d84-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09d84-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09d84-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="09d84-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09d84-118">Request headers</span></span>
|<span data-ttu-id="09d84-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09d84-119">Header</span></span>|<span data-ttu-id="09d84-120">Valor</span><span class="sxs-lookup"><span data-stu-id="09d84-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09d84-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="09d84-121">Authorization</span></span>|<span data-ttu-id="09d84-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09d84-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09d84-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09d84-123">Accept</span></span>|<span data-ttu-id="09d84-124">application/json</span><span class="sxs-lookup"><span data-stu-id="09d84-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09d84-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09d84-125">Request body</span></span>
<span data-ttu-id="09d84-126">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="09d84-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="09d84-127">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="09d84-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="09d84-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09d84-128">Property</span></span>|<span data-ttu-id="09d84-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="09d84-129">Type</span></span>|<span data-ttu-id="09d84-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="09d84-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09d84-131">id</span><span class="sxs-lookup"><span data-stu-id="09d84-131">id</span></span>|<span data-ttu-id="09d84-132">String</span><span class="sxs-lookup"><span data-stu-id="09d84-132">String</span></span>|<span data-ttu-id="09d84-133">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="09d84-133">The GUID for the object</span></span>|
|<span data-ttu-id="09d84-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="09d84-134">orderIdentifier</span></span>|<span data-ttu-id="09d84-135">String</span><span class="sxs-lookup"><span data-stu-id="09d84-135">String</span></span>|<span data-ttu-id="09d84-136">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="09d84-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="09d84-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="09d84-137">serialNumber</span></span>|<span data-ttu-id="09d84-138">String</span><span class="sxs-lookup"><span data-stu-id="09d84-138">String</span></span>|<span data-ttu-id="09d84-139">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="09d84-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="09d84-140">productKey</span><span class="sxs-lookup"><span data-stu-id="09d84-140">productKey</span></span>|<span data-ttu-id="09d84-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09d84-141">String</span></span>|<span data-ttu-id="09d84-142">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="09d84-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="09d84-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="09d84-143">hardwareIdentifier</span></span>|<span data-ttu-id="09d84-144">Binária</span><span class="sxs-lookup"><span data-stu-id="09d84-144">Binary</span></span>|<span data-ttu-id="09d84-145">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="09d84-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="09d84-146">state</span><span class="sxs-lookup"><span data-stu-id="09d84-146">state</span></span>|[<span data-ttu-id="09d84-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="09d84-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="09d84-148">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="09d84-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="09d84-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d84-149">Response</span></span>
<span data-ttu-id="09d84-150">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09d84-150">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09d84-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09d84-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="09d84-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09d84-152">Request</span></span>
<span data-ttu-id="09d84-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09d84-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="09d84-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d84-154">Response</span></span>
<span data-ttu-id="09d84-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09d84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



