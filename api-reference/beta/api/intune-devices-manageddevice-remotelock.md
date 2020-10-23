---
title: Ação remoteLock
description: Bloqueio remoto
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3c5ba66de80f6876f8bb2648429a3c843101bfb7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708225"
---
# <a name="remotelock-action"></a><span data-ttu-id="9d452-103">Ação remoteLock</span><span class="sxs-lookup"><span data-stu-id="9d452-103">remoteLock action</span></span>

<span data-ttu-id="9d452-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d452-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d452-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9d452-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d452-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d452-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d452-107">Bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="9d452-107">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d452-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9d452-108">Prerequisites</span></span>
<span data-ttu-id="9d452-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d452-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d452-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d452-111">Permission type</span></span>|<span data-ttu-id="9d452-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9d452-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d452-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d452-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d452-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9d452-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="9d452-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d452-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d452-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d452-116">Not supported.</span></span>|
|<span data-ttu-id="9d452-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d452-117">Application</span></span>|<span data-ttu-id="9d452-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9d452-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d452-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d452-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/comanagedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/remoteLock
```

## <a name="request-headers"></a><span data-ttu-id="9d452-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d452-120">Request headers</span></span>
|<span data-ttu-id="9d452-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9d452-121">Header</span></span>|<span data-ttu-id="9d452-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9d452-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d452-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d452-123">Authorization</span></span>|<span data-ttu-id="9d452-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d452-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d452-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9d452-125">Accept</span></span>|<span data-ttu-id="9d452-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d452-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d452-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d452-127">Request body</span></span>
<span data-ttu-id="9d452-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d452-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d452-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d452-129">Response</span></span>
<span data-ttu-id="9d452-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9d452-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9d452-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d452-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d452-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d452-132">Request</span></span>
<span data-ttu-id="9d452-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d452-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="9d452-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d452-134">Response</span></span>
<span data-ttu-id="9d452-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d452-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





