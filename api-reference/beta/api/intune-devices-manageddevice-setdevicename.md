---
title: Ação setDeviceName
description: Defina o nome do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ebcf90a628ff4a3a435e34a2439a277fa3a3064d
ms.sourcegitcommit: 258974d689cb8f04ff542ec8bc5fe5793da5cc05
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/08/2020
ms.locfileid: "48385804"
---
# <a name="setdevicename-action"></a><span data-ttu-id="62c55-103">Ação setDeviceName</span><span class="sxs-lookup"><span data-stu-id="62c55-103">setDeviceName action</span></span>

<span data-ttu-id="62c55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62c55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62c55-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62c55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62c55-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62c55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62c55-107">Defina o nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62c55-107">Set device name of the device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62c55-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62c55-108">Prerequisites</span></span>
<span data-ttu-id="62c55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62c55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62c55-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62c55-111">Permission type</span></span>|<span data-ttu-id="62c55-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62c55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62c55-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62c55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62c55-114">DeviceManagementManagedDevices.PrivilegedOperations.All</span><span class="sxs-lookup"><span data-stu-id="62c55-114">DeviceManagementManagedDevices.PrivilegedOperations.All</span></span>|
|<span data-ttu-id="62c55-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62c55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62c55-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62c55-116">Not supported.</span></span>|
|<span data-ttu-id="62c55-117">Application</span><span class="sxs-lookup"><span data-stu-id="62c55-117">Application</span></span>|<span data-ttu-id="62c55-118">DeviceManagementManagedDevices.PrivilegedOperations.All</span><span class="sxs-lookup"><span data-stu-id="62c55-118">DeviceManagementManagedDevices.PrivilegedOperations.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62c55-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62c55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/comanagedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/setDeviceName
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/setDeviceName
```

## <a name="request-headers"></a><span data-ttu-id="62c55-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62c55-120">Request headers</span></span>
|<span data-ttu-id="62c55-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62c55-121">Header</span></span>|<span data-ttu-id="62c55-122">Valor</span><span class="sxs-lookup"><span data-stu-id="62c55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62c55-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="62c55-123">Authorization</span></span>|<span data-ttu-id="62c55-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62c55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62c55-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62c55-125">Accept</span></span>|<span data-ttu-id="62c55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62c55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62c55-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62c55-127">Request body</span></span>
<span data-ttu-id="62c55-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="62c55-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="62c55-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="62c55-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="62c55-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62c55-130">Property</span></span>|<span data-ttu-id="62c55-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="62c55-131">Type</span></span>|<span data-ttu-id="62c55-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="62c55-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62c55-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="62c55-133">deviceName</span></span>|<span data-ttu-id="62c55-134">String</span><span class="sxs-lookup"><span data-stu-id="62c55-134">String</span></span>|<span data-ttu-id="62c55-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="62c55-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="62c55-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="62c55-136">Response</span></span>
<span data-ttu-id="62c55-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="62c55-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="62c55-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62c55-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="62c55-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62c55-139">Request</span></span>
<span data-ttu-id="62c55-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62c55-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/setDeviceName

Content-type: application/json
Content-length: 41

{
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="62c55-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="62c55-141">Response</span></span>
<span data-ttu-id="62c55-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62c55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






