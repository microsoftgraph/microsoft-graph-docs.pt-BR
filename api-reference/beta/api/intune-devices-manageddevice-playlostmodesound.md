---
title: Ação playLostModeSound
description: Bloqueio remoto
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 46820900dd45fc614755438349660d0757269625
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180346"
---
# <a name="playlostmodesound-action"></a><span data-ttu-id="e6888-103">Ação playLostModeSound</span><span class="sxs-lookup"><span data-stu-id="e6888-103">playLostModeSound action</span></span>

> <span data-ttu-id="e6888-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6888-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6888-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6888-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6888-106">Bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="e6888-106">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6888-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6888-107">Prerequisites</span></span>
<span data-ttu-id="e6888-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6888-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6888-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6888-110">Permission type</span></span>|<span data-ttu-id="e6888-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e6888-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6888-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6888-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6888-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e6888-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e6888-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6888-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6888-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6888-115">Not supported.</span></span>|
|<span data-ttu-id="e6888-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6888-116">Application</span></span>|<span data-ttu-id="e6888-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e6888-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6888-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6888-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/playLostModeSound
```

## <a name="request-headers"></a><span data-ttu-id="e6888-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6888-119">Request headers</span></span>
|<span data-ttu-id="e6888-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6888-120">Header</span></span>|<span data-ttu-id="e6888-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e6888-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6888-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6888-122">Authorization</span></span>|<span data-ttu-id="e6888-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6888-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6888-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6888-124">Accept</span></span>|<span data-ttu-id="e6888-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6888-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6888-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6888-126">Request body</span></span>
<span data-ttu-id="e6888-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6888-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6888-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6888-128">Response</span></span>
<span data-ttu-id="e6888-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e6888-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e6888-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6888-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6888-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6888-131">Request</span></span>
<span data-ttu-id="e6888-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6888-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/playLostModeSound
```

### <a name="response"></a><span data-ttu-id="e6888-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6888-133">Response</span></span>
<span data-ttu-id="e6888-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6888-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




