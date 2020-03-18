---
title: Ação setDeviceName
description: Defina o nome do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 78c88d12fec16e7ef4e08750def7c8710483ba5f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42774439"
---
# <a name="setdevicename-action"></a><span data-ttu-id="07998-103">Ação setDeviceName</span><span class="sxs-lookup"><span data-stu-id="07998-103">setDeviceName action</span></span>

> <span data-ttu-id="07998-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07998-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07998-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07998-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07998-106">Defina o nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="07998-106">Set device name of the device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07998-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07998-107">Prerequisites</span></span>
<span data-ttu-id="07998-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07998-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07998-110">Permission type</span></span>|<span data-ttu-id="07998-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07998-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07998-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07998-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07998-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="07998-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="07998-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07998-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07998-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07998-115">Not supported.</span></span>|
|<span data-ttu-id="07998-116">Application</span><span class="sxs-lookup"><span data-stu-id="07998-116">Application</span></span>|<span data-ttu-id="07998-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="07998-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07998-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07998-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/setDeviceName
```

## <a name="request-headers"></a><span data-ttu-id="07998-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07998-119">Request headers</span></span>
|<span data-ttu-id="07998-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07998-120">Header</span></span>|<span data-ttu-id="07998-121">Valor</span><span class="sxs-lookup"><span data-stu-id="07998-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07998-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="07998-122">Authorization</span></span>|<span data-ttu-id="07998-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07998-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07998-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07998-124">Accept</span></span>|<span data-ttu-id="07998-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07998-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07998-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07998-126">Request body</span></span>
<span data-ttu-id="07998-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="07998-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="07998-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="07998-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="07998-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07998-129">Property</span></span>|<span data-ttu-id="07998-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="07998-130">Type</span></span>|<span data-ttu-id="07998-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="07998-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07998-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="07998-132">deviceName</span></span>|<span data-ttu-id="07998-133">String</span><span class="sxs-lookup"><span data-stu-id="07998-133">String</span></span>|<span data-ttu-id="07998-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07998-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="07998-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="07998-135">Response</span></span>
<span data-ttu-id="07998-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="07998-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="07998-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07998-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="07998-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07998-138">Request</span></span>
<span data-ttu-id="07998-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07998-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/setDeviceName

Content-type: application/json
Content-length: 41

{
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="07998-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="07998-140">Response</span></span>
<span data-ttu-id="07998-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07998-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




