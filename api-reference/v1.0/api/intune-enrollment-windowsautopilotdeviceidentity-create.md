---
title: Criar windowsAutopilotDeviceIdentity
description: Crie um novo objeto windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7ee59ca45db337f85f1c4f0f01443c2c0965e1c0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752863"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="75492-103">Criar windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="75492-103">Create windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="75492-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75492-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75492-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75492-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75492-106">Crie um novo [objeto windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="75492-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75492-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75492-107">Prerequisites</span></span>
<span data-ttu-id="75492-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75492-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75492-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75492-110">Permission type</span></span>|<span data-ttu-id="75492-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75492-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75492-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75492-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75492-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75492-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="75492-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75492-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75492-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75492-115">Not supported.</span></span>|
|<span data-ttu-id="75492-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75492-116">Application</span></span>|<span data-ttu-id="75492-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75492-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75492-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75492-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="75492-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75492-119">Request headers</span></span>
|<span data-ttu-id="75492-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75492-120">Header</span></span>|<span data-ttu-id="75492-121">Valor</span><span class="sxs-lookup"><span data-stu-id="75492-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75492-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="75492-122">Authorization</span></span>|<span data-ttu-id="75492-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75492-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75492-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75492-124">Accept</span></span>|<span data-ttu-id="75492-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75492-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75492-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75492-126">Request body</span></span>
<span data-ttu-id="75492-127">No corpo da solicitação, fornece uma representação JSON para o objeto windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="75492-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="75492-128">A tabela a seguir mostra as propriedades necessárias ao criar o windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="75492-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="75492-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75492-129">Property</span></span>|<span data-ttu-id="75492-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="75492-130">Type</span></span>|<span data-ttu-id="75492-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="75492-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75492-132">id</span><span class="sxs-lookup"><span data-stu-id="75492-132">id</span></span>|<span data-ttu-id="75492-133">String</span><span class="sxs-lookup"><span data-stu-id="75492-133">String</span></span>|<span data-ttu-id="75492-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="75492-134">The GUID for the object</span></span>|
|<span data-ttu-id="75492-135">groupTag</span><span class="sxs-lookup"><span data-stu-id="75492-135">groupTag</span></span>|<span data-ttu-id="75492-136">String</span><span class="sxs-lookup"><span data-stu-id="75492-136">String</span></span>|<span data-ttu-id="75492-137">Marca de grupo do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="75492-137">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="75492-138">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="75492-138">purchaseOrderIdentifier</span></span>|<span data-ttu-id="75492-139">String</span><span class="sxs-lookup"><span data-stu-id="75492-139">String</span></span>|<span data-ttu-id="75492-140">Purchase Order Identifier of the Windows autopilot device.</span><span class="sxs-lookup"><span data-stu-id="75492-140">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="75492-141">serialNumber</span><span class="sxs-lookup"><span data-stu-id="75492-141">serialNumber</span></span>|<span data-ttu-id="75492-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75492-142">String</span></span>|<span data-ttu-id="75492-143">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="75492-143">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="75492-144">productKey</span><span class="sxs-lookup"><span data-stu-id="75492-144">productKey</span></span>|<span data-ttu-id="75492-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75492-145">String</span></span>|<span data-ttu-id="75492-146">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="75492-146">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="75492-147">fabricante</span><span class="sxs-lookup"><span data-stu-id="75492-147">manufacturer</span></span>|<span data-ttu-id="75492-148">String</span><span class="sxs-lookup"><span data-stu-id="75492-148">String</span></span>|<span data-ttu-id="75492-149">Fabricante Oem do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="75492-149">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="75492-150">modelo</span><span class="sxs-lookup"><span data-stu-id="75492-150">model</span></span>|<span data-ttu-id="75492-151">String</span><span class="sxs-lookup"><span data-stu-id="75492-151">String</span></span>|<span data-ttu-id="75492-152">Nome do modelo do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="75492-152">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="75492-153">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="75492-153">enrollmentState</span></span>|[<span data-ttu-id="75492-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="75492-154">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="75492-155">Estado de registro do intune do dispositivo Windows piloto automático.</span><span class="sxs-lookup"><span data-stu-id="75492-155">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="75492-156">Os valores possíveis são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`.</span><span class="sxs-lookup"><span data-stu-id="75492-156">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`.</span></span>|
|<span data-ttu-id="75492-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="75492-157">lastContactedDateTime</span></span>|<span data-ttu-id="75492-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75492-158">DateTimeOffset</span></span>|<span data-ttu-id="75492-159">Intune Last Contacted Date Time of the Windows autopilot device.</span><span class="sxs-lookup"><span data-stu-id="75492-159">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="75492-160">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="75492-160">addressableUserName</span></span>|<span data-ttu-id="75492-161">String</span><span class="sxs-lookup"><span data-stu-id="75492-161">String</span></span>|<span data-ttu-id="75492-162">Nome de usuário acessível.</span><span class="sxs-lookup"><span data-stu-id="75492-162">Addressable user name.</span></span>|
|<span data-ttu-id="75492-163">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="75492-163">userPrincipalName</span></span>|<span data-ttu-id="75492-164">String</span><span class="sxs-lookup"><span data-stu-id="75492-164">String</span></span>|<span data-ttu-id="75492-165">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="75492-165">User Principal Name.</span></span>|
|<span data-ttu-id="75492-166">resourceName</span><span class="sxs-lookup"><span data-stu-id="75492-166">resourceName</span></span>|<span data-ttu-id="75492-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75492-167">String</span></span>|<span data-ttu-id="75492-168">Nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="75492-168">Resource Name.</span></span>|
|<span data-ttu-id="75492-169">skuNumber</span><span class="sxs-lookup"><span data-stu-id="75492-169">skuNumber</span></span>|<span data-ttu-id="75492-170">String</span><span class="sxs-lookup"><span data-stu-id="75492-170">String</span></span>|<span data-ttu-id="75492-171">Número SKU</span><span class="sxs-lookup"><span data-stu-id="75492-171">SKU Number</span></span>|
|<span data-ttu-id="75492-172">systemFamily</span><span class="sxs-lookup"><span data-stu-id="75492-172">systemFamily</span></span>|<span data-ttu-id="75492-173">String</span><span class="sxs-lookup"><span data-stu-id="75492-173">String</span></span>|<span data-ttu-id="75492-174">Família do Sistema</span><span class="sxs-lookup"><span data-stu-id="75492-174">System Family</span></span>|
|<span data-ttu-id="75492-175">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="75492-175">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="75492-176">String</span><span class="sxs-lookup"><span data-stu-id="75492-176">String</span></span>|<span data-ttu-id="75492-177">ID do dispositivo AAD - a ser preterida</span><span class="sxs-lookup"><span data-stu-id="75492-177">AAD Device ID - to be deprecated</span></span>|
|<span data-ttu-id="75492-178">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="75492-178">managedDeviceId</span></span>|<span data-ttu-id="75492-179">String</span><span class="sxs-lookup"><span data-stu-id="75492-179">String</span></span>|<span data-ttu-id="75492-180">ID de dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="75492-180">Managed Device ID</span></span>|
|<span data-ttu-id="75492-181">displayName</span><span class="sxs-lookup"><span data-stu-id="75492-181">displayName</span></span>|<span data-ttu-id="75492-182">String</span><span class="sxs-lookup"><span data-stu-id="75492-182">String</span></span>|<span data-ttu-id="75492-183">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="75492-183">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="75492-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="75492-184">Response</span></span>
<span data-ttu-id="75492-185">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75492-185">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75492-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75492-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="75492-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75492-187">Request</span></span>
<span data-ttu-id="75492-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75492-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 814

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="75492-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="75492-189">Response</span></span>
<span data-ttu-id="75492-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75492-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 863

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```




