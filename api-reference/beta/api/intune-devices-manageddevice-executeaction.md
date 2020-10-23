---
title: Ação executeAction
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3e64ed7ab003ae340cbcab24bc093843b01e23c0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708232"
---
# <a name="executeaction-action"></a><span data-ttu-id="7c966-103">Ação executeAction</span><span class="sxs-lookup"><span data-stu-id="7c966-103">executeAction action</span></span>

<span data-ttu-id="7c966-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c966-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c966-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c966-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c966-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c966-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c966-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7c966-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c966-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c966-108">Prerequisites</span></span>
<span data-ttu-id="7c966-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c966-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c966-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c966-111">Permission type</span></span>|<span data-ttu-id="7c966-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7c966-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c966-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c966-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c966-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="7c966-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="7c966-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c966-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c966-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c966-116">Not supported.</span></span>|
|<span data-ttu-id="7c966-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c966-117">Application</span></span>|<span data-ttu-id="7c966-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="7c966-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c966-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c966-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/comanagedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="7c966-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c966-120">Request headers</span></span>
|<span data-ttu-id="7c966-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c966-121">Header</span></span>|<span data-ttu-id="7c966-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7c966-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c966-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c966-123">Authorization</span></span>|<span data-ttu-id="7c966-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c966-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c966-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c966-125">Accept</span></span>|<span data-ttu-id="7c966-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c966-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c966-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c966-127">Request body</span></span>
<span data-ttu-id="7c966-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7c966-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7c966-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7c966-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7c966-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c966-130">Property</span></span>|<span data-ttu-id="7c966-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c966-131">Type</span></span>|<span data-ttu-id="7c966-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c966-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c966-133">actionName</span><span class="sxs-lookup"><span data-stu-id="7c966-133">actionName</span></span>|[<span data-ttu-id="7c966-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="7c966-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="7c966-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7c966-135">Not yet documented</span></span>|
|<span data-ttu-id="7c966-136">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="7c966-136">keepEnrollmentData</span></span>|<span data-ttu-id="7c966-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="7c966-137">Boolean</span></span>|<span data-ttu-id="7c966-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7c966-138">Not yet documented</span></span>|
|<span data-ttu-id="7c966-139">keepUserData</span><span class="sxs-lookup"><span data-stu-id="7c966-139">keepUserData</span></span>|<span data-ttu-id="7c966-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="7c966-140">Boolean</span></span>|<span data-ttu-id="7c966-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7c966-141">Not yet documented</span></span>|
|<span data-ttu-id="7c966-142">deviceIds</span><span class="sxs-lookup"><span data-stu-id="7c966-142">deviceIds</span></span>|<span data-ttu-id="7c966-143">String collection</span><span class="sxs-lookup"><span data-stu-id="7c966-143">String collection</span></span>|<span data-ttu-id="7c966-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7c966-144">Not yet documented</span></span>|
|<span data-ttu-id="7c966-145">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="7c966-145">notificationTitle</span></span>|<span data-ttu-id="7c966-146">String</span><span class="sxs-lookup"><span data-stu-id="7c966-146">String</span></span>|<span data-ttu-id="7c966-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7c966-147">Not yet documented</span></span>|
|<span data-ttu-id="7c966-148">notificationBody</span><span class="sxs-lookup"><span data-stu-id="7c966-148">notificationBody</span></span>|<span data-ttu-id="7c966-149">String</span><span class="sxs-lookup"><span data-stu-id="7c966-149">String</span></span>|<span data-ttu-id="7c966-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7c966-150">Not yet documented</span></span>|
|<span data-ttu-id="7c966-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="7c966-151">deviceName</span></span>|<span data-ttu-id="7c966-152">String</span><span class="sxs-lookup"><span data-stu-id="7c966-152">String</span></span>|<span data-ttu-id="7c966-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7c966-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7c966-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c966-154">Response</span></span>
<span data-ttu-id="7c966-155">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e um [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c966-155">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c966-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c966-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c966-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c966-157">Request</span></span>
<span data-ttu-id="7c966-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c966-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/executeAction

Content-type: application/json
Content-length: 274

{
  "actionName": "delete",
  "keepEnrollmentData": true,
  "keepUserData": true,
  "deviceIds": [
    "Device Ids value"
  ],
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value",
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="7c966-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c966-159">Response</span></span>
<span data-ttu-id="7c966-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c966-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult",
    "successfulDeviceIds": [
      "Successful Device Ids value"
    ],
    "failedDeviceIds": [
      "Failed Device Ids value"
    ],
    "notFoundDeviceIds": [
      "Not Found Device Ids value"
    ],
    "notSupportedDeviceIds": [
      "Not Supported Device Ids value"
    ]
  }
}
```





