---
title: Ação executeAction
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf5edf59f0cc96f5f711dd0361e6623cd41b3ebc
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909698"
---
# <a name="executeaction-action"></a><span data-ttu-id="4d214-103">Ação executeAction</span><span class="sxs-lookup"><span data-stu-id="4d214-103">executeAction action</span></span>

> <span data-ttu-id="4d214-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4d214-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d214-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4d214-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d214-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4d214-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d214-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d214-107">Prerequisites</span></span>
<span data-ttu-id="4d214-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d214-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d214-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d214-110">Permission type</span></span>|<span data-ttu-id="4d214-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4d214-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d214-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d214-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d214-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4d214-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="4d214-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d214-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d214-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d214-115">Not supported.</span></span>|
|<span data-ttu-id="4d214-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d214-116">Application</span></span>|<span data-ttu-id="4d214-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d214-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d214-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d214-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="4d214-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d214-119">Request headers</span></span>
|<span data-ttu-id="4d214-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d214-120">Header</span></span>|<span data-ttu-id="4d214-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4d214-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d214-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d214-122">Authorization</span></span>|<span data-ttu-id="4d214-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d214-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d214-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4d214-124">Accept</span></span>|<span data-ttu-id="4d214-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d214-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d214-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d214-126">Request body</span></span>
<span data-ttu-id="4d214-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="4d214-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4d214-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="4d214-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4d214-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d214-129">Property</span></span>|<span data-ttu-id="4d214-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d214-130">Type</span></span>|<span data-ttu-id="4d214-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d214-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d214-132">actionName</span><span class="sxs-lookup"><span data-stu-id="4d214-132">actionName</span></span>|[<span data-ttu-id="4d214-133">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="4d214-133">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="4d214-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4d214-134">Not yet documented</span></span>|
|<span data-ttu-id="4d214-135">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="4d214-135">keepEnrollmentData</span></span>|<span data-ttu-id="4d214-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d214-136">Boolean</span></span>|<span data-ttu-id="4d214-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4d214-137">Not yet documented</span></span>|
|<span data-ttu-id="4d214-138">keepUserData</span><span class="sxs-lookup"><span data-stu-id="4d214-138">keepUserData</span></span>|<span data-ttu-id="4d214-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d214-139">Boolean</span></span>|<span data-ttu-id="4d214-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4d214-140">Not yet documented</span></span>|
|<span data-ttu-id="4d214-141">deviceIds</span><span class="sxs-lookup"><span data-stu-id="4d214-141">deviceIds</span></span>|<span data-ttu-id="4d214-142">String collection</span><span class="sxs-lookup"><span data-stu-id="4d214-142">String collection</span></span>|<span data-ttu-id="4d214-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4d214-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4d214-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d214-144">Response</span></span>
<span data-ttu-id="4d214-145">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d214-145">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d214-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d214-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d214-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d214-147">Request</span></span>
<span data-ttu-id="4d214-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d214-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/executeAction

Content-type: application/json
Content-length: 134

{
  "actionName": "delete",
  "keepEnrollmentData": true,
  "keepUserData": true,
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="4d214-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d214-149">Response</span></span>
<span data-ttu-id="4d214-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d214-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




