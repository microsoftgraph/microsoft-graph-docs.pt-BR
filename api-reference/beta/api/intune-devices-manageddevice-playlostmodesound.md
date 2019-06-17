---
title: Ação playLostModeSound
description: Bloqueio remoto
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d68be90221644defb4761ca41dfa00d4bfede02
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958379"
---
# <a name="playlostmodesound-action"></a><span data-ttu-id="3accc-103">Ação playLostModeSound</span><span class="sxs-lookup"><span data-stu-id="3accc-103">playLostModeSound action</span></span>

> <span data-ttu-id="3accc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3accc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3accc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3accc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3accc-106">Bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="3accc-106">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3accc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3accc-107">Prerequisites</span></span>
<span data-ttu-id="3accc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3accc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3accc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3accc-110">Permission type</span></span>|<span data-ttu-id="3accc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3accc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3accc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3accc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3accc-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="3accc-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="3accc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3accc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3accc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3accc-115">Not supported.</span></span>|
|<span data-ttu-id="3accc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3accc-116">Application</span></span>|<span data-ttu-id="3accc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3accc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3accc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3accc-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="3accc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3accc-119">Request headers</span></span>
|<span data-ttu-id="3accc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3accc-120">Header</span></span>|<span data-ttu-id="3accc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3accc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3accc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3accc-122">Authorization</span></span>|<span data-ttu-id="3accc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3accc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3accc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3accc-124">Accept</span></span>|<span data-ttu-id="3accc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3accc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3accc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3accc-126">Request body</span></span>
<span data-ttu-id="3accc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3accc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3accc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3accc-128">Response</span></span>
<span data-ttu-id="3accc-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3accc-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3accc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3accc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3accc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3accc-131">Request</span></span>
<span data-ttu-id="3accc-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3accc-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/playLostModeSound
```

### <a name="response"></a><span data-ttu-id="3accc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3accc-133">Response</span></span>
<span data-ttu-id="3accc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3accc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





