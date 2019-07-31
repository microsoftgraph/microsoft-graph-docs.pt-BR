---
title: Ação remoteLock
description: Bloqueio remoto
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60bef7349d74340e96c485bbe55a5e1c3ce21a95
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35981399"
---
# <a name="remotelock-action"></a><span data-ttu-id="970ea-103">Ação remoteLock</span><span class="sxs-lookup"><span data-stu-id="970ea-103">remoteLock action</span></span>

> <span data-ttu-id="970ea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="970ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="970ea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="970ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="970ea-106">Bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="970ea-106">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="970ea-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="970ea-107">Prerequisites</span></span>
<span data-ttu-id="970ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="970ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="970ea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="970ea-110">Permission type</span></span>|<span data-ttu-id="970ea-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="970ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="970ea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="970ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="970ea-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="970ea-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="970ea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="970ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="970ea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="970ea-115">Not supported.</span></span>|
|<span data-ttu-id="970ea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="970ea-116">Application</span></span>|<span data-ttu-id="970ea-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="970ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="970ea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="970ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/remoteLock
```

## <a name="request-headers"></a><span data-ttu-id="970ea-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="970ea-119">Request headers</span></span>
|<span data-ttu-id="970ea-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="970ea-120">Header</span></span>|<span data-ttu-id="970ea-121">Valor</span><span class="sxs-lookup"><span data-stu-id="970ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="970ea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="970ea-122">Authorization</span></span>|<span data-ttu-id="970ea-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="970ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="970ea-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="970ea-124">Accept</span></span>|<span data-ttu-id="970ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="970ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="970ea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="970ea-126">Request body</span></span>
<span data-ttu-id="970ea-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="970ea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="970ea-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="970ea-128">Response</span></span>
<span data-ttu-id="970ea-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="970ea-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="970ea-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="970ea-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="970ea-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="970ea-131">Request</span></span>
<span data-ttu-id="970ea-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="970ea-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="970ea-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="970ea-133">Response</span></span>
<span data-ttu-id="970ea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="970ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





