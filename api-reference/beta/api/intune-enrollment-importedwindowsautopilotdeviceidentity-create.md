---
title: Criar importedWindowsAutopilotDeviceIdentity
description: Criar um novo objeto importedWindowsAutopilotDeviceIdentity.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: daf692eed70a67fa447c0787e8c77020c4d4c04a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42805119"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="6413e-103">Criar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="6413e-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="6413e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6413e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6413e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6413e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6413e-106">Criar um novo objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="6413e-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6413e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6413e-107">Prerequisites</span></span>
<span data-ttu-id="6413e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6413e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6413e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6413e-110">Permission type</span></span>|<span data-ttu-id="6413e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6413e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6413e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6413e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6413e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6413e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6413e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6413e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6413e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6413e-115">Not supported.</span></span>|
|<span data-ttu-id="6413e-116">Application</span><span class="sxs-lookup"><span data-stu-id="6413e-116">Application</span></span>|<span data-ttu-id="6413e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6413e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6413e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6413e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="6413e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6413e-119">Request headers</span></span>
|<span data-ttu-id="6413e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6413e-120">Header</span></span>|<span data-ttu-id="6413e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6413e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6413e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6413e-122">Authorization</span></span>|<span data-ttu-id="6413e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6413e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6413e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6413e-124">Accept</span></span>|<span data-ttu-id="6413e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6413e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6413e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6413e-126">Request body</span></span>
<span data-ttu-id="6413e-127">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="6413e-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="6413e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="6413e-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="6413e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6413e-129">Property</span></span>|<span data-ttu-id="6413e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6413e-130">Type</span></span>|<span data-ttu-id="6413e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6413e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6413e-132">id</span><span class="sxs-lookup"><span data-stu-id="6413e-132">id</span></span>|<span data-ttu-id="6413e-133">String</span><span class="sxs-lookup"><span data-stu-id="6413e-133">String</span></span>|<span data-ttu-id="6413e-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="6413e-134">The GUID for the object</span></span>|
|<span data-ttu-id="6413e-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="6413e-135">orderIdentifier</span></span>|<span data-ttu-id="6413e-136">String</span><span class="sxs-lookup"><span data-stu-id="6413e-136">String</span></span>|<span data-ttu-id="6413e-137">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6413e-137">Order Id of the Windows autopilot device.</span></span> <span data-ttu-id="6413e-138">– Substituir</span><span class="sxs-lookup"><span data-stu-id="6413e-138">- Deprecate</span></span>|
|<span data-ttu-id="6413e-139">groupTag</span><span class="sxs-lookup"><span data-stu-id="6413e-139">groupTag</span></span>|<span data-ttu-id="6413e-140">String</span><span class="sxs-lookup"><span data-stu-id="6413e-140">String</span></span>|<span data-ttu-id="6413e-141">Marca de grupo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6413e-141">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6413e-142">serialNumber</span><span class="sxs-lookup"><span data-stu-id="6413e-142">serialNumber</span></span>|<span data-ttu-id="6413e-143">String</span><span class="sxs-lookup"><span data-stu-id="6413e-143">String</span></span>|<span data-ttu-id="6413e-144">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6413e-144">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6413e-145">productKey</span><span class="sxs-lookup"><span data-stu-id="6413e-145">productKey</span></span>|<span data-ttu-id="6413e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6413e-146">String</span></span>|<span data-ttu-id="6413e-147">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6413e-147">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6413e-148">importid</span><span class="sxs-lookup"><span data-stu-id="6413e-148">importId</span></span>|<span data-ttu-id="6413e-149">String</span><span class="sxs-lookup"><span data-stu-id="6413e-149">String</span></span>|<span data-ttu-id="6413e-150">A ID de importação do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6413e-150">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6413e-151">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="6413e-151">hardwareIdentifier</span></span>|<span data-ttu-id="6413e-152">Binária</span><span class="sxs-lookup"><span data-stu-id="6413e-152">Binary</span></span>|<span data-ttu-id="6413e-153">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6413e-153">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6413e-154">state</span><span class="sxs-lookup"><span data-stu-id="6413e-154">state</span></span>|[<span data-ttu-id="6413e-155">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="6413e-155">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="6413e-156">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="6413e-156">Current state of the imported device.</span></span>|
|<span data-ttu-id="6413e-157">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6413e-157">assignedUserPrincipalName</span></span>|<span data-ttu-id="6413e-158">String</span><span class="sxs-lookup"><span data-stu-id="6413e-158">String</span></span>|<span data-ttu-id="6413e-159">UPN do usuário que o dispositivo será atribuído</span><span class="sxs-lookup"><span data-stu-id="6413e-159">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="6413e-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="6413e-160">Response</span></span>
<span data-ttu-id="6413e-161">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6413e-161">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6413e-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6413e-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="6413e-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6413e-163">Request</span></span>
<span data-ttu-id="6413e-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6413e-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="6413e-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="6413e-165">Response</span></span>
<span data-ttu-id="6413e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6413e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




