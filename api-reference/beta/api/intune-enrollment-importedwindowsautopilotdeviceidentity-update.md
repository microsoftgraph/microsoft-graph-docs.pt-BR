---
title: Atualizar importedWindowsAutopilotDeviceIdentity
description: Atualizar as propriedades de um objeto importedWindowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86d767375059ae774080151a8cc22b9a0640f30c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943758"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="a73b0-103">Atualizar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a73b0-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="a73b0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a73b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a73b0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a73b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a73b0-106">Atualizar as propriedades de um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="a73b0-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a73b0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a73b0-107">Prerequisites</span></span>
<span data-ttu-id="a73b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a73b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a73b0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a73b0-110">Permission type</span></span>|<span data-ttu-id="a73b0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a73b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a73b0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a73b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a73b0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a73b0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a73b0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a73b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a73b0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a73b0-115">Not supported.</span></span>|
|<span data-ttu-id="a73b0-116">Application</span><span class="sxs-lookup"><span data-stu-id="a73b0-116">Application</span></span>|<span data-ttu-id="a73b0-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a73b0-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a73b0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a73b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="a73b0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a73b0-119">Request headers</span></span>
|<span data-ttu-id="a73b0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a73b0-120">Header</span></span>|<span data-ttu-id="a73b0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a73b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a73b0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a73b0-122">Authorization</span></span>|<span data-ttu-id="a73b0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a73b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a73b0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a73b0-124">Accept</span></span>|<span data-ttu-id="a73b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a73b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a73b0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a73b0-126">Request body</span></span>
<span data-ttu-id="a73b0-127">No corpo da solicitação, forneça uma representação JSON do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="a73b0-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="a73b0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="a73b0-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="a73b0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a73b0-129">Property</span></span>|<span data-ttu-id="a73b0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a73b0-130">Type</span></span>|<span data-ttu-id="a73b0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a73b0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a73b0-132">id</span><span class="sxs-lookup"><span data-stu-id="a73b0-132">id</span></span>|<span data-ttu-id="a73b0-133">String</span><span class="sxs-lookup"><span data-stu-id="a73b0-133">String</span></span>|<span data-ttu-id="a73b0-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="a73b0-134">The GUID for the object</span></span>|
|<span data-ttu-id="a73b0-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="a73b0-135">orderIdentifier</span></span>|<span data-ttu-id="a73b0-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a73b0-136">String</span></span>|<span data-ttu-id="a73b0-137">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="a73b0-137">Order Id of the Windows autopilot device.</span></span> <span data-ttu-id="a73b0-138">– Substituir</span><span class="sxs-lookup"><span data-stu-id="a73b0-138">- Deprecate</span></span>|
|<span data-ttu-id="a73b0-139">groupTag</span><span class="sxs-lookup"><span data-stu-id="a73b0-139">groupTag</span></span>|<span data-ttu-id="a73b0-140">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a73b0-140">String</span></span>|<span data-ttu-id="a73b0-141">Marca de grupo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="a73b0-141">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a73b0-142">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a73b0-142">serialNumber</span></span>|<span data-ttu-id="a73b0-143">String</span><span class="sxs-lookup"><span data-stu-id="a73b0-143">String</span></span>|<span data-ttu-id="a73b0-144">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="a73b0-144">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a73b0-145">productKey</span><span class="sxs-lookup"><span data-stu-id="a73b0-145">productKey</span></span>|<span data-ttu-id="a73b0-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a73b0-146">String</span></span>|<span data-ttu-id="a73b0-147">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="a73b0-147">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a73b0-148">importid</span><span class="sxs-lookup"><span data-stu-id="a73b0-148">importId</span></span>|<span data-ttu-id="a73b0-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a73b0-149">String</span></span>|<span data-ttu-id="a73b0-150">A ID de importação do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="a73b0-150">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a73b0-151">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="a73b0-151">hardwareIdentifier</span></span>|<span data-ttu-id="a73b0-152">Binária</span><span class="sxs-lookup"><span data-stu-id="a73b0-152">Binary</span></span>|<span data-ttu-id="a73b0-153">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="a73b0-153">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a73b0-154">state</span><span class="sxs-lookup"><span data-stu-id="a73b0-154">state</span></span>|[<span data-ttu-id="a73b0-155">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="a73b0-155">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="a73b0-156">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="a73b0-156">Current state of the imported device.</span></span>|
|<span data-ttu-id="a73b0-157">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a73b0-157">assignedUserPrincipalName</span></span>|<span data-ttu-id="a73b0-158">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a73b0-158">String</span></span>|<span data-ttu-id="a73b0-159">UPN do usuário que o dispositivo será atribuído</span><span class="sxs-lookup"><span data-stu-id="a73b0-159">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="a73b0-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="a73b0-160">Response</span></span>
<span data-ttu-id="a73b0-161">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [plannerTask](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a73b0-161">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a73b0-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a73b0-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="a73b0-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a73b0-163">Request</span></span>
<span data-ttu-id="a73b0-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a73b0-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a73b0-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="a73b0-165">Response</span></span>
<span data-ttu-id="a73b0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a73b0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





