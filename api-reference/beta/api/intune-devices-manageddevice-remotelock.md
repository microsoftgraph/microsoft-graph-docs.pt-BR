---
title: Ação remoteLock
description: Bloqueio remoto
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e611d90c0e453b6e82f436d386f7df79d889b510
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157201"
---
# <a name="remotelock-action"></a><span data-ttu-id="5d81a-103">Ação remoteLock</span><span class="sxs-lookup"><span data-stu-id="5d81a-103">remoteLock action</span></span>

> <span data-ttu-id="5d81a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5d81a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d81a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5d81a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d81a-106">Bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="5d81a-106">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d81a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5d81a-107">Prerequisites</span></span>
<span data-ttu-id="5d81a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d81a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5d81a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d81a-110">Permission type</span></span>|<span data-ttu-id="5d81a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5d81a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d81a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d81a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5d81a-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="5d81a-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="5d81a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d81a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d81a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d81a-115">Not supported.</span></span>|
|<span data-ttu-id="5d81a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d81a-116">Application</span></span>|<span data-ttu-id="5d81a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d81a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d81a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d81a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/remoteLock
```

## <a name="request-headers"></a><span data-ttu-id="5d81a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d81a-119">Request headers</span></span>
|<span data-ttu-id="5d81a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5d81a-120">Header</span></span>|<span data-ttu-id="5d81a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5d81a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d81a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d81a-122">Authorization</span></span>|<span data-ttu-id="5d81a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d81a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d81a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5d81a-124">Accept</span></span>|<span data-ttu-id="5d81a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5d81a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d81a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d81a-126">Request body</span></span>
<span data-ttu-id="5d81a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d81a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d81a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d81a-128">Response</span></span>
<span data-ttu-id="5d81a-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5d81a-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5d81a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d81a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d81a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d81a-131">Request</span></span>
<span data-ttu-id="5d81a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d81a-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="5d81a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d81a-133">Response</span></span>
<span data-ttu-id="5d81a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d81a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




