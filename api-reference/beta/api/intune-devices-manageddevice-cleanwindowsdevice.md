---
title: Ação cleanWindowsDevice
description: Limpar dispositivo Windows
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b6322a473d30a8a032448aacbe4f25c86c4fca7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792321"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="05163-103">Ação cleanWindowsDevice</span><span class="sxs-lookup"><span data-stu-id="05163-103">cleanWindowsDevice action</span></span>

<span data-ttu-id="05163-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05163-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05163-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="05163-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05163-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05163-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05163-107">Limpar dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="05163-107">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05163-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05163-108">Prerequisites</span></span>
<span data-ttu-id="05163-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="05163-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="05163-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05163-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05163-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05163-111">Permission type</span></span>|<span data-ttu-id="05163-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05163-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05163-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05163-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05163-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="05163-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="05163-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05163-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05163-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05163-116">Not supported.</span></span>|
|<span data-ttu-id="05163-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05163-117">Application</span></span>|<span data-ttu-id="05163-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="05163-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05163-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05163-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/comanagedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/cleanWindowsDevice
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="05163-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05163-120">Request headers</span></span>
|<span data-ttu-id="05163-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05163-121">Header</span></span>|<span data-ttu-id="05163-122">Valor</span><span class="sxs-lookup"><span data-stu-id="05163-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05163-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="05163-123">Authorization</span></span>|<span data-ttu-id="05163-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05163-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05163-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05163-125">Accept</span></span>|<span data-ttu-id="05163-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05163-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05163-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05163-127">Request body</span></span>
<span data-ttu-id="05163-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="05163-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="05163-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="05163-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="05163-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05163-130">Property</span></span>|<span data-ttu-id="05163-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="05163-131">Type</span></span>|<span data-ttu-id="05163-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="05163-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05163-133">keepUserData</span><span class="sxs-lookup"><span data-stu-id="05163-133">keepUserData</span></span>|<span data-ttu-id="05163-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="05163-134">Boolean</span></span>|<span data-ttu-id="05163-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="05163-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="05163-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="05163-136">Response</span></span>
<span data-ttu-id="05163-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="05163-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="05163-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05163-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="05163-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05163-139">Request</span></span>
<span data-ttu-id="05163-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05163-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="05163-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="05163-141">Response</span></span>
<span data-ttu-id="05163-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="05163-142">Here is an example of the response.</span></span> <span data-ttu-id="05163-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="05163-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="05163-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="05163-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



