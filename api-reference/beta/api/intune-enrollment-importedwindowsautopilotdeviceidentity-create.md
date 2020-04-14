---
title: Criar importedWindowsAutopilotDeviceIdentity
description: Criar um novo objeto importedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ef21ddb7f3d392bd833f7396a8c29b9cd92dbe1d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452592"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="58bfb-103">Criar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="58bfb-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="58bfb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58bfb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58bfb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58bfb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58bfb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58bfb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58bfb-107">Criar um novo objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="58bfb-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58bfb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58bfb-108">Prerequisites</span></span>
<span data-ttu-id="58bfb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58bfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58bfb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58bfb-111">Permission type</span></span>|<span data-ttu-id="58bfb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58bfb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58bfb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58bfb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58bfb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58bfb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="58bfb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58bfb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58bfb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58bfb-116">Not supported.</span></span>|
|<span data-ttu-id="58bfb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58bfb-117">Application</span></span>|<span data-ttu-id="58bfb-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58bfb-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58bfb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58bfb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="58bfb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58bfb-120">Request headers</span></span>
|<span data-ttu-id="58bfb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58bfb-121">Header</span></span>|<span data-ttu-id="58bfb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="58bfb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58bfb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="58bfb-123">Authorization</span></span>|<span data-ttu-id="58bfb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58bfb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58bfb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58bfb-125">Accept</span></span>|<span data-ttu-id="58bfb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58bfb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58bfb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58bfb-127">Request body</span></span>
<span data-ttu-id="58bfb-128">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="58bfb-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="58bfb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="58bfb-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="58bfb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58bfb-130">Property</span></span>|<span data-ttu-id="58bfb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="58bfb-131">Type</span></span>|<span data-ttu-id="58bfb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="58bfb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58bfb-133">id</span><span class="sxs-lookup"><span data-stu-id="58bfb-133">id</span></span>|<span data-ttu-id="58bfb-134">String</span><span class="sxs-lookup"><span data-stu-id="58bfb-134">String</span></span>|<span data-ttu-id="58bfb-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="58bfb-135">The GUID for the object</span></span>|
|<span data-ttu-id="58bfb-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="58bfb-136">orderIdentifier</span></span>|<span data-ttu-id="58bfb-137">String</span><span class="sxs-lookup"><span data-stu-id="58bfb-137">String</span></span>|<span data-ttu-id="58bfb-138">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="58bfb-138">Order Id of the Windows autopilot device.</span></span> <span data-ttu-id="58bfb-139">– Substituir</span><span class="sxs-lookup"><span data-stu-id="58bfb-139">- Deprecate</span></span>|
|<span data-ttu-id="58bfb-140">groupTag</span><span class="sxs-lookup"><span data-stu-id="58bfb-140">groupTag</span></span>|<span data-ttu-id="58bfb-141">String</span><span class="sxs-lookup"><span data-stu-id="58bfb-141">String</span></span>|<span data-ttu-id="58bfb-142">Marca de grupo do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="58bfb-142">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58bfb-143">serialNumber</span><span class="sxs-lookup"><span data-stu-id="58bfb-143">serialNumber</span></span>|<span data-ttu-id="58bfb-144">String</span><span class="sxs-lookup"><span data-stu-id="58bfb-144">String</span></span>|<span data-ttu-id="58bfb-145">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="58bfb-145">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58bfb-146">productKey</span><span class="sxs-lookup"><span data-stu-id="58bfb-146">productKey</span></span>|<span data-ttu-id="58bfb-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58bfb-147">String</span></span>|<span data-ttu-id="58bfb-148">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="58bfb-148">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58bfb-149">importid</span><span class="sxs-lookup"><span data-stu-id="58bfb-149">importId</span></span>|<span data-ttu-id="58bfb-150">String</span><span class="sxs-lookup"><span data-stu-id="58bfb-150">String</span></span>|<span data-ttu-id="58bfb-151">A ID de importação do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="58bfb-151">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58bfb-152">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="58bfb-152">hardwareIdentifier</span></span>|<span data-ttu-id="58bfb-153">Binária</span><span class="sxs-lookup"><span data-stu-id="58bfb-153">Binary</span></span>|<span data-ttu-id="58bfb-154">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="58bfb-154">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="58bfb-155">state</span><span class="sxs-lookup"><span data-stu-id="58bfb-155">state</span></span>|[<span data-ttu-id="58bfb-156">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="58bfb-156">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="58bfb-157">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="58bfb-157">Current state of the imported device.</span></span>|
|<span data-ttu-id="58bfb-158">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="58bfb-158">assignedUserPrincipalName</span></span>|<span data-ttu-id="58bfb-159">String</span><span class="sxs-lookup"><span data-stu-id="58bfb-159">String</span></span>|<span data-ttu-id="58bfb-160">UPN do usuário que o dispositivo será atribuído</span><span class="sxs-lookup"><span data-stu-id="58bfb-160">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="58bfb-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="58bfb-161">Response</span></span>
<span data-ttu-id="58bfb-162">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58bfb-162">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58bfb-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58bfb-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="58bfb-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58bfb-164">Request</span></span>
<span data-ttu-id="58bfb-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58bfb-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58bfb-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="58bfb-166">Response</span></span>
<span data-ttu-id="58bfb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58bfb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



