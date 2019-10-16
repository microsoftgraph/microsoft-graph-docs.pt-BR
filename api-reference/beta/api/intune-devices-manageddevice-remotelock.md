---
title: Ação remoteLock
description: Bloqueio remoto
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e3cbe79f751d481cf7f36f568803532871e7768
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37528840"
---
# <a name="remotelock-action"></a><span data-ttu-id="2bc3e-103">Ação remoteLock</span><span class="sxs-lookup"><span data-stu-id="2bc3e-103">remoteLock action</span></span>

> <span data-ttu-id="2bc3e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2bc3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bc3e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2bc3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bc3e-106">Bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="2bc3e-106">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bc3e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2bc3e-107">Prerequisites</span></span>
<span data-ttu-id="2bc3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bc3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bc3e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bc3e-110">Permission type</span></span>|<span data-ttu-id="2bc3e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2bc3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bc3e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bc3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bc3e-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="2bc3e-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="2bc3e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bc3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bc3e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bc3e-115">Not supported.</span></span>|
|<span data-ttu-id="2bc3e-116">Application</span><span class="sxs-lookup"><span data-stu-id="2bc3e-116">Application</span></span>|<span data-ttu-id="2bc3e-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="2bc3e-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bc3e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bc3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/remoteLock
```

## <a name="request-headers"></a><span data-ttu-id="2bc3e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bc3e-119">Request headers</span></span>
|<span data-ttu-id="2bc3e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2bc3e-120">Header</span></span>|<span data-ttu-id="2bc3e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2bc3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bc3e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bc3e-122">Authorization</span></span>|<span data-ttu-id="2bc3e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bc3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bc3e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2bc3e-124">Accept</span></span>|<span data-ttu-id="2bc3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2bc3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bc3e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bc3e-126">Request body</span></span>
<span data-ttu-id="2bc3e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2bc3e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bc3e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bc3e-128">Response</span></span>
<span data-ttu-id="2bc3e-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2bc3e-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2bc3e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bc3e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bc3e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bc3e-131">Request</span></span>
<span data-ttu-id="2bc3e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bc3e-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="2bc3e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bc3e-133">Response</span></span>
<span data-ttu-id="2bc3e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bc3e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






