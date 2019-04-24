---
title: Atualizar importedWindowsAutopilotDeviceIdentity
description: Atualizar as propriedades de um objeto importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a8668fa78c5996b2d33af18e7cbd23a03df1200
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459707"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="cf818-103">Atualizar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="cf818-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="cf818-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf818-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf818-105">Atualizar as propriedades de um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="cf818-105">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf818-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf818-106">Prerequisites</span></span>
<span data-ttu-id="cf818-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf818-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf818-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf818-109">Permission type</span></span>|<span data-ttu-id="cf818-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf818-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf818-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf818-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf818-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf818-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cf818-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf818-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf818-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf818-114">Not supported.</span></span>|
|<span data-ttu-id="cf818-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf818-115">Application</span></span>|<span data-ttu-id="cf818-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf818-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf818-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf818-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="cf818-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf818-118">Request headers</span></span>
|<span data-ttu-id="cf818-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf818-119">Header</span></span>|<span data-ttu-id="cf818-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cf818-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf818-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf818-121">Authorization</span></span>|<span data-ttu-id="cf818-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf818-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf818-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf818-123">Accept</span></span>|<span data-ttu-id="cf818-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cf818-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf818-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf818-125">Request body</span></span>
<span data-ttu-id="cf818-126">No corpo da solicitação, forneça uma representação JSON do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="cf818-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="cf818-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="cf818-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="cf818-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf818-128">Property</span></span>|<span data-ttu-id="cf818-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf818-129">Type</span></span>|<span data-ttu-id="cf818-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf818-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf818-131">id</span><span class="sxs-lookup"><span data-stu-id="cf818-131">id</span></span>|<span data-ttu-id="cf818-132">String</span><span class="sxs-lookup"><span data-stu-id="cf818-132">String</span></span>|<span data-ttu-id="cf818-133">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="cf818-133">The GUID for the object</span></span>|
|<span data-ttu-id="cf818-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="cf818-134">orderIdentifier</span></span>|<span data-ttu-id="cf818-135">String</span><span class="sxs-lookup"><span data-stu-id="cf818-135">String</span></span>|<span data-ttu-id="cf818-136">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="cf818-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="cf818-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="cf818-137">serialNumber</span></span>|<span data-ttu-id="cf818-138">String</span><span class="sxs-lookup"><span data-stu-id="cf818-138">String</span></span>|<span data-ttu-id="cf818-139">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="cf818-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="cf818-140">productKey</span><span class="sxs-lookup"><span data-stu-id="cf818-140">productKey</span></span>|<span data-ttu-id="cf818-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf818-141">String</span></span>|<span data-ttu-id="cf818-142">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="cf818-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="cf818-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="cf818-143">hardwareIdentifier</span></span>|<span data-ttu-id="cf818-144">Binária</span><span class="sxs-lookup"><span data-stu-id="cf818-144">Binary</span></span>|<span data-ttu-id="cf818-145">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="cf818-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="cf818-146">state</span><span class="sxs-lookup"><span data-stu-id="cf818-146">state</span></span>|[<span data-ttu-id="cf818-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="cf818-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="cf818-148">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="cf818-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="cf818-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf818-149">Response</span></span>
<span data-ttu-id="cf818-150">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [plannerTask](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf818-150">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf818-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf818-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf818-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf818-152">Request</span></span>
<span data-ttu-id="cf818-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf818-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cf818-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf818-154">Response</span></span>
<span data-ttu-id="cf818-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf818-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



