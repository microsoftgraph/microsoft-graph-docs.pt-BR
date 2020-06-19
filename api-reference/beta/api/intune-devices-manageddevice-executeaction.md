---
title: Ação executeAction
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b16beb4e8a40c674e3c1a95d937d21893df595e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792293"
---
# <a name="executeaction-action"></a><span data-ttu-id="4a8d2-103">Ação executeAction</span><span class="sxs-lookup"><span data-stu-id="4a8d2-103">executeAction action</span></span>

<span data-ttu-id="4a8d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a8d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a8d2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a8d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a8d2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a8d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a8d2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a8d2-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a8d2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a8d2-108">Prerequisites</span></span>
<span data-ttu-id="4a8d2-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4a8d2-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4a8d2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a8d2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a8d2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a8d2-111">Permission type</span></span>|<span data-ttu-id="4a8d2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a8d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a8d2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a8d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a8d2-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4a8d2-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="4a8d2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a8d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a8d2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a8d2-116">Not supported.</span></span>|
|<span data-ttu-id="4a8d2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a8d2-117">Application</span></span>|<span data-ttu-id="4a8d2-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4a8d2-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a8d2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a8d2-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4a8d2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a8d2-120">Request headers</span></span>
|<span data-ttu-id="4a8d2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a8d2-121">Header</span></span>|<span data-ttu-id="4a8d2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4a8d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a8d2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a8d2-123">Authorization</span></span>|<span data-ttu-id="4a8d2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a8d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a8d2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a8d2-125">Accept</span></span>|<span data-ttu-id="4a8d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a8d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a8d2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a8d2-127">Request body</span></span>
<span data-ttu-id="4a8d2-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="4a8d2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4a8d2-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="4a8d2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4a8d2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a8d2-130">Property</span></span>|<span data-ttu-id="4a8d2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a8d2-131">Type</span></span>|<span data-ttu-id="4a8d2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a8d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a8d2-133">actionName</span><span class="sxs-lookup"><span data-stu-id="4a8d2-133">actionName</span></span>|[<span data-ttu-id="4a8d2-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="4a8d2-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="4a8d2-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a8d2-135">Not yet documented</span></span>|
|<span data-ttu-id="4a8d2-136">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="4a8d2-136">keepEnrollmentData</span></span>|<span data-ttu-id="4a8d2-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a8d2-137">Boolean</span></span>|<span data-ttu-id="4a8d2-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a8d2-138">Not yet documented</span></span>|
|<span data-ttu-id="4a8d2-139">keepUserData</span><span class="sxs-lookup"><span data-stu-id="4a8d2-139">keepUserData</span></span>|<span data-ttu-id="4a8d2-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a8d2-140">Boolean</span></span>|<span data-ttu-id="4a8d2-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a8d2-141">Not yet documented</span></span>|
|<span data-ttu-id="4a8d2-142">deviceIds</span><span class="sxs-lookup"><span data-stu-id="4a8d2-142">deviceIds</span></span>|<span data-ttu-id="4a8d2-143">String collection</span><span class="sxs-lookup"><span data-stu-id="4a8d2-143">String collection</span></span>|<span data-ttu-id="4a8d2-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a8d2-144">Not yet documented</span></span>|
|<span data-ttu-id="4a8d2-145">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="4a8d2-145">notificationTitle</span></span>|<span data-ttu-id="4a8d2-146">String</span><span class="sxs-lookup"><span data-stu-id="4a8d2-146">String</span></span>|<span data-ttu-id="4a8d2-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a8d2-147">Not yet documented</span></span>|
|<span data-ttu-id="4a8d2-148">notificationBody</span><span class="sxs-lookup"><span data-stu-id="4a8d2-148">notificationBody</span></span>|<span data-ttu-id="4a8d2-149">String</span><span class="sxs-lookup"><span data-stu-id="4a8d2-149">String</span></span>|<span data-ttu-id="4a8d2-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a8d2-150">Not yet documented</span></span>|
|<span data-ttu-id="4a8d2-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="4a8d2-151">deviceName</span></span>|<span data-ttu-id="4a8d2-152">String</span><span class="sxs-lookup"><span data-stu-id="4a8d2-152">String</span></span>|<span data-ttu-id="4a8d2-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a8d2-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4a8d2-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a8d2-154">Response</span></span>
<span data-ttu-id="4a8d2-155">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e um [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a8d2-155">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a8d2-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a8d2-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a8d2-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a8d2-157">Request</span></span>
<span data-ttu-id="4a8d2-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a8d2-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4a8d2-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a8d2-159">Response</span></span>
<span data-ttu-id="4a8d2-160">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="4a8d2-160">Here is an example of the response.</span></span> <span data-ttu-id="4a8d2-161">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="4a8d2-161">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4a8d2-162">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="4a8d2-162">All of the properties will be returned from an actual call.</span></span>
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



