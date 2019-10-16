---
title: Ação bypassActivationLock
description: Ignorar bloqueio de ativação
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0474a3783563132ded53aa2ee3bd162b455887a7
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37530101"
---
# <a name="bypassactivationlock-action"></a><span data-ttu-id="c7ef8-103">Ação bypassActivationLock</span><span class="sxs-lookup"><span data-stu-id="c7ef8-103">bypassActivationLock action</span></span>

> <span data-ttu-id="c7ef8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7ef8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7ef8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7ef8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7ef8-106">Ignorar bloqueio de ativação</span><span class="sxs-lookup"><span data-stu-id="c7ef8-106">Bypass activation lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7ef8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7ef8-107">Prerequisites</span></span>
<span data-ttu-id="c7ef8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7ef8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7ef8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7ef8-110">Permission type</span></span>|<span data-ttu-id="c7ef8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7ef8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7ef8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7ef8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7ef8-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c7ef8-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="c7ef8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7ef8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7ef8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7ef8-115">Not supported.</span></span>|
|<span data-ttu-id="c7ef8-116">Application</span><span class="sxs-lookup"><span data-stu-id="c7ef8-116">Application</span></span>|<span data-ttu-id="c7ef8-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c7ef8-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7ef8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7ef8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/bypassActivationLock
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/bypassActivationLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/bypassActivationLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/bypassActivationLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/bypassActivationLock
```

## <a name="request-headers"></a><span data-ttu-id="c7ef8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7ef8-119">Request headers</span></span>
|<span data-ttu-id="c7ef8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7ef8-120">Header</span></span>|<span data-ttu-id="c7ef8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c7ef8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7ef8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7ef8-122">Authorization</span></span>|<span data-ttu-id="c7ef8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7ef8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7ef8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7ef8-124">Accept</span></span>|<span data-ttu-id="c7ef8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7ef8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7ef8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7ef8-126">Request body</span></span>
<span data-ttu-id="c7ef8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7ef8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7ef8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7ef8-128">Response</span></span>
<span data-ttu-id="c7ef8-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c7ef8-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c7ef8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7ef8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7ef8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7ef8-131">Request</span></span>
<span data-ttu-id="c7ef8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7ef8-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/bypassActivationLock
```

### <a name="response"></a><span data-ttu-id="c7ef8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7ef8-133">Response</span></span>
<span data-ttu-id="c7ef8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7ef8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






