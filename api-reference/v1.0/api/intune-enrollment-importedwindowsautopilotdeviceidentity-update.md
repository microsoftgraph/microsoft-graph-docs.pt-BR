---
title: Atualizar importedWindowsAutopilotDeviceIdentity
description: Atualizar as propriedades de um objeto importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4ac55088b70b31057b026e16263995c9c37b858f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020861"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="d095e-103">Atualizar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d095e-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="d095e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d095e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d095e-105">Atualizar as propriedades de um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d095e-105">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d095e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d095e-106">Prerequisites</span></span>
<span data-ttu-id="d095e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d095e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d095e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d095e-109">Permission type</span></span>|<span data-ttu-id="d095e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d095e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d095e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d095e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d095e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d095e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d095e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d095e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d095e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d095e-114">Not supported.</span></span>|
|<span data-ttu-id="d095e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d095e-115">Application</span></span>|<span data-ttu-id="d095e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d095e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d095e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d095e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="d095e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d095e-118">Request headers</span></span>
|<span data-ttu-id="d095e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d095e-119">Header</span></span>|<span data-ttu-id="d095e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d095e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d095e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d095e-121">Authorization</span></span>|<span data-ttu-id="d095e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d095e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d095e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d095e-123">Accept</span></span>|<span data-ttu-id="d095e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d095e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d095e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d095e-125">Request body</span></span>
<span data-ttu-id="d095e-126">No corpo da solicitação, forneça uma representação JSON do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d095e-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="d095e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d095e-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="d095e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d095e-128">Property</span></span>|<span data-ttu-id="d095e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d095e-129">Type</span></span>|<span data-ttu-id="d095e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d095e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d095e-131">id</span><span class="sxs-lookup"><span data-stu-id="d095e-131">id</span></span>|<span data-ttu-id="d095e-132">String</span><span class="sxs-lookup"><span data-stu-id="d095e-132">String</span></span>|<span data-ttu-id="d095e-133">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="d095e-133">The GUID for the object</span></span>|
|<span data-ttu-id="d095e-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="d095e-134">orderIdentifier</span></span>|<span data-ttu-id="d095e-135">String</span><span class="sxs-lookup"><span data-stu-id="d095e-135">String</span></span>|<span data-ttu-id="d095e-136">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="d095e-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d095e-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d095e-137">serialNumber</span></span>|<span data-ttu-id="d095e-138">String</span><span class="sxs-lookup"><span data-stu-id="d095e-138">String</span></span>|<span data-ttu-id="d095e-139">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="d095e-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d095e-140">productKey</span><span class="sxs-lookup"><span data-stu-id="d095e-140">productKey</span></span>|<span data-ttu-id="d095e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d095e-141">String</span></span>|<span data-ttu-id="d095e-142">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="d095e-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d095e-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="d095e-143">hardwareIdentifier</span></span>|<span data-ttu-id="d095e-144">Binária</span><span class="sxs-lookup"><span data-stu-id="d095e-144">Binary</span></span>|<span data-ttu-id="d095e-145">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="d095e-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d095e-146">state</span><span class="sxs-lookup"><span data-stu-id="d095e-146">state</span></span>|[<span data-ttu-id="d095e-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="d095e-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="d095e-148">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="d095e-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="d095e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d095e-149">Response</span></span>
<span data-ttu-id="d095e-150">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [plannerTask](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d095e-150">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d095e-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d095e-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="d095e-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d095e-152">Request</span></span>
<span data-ttu-id="d095e-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d095e-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d095e-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d095e-154">Response</span></span>
<span data-ttu-id="d095e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d095e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



