---
title: Criar importedWindowsAutopilotDeviceIdentity
description: Crie um novo objeto importedWindowsAutopilotDeviceIdentity.
ms.openlocfilehash: 3fe1661aa4281753aa79584bfa08c28024d01297
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037502"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="6abd3-103">Criar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="6abd3-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="6abd3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6abd3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6abd3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6abd3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6abd3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6abd3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6abd3-107">Criar um novo objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="6abd3-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6abd3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6abd3-108">Prerequisites</span></span>
<span data-ttu-id="6abd3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6abd3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6abd3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6abd3-111">Permission type</span></span>|<span data-ttu-id="6abd3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6abd3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6abd3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6abd3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6abd3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abd3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6abd3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6abd3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6abd3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6abd3-116">Not supported.</span></span>|
|<span data-ttu-id="6abd3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6abd3-117">Application</span></span>|<span data-ttu-id="6abd3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6abd3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6abd3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6abd3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="6abd3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6abd3-120">Request headers</span></span>
|<span data-ttu-id="6abd3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6abd3-121">Header</span></span>|<span data-ttu-id="6abd3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6abd3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6abd3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6abd3-123">Authorization</span></span>|<span data-ttu-id="6abd3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6abd3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6abd3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6abd3-125">Accept</span></span>|<span data-ttu-id="6abd3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6abd3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6abd3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6abd3-127">Request body</span></span>
<span data-ttu-id="6abd3-128">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="6abd3-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="6abd3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="6abd3-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="6abd3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6abd3-130">Property</span></span>|<span data-ttu-id="6abd3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6abd3-131">Type</span></span>|<span data-ttu-id="6abd3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6abd3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6abd3-133">id</span><span class="sxs-lookup"><span data-stu-id="6abd3-133">id</span></span>|<span data-ttu-id="6abd3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abd3-134">String</span></span>|<span data-ttu-id="6abd3-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="6abd3-135">The GUID for the object</span></span>|
|<span data-ttu-id="6abd3-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="6abd3-136">orderIdentifier</span></span>|<span data-ttu-id="6abd3-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abd3-137">String</span></span>|<span data-ttu-id="6abd3-138">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6abd3-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6abd3-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="6abd3-139">serialNumber</span></span>|<span data-ttu-id="6abd3-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abd3-140">String</span></span>|<span data-ttu-id="6abd3-141">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6abd3-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6abd3-142">productKey</span><span class="sxs-lookup"><span data-stu-id="6abd3-142">productKey</span></span>|<span data-ttu-id="6abd3-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6abd3-143">String</span></span>|<span data-ttu-id="6abd3-144">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6abd3-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6abd3-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="6abd3-145">hardwareIdentifier</span></span>|<span data-ttu-id="6abd3-146">Binária</span><span class="sxs-lookup"><span data-stu-id="6abd3-146">Binary</span></span>|<span data-ttu-id="6abd3-147">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="6abd3-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6abd3-148">state</span><span class="sxs-lookup"><span data-stu-id="6abd3-148">state</span></span>|[<span data-ttu-id="6abd3-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="6abd3-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="6abd3-150">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="6abd3-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="6abd3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6abd3-151">Response</span></span>
<span data-ttu-id="6abd3-152">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6abd3-152">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6abd3-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6abd3-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="6abd3-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6abd3-154">Request</span></span>
<span data-ttu-id="6abd3-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6abd3-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="6abd3-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="6abd3-156">Response</span></span>
<span data-ttu-id="6abd3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6abd3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





