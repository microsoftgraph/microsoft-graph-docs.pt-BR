---
title: Ação updateWindowsDeviceAccount
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9492d1a36f571b253b77e85d2ea631399c845805
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519889"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="f2565-103">Ação updateWindowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="f2565-103">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="f2565-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2565-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2565-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2565-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2565-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2565-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2565-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2565-107">Prerequisites</span></span>
<span data-ttu-id="f2565-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2565-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2565-110">Permission type</span></span>|<span data-ttu-id="f2565-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2565-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2565-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2565-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2565-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="f2565-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="f2565-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2565-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2565-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2565-115">Not supported.</span></span>|
|<span data-ttu-id="f2565-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2565-116">Application</span></span>|<span data-ttu-id="f2565-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2565-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2565-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2565-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f2565-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2565-119">Request headers</span></span>
|<span data-ttu-id="f2565-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2565-120">Header</span></span>|<span data-ttu-id="f2565-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f2565-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2565-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2565-122">Authorization</span></span>|<span data-ttu-id="f2565-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2565-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2565-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2565-124">Accept</span></span>|<span data-ttu-id="f2565-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f2565-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2565-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2565-126">Request body</span></span>
<span data-ttu-id="f2565-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f2565-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f2565-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f2565-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f2565-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2565-129">Property</span></span>|<span data-ttu-id="f2565-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2565-130">Type</span></span>|<span data-ttu-id="f2565-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2565-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2565-132">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="f2565-132">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="f2565-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="f2565-133">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="f2565-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2565-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f2565-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2565-135">Response</span></span>
<span data-ttu-id="f2565-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f2565-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f2565-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2565-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2565-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2565-138">Request</span></span>
<span data-ttu-id="f2565-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2565-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f2565-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2565-140">Response</span></span>
<span data-ttu-id="f2565-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2565-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





