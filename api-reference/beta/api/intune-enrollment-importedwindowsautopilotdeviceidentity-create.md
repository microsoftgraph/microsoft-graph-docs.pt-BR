---
title: Criar importedWindowsAutopilotDeviceIdentity
description: Criar um novo objeto importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7a35693408b214d028af90945e0d3179af83395
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532720"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="6662e-103">Criar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="6662e-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="6662e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6662e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6662e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6662e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6662e-106">Criar um novo objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="6662e-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6662e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6662e-107">Prerequisites</span></span>
<span data-ttu-id="6662e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6662e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6662e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6662e-110">Permission type</span></span>|<span data-ttu-id="6662e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6662e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6662e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6662e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6662e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6662e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6662e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6662e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6662e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6662e-115">Not supported.</span></span>|
|<span data-ttu-id="6662e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6662e-116">Application</span></span>|<span data-ttu-id="6662e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6662e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6662e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6662e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="6662e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6662e-119">Request headers</span></span>
|<span data-ttu-id="6662e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6662e-120">Header</span></span>|<span data-ttu-id="6662e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6662e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6662e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6662e-122">Authorization</span></span>|<span data-ttu-id="6662e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6662e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6662e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6662e-124">Accept</span></span>|<span data-ttu-id="6662e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6662e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6662e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6662e-126">Request body</span></span>
<span data-ttu-id="6662e-127">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="6662e-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="6662e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="6662e-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="6662e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6662e-129">Property</span></span>|<span data-ttu-id="6662e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6662e-130">Type</span></span>|<span data-ttu-id="6662e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6662e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6662e-132">id</span><span class="sxs-lookup"><span data-stu-id="6662e-132">id</span></span>|<span data-ttu-id="6662e-133">String</span><span class="sxs-lookup"><span data-stu-id="6662e-133">String</span></span>|<span data-ttu-id="6662e-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="6662e-134">The GUID for the object</span></span>|
|<span data-ttu-id="6662e-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="6662e-135">orderIdentifier</span></span>|<span data-ttu-id="6662e-136">String</span><span class="sxs-lookup"><span data-stu-id="6662e-136">String</span></span>|<span data-ttu-id="6662e-137">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6662e-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6662e-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="6662e-138">serialNumber</span></span>|<span data-ttu-id="6662e-139">String</span><span class="sxs-lookup"><span data-stu-id="6662e-139">String</span></span>|<span data-ttu-id="6662e-140">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6662e-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6662e-141">productKey</span><span class="sxs-lookup"><span data-stu-id="6662e-141">productKey</span></span>|<span data-ttu-id="6662e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6662e-142">String</span></span>|<span data-ttu-id="6662e-143">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6662e-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6662e-144">importid</span><span class="sxs-lookup"><span data-stu-id="6662e-144">importId</span></span>|<span data-ttu-id="6662e-145">String</span><span class="sxs-lookup"><span data-stu-id="6662e-145">String</span></span>|<span data-ttu-id="6662e-146">A ID de importação do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6662e-146">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6662e-147">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="6662e-147">hardwareIdentifier</span></span>|<span data-ttu-id="6662e-148">Binária</span><span class="sxs-lookup"><span data-stu-id="6662e-148">Binary</span></span>|<span data-ttu-id="6662e-149">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6662e-149">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6662e-150">state</span><span class="sxs-lookup"><span data-stu-id="6662e-150">state</span></span>|[<span data-ttu-id="6662e-151">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="6662e-151">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="6662e-152">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="6662e-152">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="6662e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6662e-153">Response</span></span>
<span data-ttu-id="6662e-154">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6662e-154">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6662e-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6662e-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="6662e-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6662e-156">Request</span></span>
<span data-ttu-id="6662e-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6662e-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 575

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
  }
}
```

### <a name="response"></a><span data-ttu-id="6662e-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="6662e-158">Response</span></span>
<span data-ttu-id="6662e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6662e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 624

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
  }
}
```





