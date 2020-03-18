---
title: Ação cleanWindowsDevice
description: Limpar dispositivo Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 532480a4f08a0edabdf6a3dc095070918aea5f44
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814292"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="242db-103">Ação cleanWindowsDevice</span><span class="sxs-lookup"><span data-stu-id="242db-103">cleanWindowsDevice action</span></span>

> <span data-ttu-id="242db-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="242db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="242db-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="242db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="242db-106">Limpar dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="242db-106">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="242db-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="242db-107">Prerequisites</span></span>
<span data-ttu-id="242db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="242db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="242db-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="242db-110">Permission type</span></span>|<span data-ttu-id="242db-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="242db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="242db-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="242db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="242db-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="242db-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="242db-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="242db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="242db-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="242db-115">Not supported.</span></span>|
|<span data-ttu-id="242db-116">Application</span><span class="sxs-lookup"><span data-stu-id="242db-116">Application</span></span>|<span data-ttu-id="242db-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="242db-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="242db-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="242db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="242db-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="242db-119">Request headers</span></span>
|<span data-ttu-id="242db-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="242db-120">Header</span></span>|<span data-ttu-id="242db-121">Valor</span><span class="sxs-lookup"><span data-stu-id="242db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="242db-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="242db-122">Authorization</span></span>|<span data-ttu-id="242db-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="242db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="242db-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="242db-124">Accept</span></span>|<span data-ttu-id="242db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="242db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="242db-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="242db-126">Request body</span></span>
<span data-ttu-id="242db-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="242db-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="242db-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="242db-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="242db-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="242db-129">Property</span></span>|<span data-ttu-id="242db-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="242db-130">Type</span></span>|<span data-ttu-id="242db-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="242db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="242db-132">keepUserData</span><span class="sxs-lookup"><span data-stu-id="242db-132">keepUserData</span></span>|<span data-ttu-id="242db-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="242db-133">Boolean</span></span>|<span data-ttu-id="242db-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="242db-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="242db-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="242db-135">Response</span></span>
<span data-ttu-id="242db-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="242db-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="242db-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="242db-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="242db-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="242db-138">Request</span></span>
<span data-ttu-id="242db-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="242db-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="242db-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="242db-140">Response</span></span>
<span data-ttu-id="242db-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="242db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




