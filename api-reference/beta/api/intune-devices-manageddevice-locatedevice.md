---
title: Ação locateDevice
description: Localizar um dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 773117ccae4f3c408012698de718d4ad19a128ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468982"
---
# <a name="locatedevice-action"></a><span data-ttu-id="f8885-103">Ação locateDevice</span><span class="sxs-lookup"><span data-stu-id="f8885-103">locateDevice action</span></span>

<span data-ttu-id="f8885-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f8885-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8885-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8885-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8885-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8885-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8885-107">Localizar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="f8885-107">Locate a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8885-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8885-108">Prerequisites</span></span>
<span data-ttu-id="f8885-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8885-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8885-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8885-111">Permission type</span></span>|<span data-ttu-id="f8885-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8885-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8885-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8885-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8885-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="f8885-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="f8885-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8885-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8885-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8885-116">Not supported.</span></span>|
|<span data-ttu-id="f8885-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8885-117">Application</span></span>|<span data-ttu-id="f8885-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="f8885-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8885-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8885-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/locateDevice
```

## <a name="request-headers"></a><span data-ttu-id="f8885-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8885-120">Request headers</span></span>
|<span data-ttu-id="f8885-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8885-121">Header</span></span>|<span data-ttu-id="f8885-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f8885-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8885-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8885-123">Authorization</span></span>|<span data-ttu-id="f8885-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8885-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8885-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8885-125">Accept</span></span>|<span data-ttu-id="f8885-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8885-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8885-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8885-127">Request body</span></span>
<span data-ttu-id="f8885-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8885-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8885-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8885-129">Response</span></span>
<span data-ttu-id="f8885-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f8885-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f8885-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8885-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8885-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8885-132">Request</span></span>
<span data-ttu-id="f8885-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8885-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/locateDevice
```

### <a name="response"></a><span data-ttu-id="f8885-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8885-134">Response</span></span>
<span data-ttu-id="f8885-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8885-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





