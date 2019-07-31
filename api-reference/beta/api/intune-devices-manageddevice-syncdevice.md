---
title: Ação syncDevice
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 697aa09ff303ad9c7a3d715c3b3a8148ed479501
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35981336"
---
# <a name="syncdevice-action"></a><span data-ttu-id="34773-103">Ação syncDevice</span><span class="sxs-lookup"><span data-stu-id="34773-103">syncDevice action</span></span>

> <span data-ttu-id="34773-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34773-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34773-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34773-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34773-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="34773-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34773-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34773-107">Prerequisites</span></span>
<span data-ttu-id="34773-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34773-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34773-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34773-110">Permission type</span></span>|<span data-ttu-id="34773-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34773-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34773-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34773-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34773-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="34773-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="34773-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34773-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34773-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34773-115">Not supported.</span></span>|
|<span data-ttu-id="34773-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34773-116">Application</span></span>|<span data-ttu-id="34773-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34773-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34773-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34773-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/syncDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/syncDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/syncDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/syncDevice
```

## <a name="request-headers"></a><span data-ttu-id="34773-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34773-119">Request headers</span></span>
|<span data-ttu-id="34773-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34773-120">Header</span></span>|<span data-ttu-id="34773-121">Valor</span><span class="sxs-lookup"><span data-stu-id="34773-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34773-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="34773-122">Authorization</span></span>|<span data-ttu-id="34773-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34773-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34773-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34773-124">Accept</span></span>|<span data-ttu-id="34773-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34773-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34773-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34773-126">Request body</span></span>
<span data-ttu-id="34773-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34773-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34773-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="34773-128">Response</span></span>
<span data-ttu-id="34773-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="34773-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="34773-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34773-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="34773-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34773-131">Request</span></span>
<span data-ttu-id="34773-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34773-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/syncDevice
```

### <a name="response"></a><span data-ttu-id="34773-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="34773-133">Response</span></span>
<span data-ttu-id="34773-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34773-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





