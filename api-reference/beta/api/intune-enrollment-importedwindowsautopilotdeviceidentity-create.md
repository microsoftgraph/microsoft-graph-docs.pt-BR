---
title: Criar importedWindowsAutopilotDeviceIdentity
description: Criar um novo objeto importedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c39fed44dd8d4d7f0516f2215534ed861e13ec4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149860"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="655ae-103">Criar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="655ae-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="655ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="655ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="655ae-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="655ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="655ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="655ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="655ae-107">Criar um novo objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="655ae-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="655ae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="655ae-108">Prerequisites</span></span>
<span data-ttu-id="655ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="655ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="655ae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="655ae-111">Permission type</span></span>|<span data-ttu-id="655ae-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="655ae-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="655ae-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="655ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="655ae-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="655ae-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="655ae-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="655ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="655ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="655ae-116">Not supported.</span></span>|
|<span data-ttu-id="655ae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="655ae-117">Application</span></span>|<span data-ttu-id="655ae-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="655ae-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="655ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="655ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="655ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="655ae-120">Request headers</span></span>
|<span data-ttu-id="655ae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="655ae-121">Header</span></span>|<span data-ttu-id="655ae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="655ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="655ae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="655ae-123">Authorization</span></span>|<span data-ttu-id="655ae-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="655ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="655ae-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="655ae-125">Accept</span></span>|<span data-ttu-id="655ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="655ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="655ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="655ae-127">Request body</span></span>
<span data-ttu-id="655ae-128">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="655ae-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="655ae-129">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="655ae-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="655ae-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="655ae-130">Property</span></span>|<span data-ttu-id="655ae-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="655ae-131">Type</span></span>|<span data-ttu-id="655ae-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="655ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="655ae-133">id</span><span class="sxs-lookup"><span data-stu-id="655ae-133">id</span></span>|<span data-ttu-id="655ae-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="655ae-134">String</span></span>|<span data-ttu-id="655ae-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="655ae-135">The GUID for the object</span></span>|
|<span data-ttu-id="655ae-136">groupTag</span><span class="sxs-lookup"><span data-stu-id="655ae-136">groupTag</span></span>|<span data-ttu-id="655ae-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="655ae-137">String</span></span>|<span data-ttu-id="655ae-138">Marca de grupo do dispositivo de piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="655ae-138">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="655ae-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="655ae-139">serialNumber</span></span>|<span data-ttu-id="655ae-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="655ae-140">String</span></span>|<span data-ttu-id="655ae-141">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="655ae-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="655ae-142">productKey</span><span class="sxs-lookup"><span data-stu-id="655ae-142">productKey</span></span>|<span data-ttu-id="655ae-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="655ae-143">String</span></span>|<span data-ttu-id="655ae-144">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="655ae-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="655ae-145">importId</span><span class="sxs-lookup"><span data-stu-id="655ae-145">importId</span></span>|<span data-ttu-id="655ae-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="655ae-146">String</span></span>|<span data-ttu-id="655ae-147">A ID de Importação do dispositivo de piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="655ae-147">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="655ae-148">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="655ae-148">hardwareIdentifier</span></span>|<span data-ttu-id="655ae-149">Binária</span><span class="sxs-lookup"><span data-stu-id="655ae-149">Binary</span></span>|<span data-ttu-id="655ae-150">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="655ae-150">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="655ae-151">state</span><span class="sxs-lookup"><span data-stu-id="655ae-151">state</span></span>|[<span data-ttu-id="655ae-152">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="655ae-152">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="655ae-153">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="655ae-153">Current state of the imported device.</span></span>|
|<span data-ttu-id="655ae-154">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="655ae-154">assignedUserPrincipalName</span></span>|<span data-ttu-id="655ae-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="655ae-155">String</span></span>|<span data-ttu-id="655ae-156">UPN do usuário que o dispositivo será atribuído</span><span class="sxs-lookup"><span data-stu-id="655ae-156">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="655ae-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="655ae-157">Response</span></span>
<span data-ttu-id="655ae-158">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="655ae-158">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="655ae-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="655ae-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="655ae-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="655ae-160">Request</span></span>
<span data-ttu-id="655ae-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="655ae-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 631

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
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

### <a name="response"></a><span data-ttu-id="655ae-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="655ae-162">Response</span></span>
<span data-ttu-id="655ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="655ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 680

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
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




