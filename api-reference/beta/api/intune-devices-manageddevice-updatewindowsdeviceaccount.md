---
title: Ação updateWindowsDeviceAccount
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6453d2b47b370a3642409794f3fed96a5f579f6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35981371"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="1db9b-103">Ação updateWindowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="1db9b-103">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="1db9b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1db9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1db9b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1db9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1db9b-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1db9b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1db9b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1db9b-107">Prerequisites</span></span>
<span data-ttu-id="1db9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1db9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1db9b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1db9b-110">Permission type</span></span>|<span data-ttu-id="1db9b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1db9b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1db9b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1db9b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1db9b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="1db9b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="1db9b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1db9b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1db9b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1db9b-115">Not supported.</span></span>|
|<span data-ttu-id="1db9b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1db9b-116">Application</span></span>|<span data-ttu-id="1db9b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1db9b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1db9b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1db9b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="1db9b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1db9b-119">Request headers</span></span>
|<span data-ttu-id="1db9b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1db9b-120">Header</span></span>|<span data-ttu-id="1db9b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1db9b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1db9b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1db9b-122">Authorization</span></span>|<span data-ttu-id="1db9b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1db9b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1db9b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1db9b-124">Accept</span></span>|<span data-ttu-id="1db9b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1db9b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1db9b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1db9b-126">Request body</span></span>
<span data-ttu-id="1db9b-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1db9b-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1db9b-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1db9b-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1db9b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1db9b-129">Property</span></span>|<span data-ttu-id="1db9b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1db9b-130">Type</span></span>|<span data-ttu-id="1db9b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1db9b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1db9b-132">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="1db9b-132">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="1db9b-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="1db9b-133">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="1db9b-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1db9b-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1db9b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1db9b-135">Response</span></span>
<span data-ttu-id="1db9b-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1db9b-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1db9b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1db9b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1db9b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1db9b-138">Request</span></span>
<span data-ttu-id="1db9b-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1db9b-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1db9b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1db9b-140">Response</span></span>
<span data-ttu-id="1db9b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1db9b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





