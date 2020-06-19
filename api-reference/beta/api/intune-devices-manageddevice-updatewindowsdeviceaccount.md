---
title: Ação updateWindowsDeviceAccount
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 52ddeb86f69ddc781633ffa87a02f261575c6791
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792139"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="49105-103">Ação updateWindowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="49105-103">updateWindowsDeviceAccount action</span></span>

<span data-ttu-id="49105-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49105-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49105-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49105-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49105-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49105-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49105-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="49105-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49105-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49105-108">Prerequisites</span></span>
<span data-ttu-id="49105-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="49105-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="49105-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49105-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49105-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49105-111">Permission type</span></span>|<span data-ttu-id="49105-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49105-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49105-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49105-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49105-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="49105-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="49105-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49105-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49105-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49105-116">Not supported.</span></span>|
|<span data-ttu-id="49105-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49105-117">Application</span></span>|<span data-ttu-id="49105-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="49105-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49105-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49105-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/comanagedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="49105-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49105-120">Request headers</span></span>
|<span data-ttu-id="49105-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49105-121">Header</span></span>|<span data-ttu-id="49105-122">Valor</span><span class="sxs-lookup"><span data-stu-id="49105-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49105-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="49105-123">Authorization</span></span>|<span data-ttu-id="49105-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49105-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49105-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49105-125">Accept</span></span>|<span data-ttu-id="49105-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49105-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49105-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49105-127">Request body</span></span>
<span data-ttu-id="49105-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="49105-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="49105-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="49105-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="49105-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49105-130">Property</span></span>|<span data-ttu-id="49105-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="49105-131">Type</span></span>|<span data-ttu-id="49105-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="49105-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49105-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="49105-133">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="49105-134">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="49105-134">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="49105-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="49105-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="49105-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="49105-136">Response</span></span>
<span data-ttu-id="49105-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="49105-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="49105-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49105-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="49105-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49105-139">Request</span></span>
<span data-ttu-id="49105-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49105-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a><span data-ttu-id="49105-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="49105-141">Response</span></span>
<span data-ttu-id="49105-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="49105-142">Here is an example of the response.</span></span> <span data-ttu-id="49105-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="49105-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="49105-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="49105-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



