---
title: Ação syncDevice
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 12382d8639a3e211cf634199712efe813074bb4f
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556181"
---
# <a name="syncdevice-action"></a><span data-ttu-id="26723-103">Ação syncDevice</span><span class="sxs-lookup"><span data-stu-id="26723-103">syncDevice action</span></span>

<span data-ttu-id="26723-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26723-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26723-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26723-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26723-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26723-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26723-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="26723-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26723-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26723-108">Prerequisites</span></span>
<span data-ttu-id="26723-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26723-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26723-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26723-111">Permission type</span></span>|<span data-ttu-id="26723-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26723-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26723-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26723-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26723-114">DeviceManagementManagedDevices.PrivilegedOperations.All</span><span class="sxs-lookup"><span data-stu-id="26723-114">DeviceManagementManagedDevices.PrivilegedOperations.All</span></span>|
|<span data-ttu-id="26723-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26723-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26723-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26723-116">Not supported.</span></span>|
|<span data-ttu-id="26723-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26723-117">Application</span></span>|<span data-ttu-id="26723-118">DeviceManagementManagedDevices.PrivilegedOperations.All</span><span class="sxs-lookup"><span data-stu-id="26723-118">DeviceManagementManagedDevices.PrivilegedOperations.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26723-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26723-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/syncDevice
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/syncDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/syncDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/syncDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/syncDevice
```

## <a name="request-headers"></a><span data-ttu-id="26723-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26723-120">Request headers</span></span>
|<span data-ttu-id="26723-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26723-121">Header</span></span>|<span data-ttu-id="26723-122">Valor</span><span class="sxs-lookup"><span data-stu-id="26723-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26723-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="26723-123">Authorization</span></span>|<span data-ttu-id="26723-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26723-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26723-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26723-125">Accept</span></span>|<span data-ttu-id="26723-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26723-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26723-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26723-127">Request body</span></span>
<span data-ttu-id="26723-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26723-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26723-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="26723-129">Response</span></span>
<span data-ttu-id="26723-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="26723-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="26723-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26723-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="26723-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26723-132">Request</span></span>
<span data-ttu-id="26723-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26723-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/syncDevice
```

### <a name="response"></a><span data-ttu-id="26723-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="26723-134">Response</span></span>
<span data-ttu-id="26723-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26723-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



