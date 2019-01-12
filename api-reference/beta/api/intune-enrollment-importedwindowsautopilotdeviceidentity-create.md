---
title: Criar importedWindowsAutopilotDeviceIdentity
description: Crie um novo objeto importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fe0b127db8309daddfc000d3c985a687739b68d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939249"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="e3789-103">Criar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="e3789-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="e3789-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e3789-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3789-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e3789-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3789-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e3789-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3789-107">Criar um novo objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="e3789-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3789-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3789-108">Prerequisites</span></span>
<span data-ttu-id="e3789-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3789-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3789-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3789-111">Permission type</span></span>|<span data-ttu-id="e3789-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3789-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3789-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3789-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3789-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3789-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e3789-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3789-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3789-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3789-116">Not supported.</span></span>|
|<span data-ttu-id="e3789-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3789-117">Application</span></span>|<span data-ttu-id="e3789-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3789-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3789-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3789-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="e3789-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3789-120">Request headers</span></span>
|<span data-ttu-id="e3789-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3789-121">Header</span></span>|<span data-ttu-id="e3789-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e3789-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3789-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3789-123">Authorization</span></span>|<span data-ttu-id="e3789-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3789-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3789-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3789-125">Accept</span></span>|<span data-ttu-id="e3789-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3789-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3789-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3789-127">Request body</span></span>
<span data-ttu-id="e3789-128">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="e3789-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="e3789-129">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="e3789-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="e3789-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3789-130">Property</span></span>|<span data-ttu-id="e3789-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3789-131">Type</span></span>|<span data-ttu-id="e3789-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3789-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3789-133">id</span><span class="sxs-lookup"><span data-stu-id="e3789-133">id</span></span>|<span data-ttu-id="e3789-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3789-134">String</span></span>|<span data-ttu-id="e3789-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="e3789-135">The GUID for the object</span></span>|
|<span data-ttu-id="e3789-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="e3789-136">orderIdentifier</span></span>|<span data-ttu-id="e3789-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3789-137">String</span></span>|<span data-ttu-id="e3789-138">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="e3789-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e3789-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="e3789-139">serialNumber</span></span>|<span data-ttu-id="e3789-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3789-140">String</span></span>|<span data-ttu-id="e3789-141">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="e3789-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e3789-142">productKey</span><span class="sxs-lookup"><span data-stu-id="e3789-142">productKey</span></span>|<span data-ttu-id="e3789-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3789-143">String</span></span>|<span data-ttu-id="e3789-144">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="e3789-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e3789-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="e3789-145">hardwareIdentifier</span></span>|<span data-ttu-id="e3789-146">Binária</span><span class="sxs-lookup"><span data-stu-id="e3789-146">Binary</span></span>|<span data-ttu-id="e3789-147">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="e3789-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e3789-148">state</span><span class="sxs-lookup"><span data-stu-id="e3789-148">state</span></span>|[<span data-ttu-id="e3789-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="e3789-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="e3789-150">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="e3789-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="e3789-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3789-151">Response</span></span>
<span data-ttu-id="e3789-152">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3789-152">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3789-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3789-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3789-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3789-154">Request</span></span>
<span data-ttu-id="e3789-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3789-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3789-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3789-156">Response</span></span>
<span data-ttu-id="e3789-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3789-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





