---
title: Ação shutDown
description: Desligar o dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 863384471fa29eec1bc0028930789f8704f8ceb6
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792174"
---
# <a name="shutdown-action"></a><span data-ttu-id="ff510-103">Ação shutDown</span><span class="sxs-lookup"><span data-stu-id="ff510-103">shutDown action</span></span>

<span data-ttu-id="ff510-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff510-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff510-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff510-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff510-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff510-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff510-107">Desligar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="ff510-107">Shut down device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff510-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff510-108">Prerequisites</span></span>
<span data-ttu-id="ff510-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff510-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff510-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff510-111">Permission type</span></span>|<span data-ttu-id="ff510-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff510-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff510-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff510-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff510-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ff510-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ff510-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff510-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff510-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff510-116">Not supported.</span></span>|
|<span data-ttu-id="ff510-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff510-117">Application</span></span>|<span data-ttu-id="ff510-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ff510-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff510-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff510-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/comanagedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/shutDown
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/shutDown
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/shutDown
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/shutDown
```

## <a name="request-headers"></a><span data-ttu-id="ff510-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff510-120">Request headers</span></span>
|<span data-ttu-id="ff510-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff510-121">Header</span></span>|<span data-ttu-id="ff510-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ff510-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff510-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff510-123">Authorization</span></span>|<span data-ttu-id="ff510-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff510-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff510-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff510-125">Accept</span></span>|<span data-ttu-id="ff510-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff510-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff510-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff510-127">Request body</span></span>
<span data-ttu-id="ff510-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff510-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff510-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff510-129">Response</span></span>
<span data-ttu-id="ff510-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ff510-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff510-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff510-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff510-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff510-132">Request</span></span>
<span data-ttu-id="ff510-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff510-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/shutDown
```

### <a name="response"></a><span data-ttu-id="ff510-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff510-134">Response</span></span>
<span data-ttu-id="ff510-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff510-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



