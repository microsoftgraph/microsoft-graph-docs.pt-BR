---
title: Ação playLostModeSound
description: Bloqueio remoto
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1f1e6b13f4e778cf3cb6810b55a9019a64e46be
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792258"
---
# <a name="playlostmodesound-action"></a><span data-ttu-id="a2573-103">Ação playLostModeSound</span><span class="sxs-lookup"><span data-stu-id="a2573-103">playLostModeSound action</span></span>

<span data-ttu-id="a2573-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2573-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2573-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2573-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2573-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2573-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2573-107">Bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="a2573-107">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2573-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2573-108">Prerequisites</span></span>
<span data-ttu-id="a2573-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2573-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2573-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2573-111">Permission type</span></span>|<span data-ttu-id="a2573-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2573-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2573-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2573-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2573-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a2573-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a2573-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2573-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2573-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2573-116">Not supported.</span></span>|
|<span data-ttu-id="a2573-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2573-117">Application</span></span>|<span data-ttu-id="a2573-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a2573-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2573-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2573-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/comanagedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/playLostModeSound
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/playLostModeSound
```

## <a name="request-headers"></a><span data-ttu-id="a2573-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2573-120">Request headers</span></span>
|<span data-ttu-id="a2573-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2573-121">Header</span></span>|<span data-ttu-id="a2573-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a2573-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2573-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2573-123">Authorization</span></span>|<span data-ttu-id="a2573-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2573-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2573-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2573-125">Accept</span></span>|<span data-ttu-id="a2573-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2573-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2573-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2573-127">Request body</span></span>
<span data-ttu-id="a2573-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2573-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2573-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2573-129">Response</span></span>
<span data-ttu-id="a2573-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a2573-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a2573-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2573-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2573-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2573-132">Request</span></span>
<span data-ttu-id="a2573-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2573-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/playLostModeSound
```

### <a name="response"></a><span data-ttu-id="a2573-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2573-134">Response</span></span>
<span data-ttu-id="a2573-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2573-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



