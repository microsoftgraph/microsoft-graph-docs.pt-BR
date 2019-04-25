---
title: Ação rebootNow
description: Reinicie o dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 781742036efcb88141434c1763c6dd0a9daff37d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520274"
---
# <a name="rebootnow-action"></a><span data-ttu-id="045ee-103">Ação rebootNow</span><span class="sxs-lookup"><span data-stu-id="045ee-103">rebootNow action</span></span>

> <span data-ttu-id="045ee-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="045ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="045ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="045ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="045ee-106">Reinicie o dispositivo</span><span class="sxs-lookup"><span data-stu-id="045ee-106">Reboot device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="045ee-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="045ee-107">Prerequisites</span></span>
<span data-ttu-id="045ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="045ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="045ee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="045ee-110">Permission type</span></span>|<span data-ttu-id="045ee-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="045ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="045ee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="045ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="045ee-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="045ee-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="045ee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="045ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="045ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="045ee-115">Not supported.</span></span>|
|<span data-ttu-id="045ee-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="045ee-116">Application</span></span>|<span data-ttu-id="045ee-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="045ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="045ee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="045ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/rebootNow
```

## <a name="request-headers"></a><span data-ttu-id="045ee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="045ee-119">Request headers</span></span>
|<span data-ttu-id="045ee-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="045ee-120">Header</span></span>|<span data-ttu-id="045ee-121">Valor</span><span class="sxs-lookup"><span data-stu-id="045ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="045ee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="045ee-122">Authorization</span></span>|<span data-ttu-id="045ee-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="045ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="045ee-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="045ee-124">Accept</span></span>|<span data-ttu-id="045ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="045ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="045ee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="045ee-126">Request body</span></span>
<span data-ttu-id="045ee-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="045ee-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="045ee-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="045ee-128">Response</span></span>
<span data-ttu-id="045ee-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="045ee-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="045ee-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="045ee-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="045ee-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="045ee-131">Request</span></span>
<span data-ttu-id="045ee-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="045ee-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/rebootNow
```

### <a name="response"></a><span data-ttu-id="045ee-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="045ee-133">Response</span></span>
<span data-ttu-id="045ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="045ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





