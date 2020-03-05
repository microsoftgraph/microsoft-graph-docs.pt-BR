---
title: Ação executeAction
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5500b697afcb21d62cb063231924843ed2d1de20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469059"
---
# <a name="executeaction-action"></a><span data-ttu-id="c81f0-103">Ação executeAction</span><span class="sxs-lookup"><span data-stu-id="c81f0-103">executeAction action</span></span>

<span data-ttu-id="c81f0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c81f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c81f0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c81f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c81f0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c81f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c81f0-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c81f0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c81f0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c81f0-108">Prerequisites</span></span>
<span data-ttu-id="c81f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c81f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c81f0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c81f0-111">Permission type</span></span>|<span data-ttu-id="c81f0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c81f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c81f0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c81f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c81f0-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c81f0-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="c81f0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c81f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c81f0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c81f0-116">Not supported.</span></span>|
|<span data-ttu-id="c81f0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c81f0-117">Application</span></span>|<span data-ttu-id="c81f0-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c81f0-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c81f0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c81f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="c81f0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c81f0-120">Request headers</span></span>
|<span data-ttu-id="c81f0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c81f0-121">Header</span></span>|<span data-ttu-id="c81f0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c81f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c81f0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c81f0-123">Authorization</span></span>|<span data-ttu-id="c81f0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c81f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c81f0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c81f0-125">Accept</span></span>|<span data-ttu-id="c81f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c81f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c81f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c81f0-127">Request body</span></span>
<span data-ttu-id="c81f0-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c81f0-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c81f0-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c81f0-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c81f0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c81f0-130">Property</span></span>|<span data-ttu-id="c81f0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c81f0-131">Type</span></span>|<span data-ttu-id="c81f0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c81f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c81f0-133">actionName</span><span class="sxs-lookup"><span data-stu-id="c81f0-133">actionName</span></span>|[<span data-ttu-id="c81f0-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="c81f0-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="c81f0-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c81f0-135">Not yet documented</span></span>|
|<span data-ttu-id="c81f0-136">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="c81f0-136">keepEnrollmentData</span></span>|<span data-ttu-id="c81f0-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="c81f0-137">Boolean</span></span>|<span data-ttu-id="c81f0-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c81f0-138">Not yet documented</span></span>|
|<span data-ttu-id="c81f0-139">keepUserData</span><span class="sxs-lookup"><span data-stu-id="c81f0-139">keepUserData</span></span>|<span data-ttu-id="c81f0-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="c81f0-140">Boolean</span></span>|<span data-ttu-id="c81f0-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c81f0-141">Not yet documented</span></span>|
|<span data-ttu-id="c81f0-142">deviceIds</span><span class="sxs-lookup"><span data-stu-id="c81f0-142">deviceIds</span></span>|<span data-ttu-id="c81f0-143">String collection</span><span class="sxs-lookup"><span data-stu-id="c81f0-143">String collection</span></span>|<span data-ttu-id="c81f0-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c81f0-144">Not yet documented</span></span>|
|<span data-ttu-id="c81f0-145">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="c81f0-145">notificationTitle</span></span>|<span data-ttu-id="c81f0-146">String</span><span class="sxs-lookup"><span data-stu-id="c81f0-146">String</span></span>|<span data-ttu-id="c81f0-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c81f0-147">Not yet documented</span></span>|
|<span data-ttu-id="c81f0-148">notificationBody</span><span class="sxs-lookup"><span data-stu-id="c81f0-148">notificationBody</span></span>|<span data-ttu-id="c81f0-149">String</span><span class="sxs-lookup"><span data-stu-id="c81f0-149">String</span></span>|<span data-ttu-id="c81f0-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c81f0-150">Not yet documented</span></span>|
|<span data-ttu-id="c81f0-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="c81f0-151">deviceName</span></span>|<span data-ttu-id="c81f0-152">String</span><span class="sxs-lookup"><span data-stu-id="c81f0-152">String</span></span>|<span data-ttu-id="c81f0-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c81f0-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c81f0-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="c81f0-154">Response</span></span>
<span data-ttu-id="c81f0-155">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c81f0-155">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c81f0-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c81f0-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="c81f0-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c81f0-157">Request</span></span>
<span data-ttu-id="c81f0-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c81f0-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c81f0-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="c81f0-159">Response</span></span>
<span data-ttu-id="c81f0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c81f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





