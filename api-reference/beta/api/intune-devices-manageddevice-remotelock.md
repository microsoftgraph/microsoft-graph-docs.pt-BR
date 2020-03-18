---
title: Ação remoteLock
description: Bloqueio remoto
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35e091cec3a46b0d475ebe590713f295ef2139a2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775132"
---
# <a name="remotelock-action"></a><span data-ttu-id="cd86b-103">Ação remoteLock</span><span class="sxs-lookup"><span data-stu-id="cd86b-103">remoteLock action</span></span>

> <span data-ttu-id="cd86b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cd86b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd86b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd86b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd86b-106">Bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="cd86b-106">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd86b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cd86b-107">Prerequisites</span></span>
<span data-ttu-id="cd86b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd86b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd86b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd86b-110">Permission type</span></span>|<span data-ttu-id="cd86b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cd86b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd86b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd86b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd86b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="cd86b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="cd86b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd86b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd86b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd86b-115">Not supported.</span></span>|
|<span data-ttu-id="cd86b-116">Application</span><span class="sxs-lookup"><span data-stu-id="cd86b-116">Application</span></span>|<span data-ttu-id="cd86b-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="cd86b-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd86b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd86b-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="cd86b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd86b-119">Request headers</span></span>
|<span data-ttu-id="cd86b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd86b-120">Header</span></span>|<span data-ttu-id="cd86b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cd86b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd86b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd86b-122">Authorization</span></span>|<span data-ttu-id="cd86b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd86b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd86b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cd86b-124">Accept</span></span>|<span data-ttu-id="cd86b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd86b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd86b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd86b-126">Request body</span></span>
<span data-ttu-id="cd86b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd86b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd86b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd86b-128">Response</span></span>
<span data-ttu-id="cd86b-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cd86b-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd86b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd86b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd86b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd86b-131">Request</span></span>
<span data-ttu-id="cd86b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd86b-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="cd86b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd86b-133">Response</span></span>
<span data-ttu-id="cd86b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd86b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




