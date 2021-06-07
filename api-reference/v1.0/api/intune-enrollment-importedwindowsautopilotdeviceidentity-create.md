---
title: Criar importedWindowsAutopilotDeviceIdentity
description: Criar um novo objeto importedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d0478e84f3bf0679588fbc9f962b3471dec90f1d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752875"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="b4b82-103">Criar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="b4b82-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="b4b82-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4b82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4b82-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4b82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4b82-106">Criar um novo objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="b4b82-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4b82-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4b82-107">Prerequisites</span></span>
<span data-ttu-id="b4b82-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4b82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4b82-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4b82-110">Permission type</span></span>|<span data-ttu-id="b4b82-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4b82-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4b82-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4b82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4b82-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4b82-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b4b82-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4b82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4b82-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4b82-115">Not supported.</span></span>|
|<span data-ttu-id="b4b82-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4b82-116">Application</span></span>|<span data-ttu-id="b4b82-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4b82-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4b82-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4b82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="b4b82-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4b82-119">Request headers</span></span>
|<span data-ttu-id="b4b82-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4b82-120">Header</span></span>|<span data-ttu-id="b4b82-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b4b82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4b82-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4b82-122">Authorization</span></span>|<span data-ttu-id="b4b82-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4b82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4b82-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4b82-124">Accept</span></span>|<span data-ttu-id="b4b82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4b82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4b82-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4b82-126">Request body</span></span>
<span data-ttu-id="b4b82-127">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="b4b82-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="b4b82-128">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="b4b82-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="b4b82-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4b82-129">Property</span></span>|<span data-ttu-id="b4b82-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4b82-130">Type</span></span>|<span data-ttu-id="b4b82-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4b82-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4b82-132">id</span><span class="sxs-lookup"><span data-stu-id="b4b82-132">id</span></span>|<span data-ttu-id="b4b82-133">String</span><span class="sxs-lookup"><span data-stu-id="b4b82-133">String</span></span>|<span data-ttu-id="b4b82-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="b4b82-134">The GUID for the object</span></span>|
|<span data-ttu-id="b4b82-135">groupTag</span><span class="sxs-lookup"><span data-stu-id="b4b82-135">groupTag</span></span>|<span data-ttu-id="b4b82-136">String</span><span class="sxs-lookup"><span data-stu-id="b4b82-136">String</span></span>|<span data-ttu-id="b4b82-137">Marca de grupo do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="b4b82-137">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b4b82-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="b4b82-138">serialNumber</span></span>|<span data-ttu-id="b4b82-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4b82-139">String</span></span>|<span data-ttu-id="b4b82-140">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="b4b82-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b4b82-141">productKey</span><span class="sxs-lookup"><span data-stu-id="b4b82-141">productKey</span></span>|<span data-ttu-id="b4b82-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4b82-142">String</span></span>|<span data-ttu-id="b4b82-143">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="b4b82-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b4b82-144">importId</span><span class="sxs-lookup"><span data-stu-id="b4b82-144">importId</span></span>|<span data-ttu-id="b4b82-145">String</span><span class="sxs-lookup"><span data-stu-id="b4b82-145">String</span></span>|<span data-ttu-id="b4b82-146">A ID de Importação do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="b4b82-146">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b4b82-147">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="b4b82-147">hardwareIdentifier</span></span>|<span data-ttu-id="b4b82-148">Binária</span><span class="sxs-lookup"><span data-stu-id="b4b82-148">Binary</span></span>|<span data-ttu-id="b4b82-149">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="b4b82-149">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b4b82-150">state</span><span class="sxs-lookup"><span data-stu-id="b4b82-150">state</span></span>|[<span data-ttu-id="b4b82-151">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="b4b82-151">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="b4b82-152">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="b4b82-152">Current state of the imported device.</span></span>|
|<span data-ttu-id="b4b82-153">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b4b82-153">assignedUserPrincipalName</span></span>|<span data-ttu-id="b4b82-154">String</span><span class="sxs-lookup"><span data-stu-id="b4b82-154">String</span></span>|<span data-ttu-id="b4b82-155">UPN do usuário que o dispositivo será atribuído</span><span class="sxs-lookup"><span data-stu-id="b4b82-155">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="b4b82-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4b82-156">Response</span></span>
<span data-ttu-id="b4b82-157">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4b82-157">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4b82-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4b82-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4b82-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4b82-159">Request</span></span>
<span data-ttu-id="b4b82-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4b82-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="b4b82-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4b82-161">Response</span></span>
<span data-ttu-id="b4b82-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4b82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




