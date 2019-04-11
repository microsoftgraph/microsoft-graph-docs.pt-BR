---
title: Ação cleanWindowsDevice
description: Limpar dispositivo Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68775825b67e6e6410f5159f1a43b1dc3f248bb6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785843"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="6c98e-103">Ação cleanWindowsDevice</span><span class="sxs-lookup"><span data-stu-id="6c98e-103">cleanWindowsDevice action</span></span>

> <span data-ttu-id="6c98e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c98e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c98e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c98e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c98e-106">Limpar dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="6c98e-106">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c98e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c98e-107">Prerequisites</span></span>
<span data-ttu-id="6c98e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c98e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c98e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c98e-110">Permission type</span></span>|<span data-ttu-id="6c98e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c98e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c98e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c98e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c98e-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6c98e-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="6c98e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c98e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c98e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c98e-115">Not supported.</span></span>|
|<span data-ttu-id="6c98e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c98e-116">Application</span></span>|<span data-ttu-id="6c98e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c98e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c98e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c98e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="6c98e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c98e-119">Request headers</span></span>
|<span data-ttu-id="6c98e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c98e-120">Header</span></span>|<span data-ttu-id="6c98e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6c98e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c98e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c98e-122">Authorization</span></span>|<span data-ttu-id="6c98e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c98e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c98e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c98e-124">Accept</span></span>|<span data-ttu-id="6c98e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c98e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c98e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c98e-126">Request body</span></span>
<span data-ttu-id="6c98e-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6c98e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6c98e-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="6c98e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6c98e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c98e-129">Property</span></span>|<span data-ttu-id="6c98e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c98e-130">Type</span></span>|<span data-ttu-id="6c98e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c98e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c98e-132">keepUserData</span><span class="sxs-lookup"><span data-stu-id="6c98e-132">keepUserData</span></span>|<span data-ttu-id="6c98e-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c98e-133">Boolean</span></span>|<span data-ttu-id="6c98e-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6c98e-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6c98e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c98e-135">Response</span></span>
<span data-ttu-id="6c98e-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6c98e-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6c98e-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c98e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c98e-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c98e-138">Request</span></span>
<span data-ttu-id="6c98e-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c98e-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="6c98e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c98e-140">Response</span></span>
<span data-ttu-id="6c98e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c98e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





