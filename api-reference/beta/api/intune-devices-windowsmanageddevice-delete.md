---
title: Excluir windowsManagedDevice
description: Exclui windowsManagedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 19c905fd5681eb4f9a93ffdcfddbdab5577dd891
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467813"
---
# <a name="delete-windowsmanageddevice"></a><span data-ttu-id="f98fa-103">Excluir windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="f98fa-103">Delete windowsManagedDevice</span></span>

<span data-ttu-id="f98fa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f98fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f98fa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f98fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f98fa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f98fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f98fa-107">Exclui [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f98fa-107">Deletes a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f98fa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f98fa-108">Prerequisites</span></span>
<span data-ttu-id="f98fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f98fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f98fa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f98fa-111">Permission type</span></span>|<span data-ttu-id="f98fa-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f98fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f98fa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f98fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f98fa-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f98fa-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f98fa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f98fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f98fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f98fa-116">Not supported.</span></span>|
|<span data-ttu-id="f98fa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f98fa-117">Application</span></span>|<span data-ttu-id="f98fa-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f98fa-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f98fa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f98fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/managedDevices/{managedDeviceId}
DELETE /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="f98fa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f98fa-120">Request headers</span></span>
|<span data-ttu-id="f98fa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f98fa-121">Header</span></span>|<span data-ttu-id="f98fa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f98fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f98fa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f98fa-123">Authorization</span></span>|<span data-ttu-id="f98fa-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f98fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f98fa-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f98fa-125">Accept</span></span>|<span data-ttu-id="f98fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f98fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f98fa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f98fa-127">Request body</span></span>
<span data-ttu-id="f98fa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f98fa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f98fa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f98fa-129">Response</span></span>
<span data-ttu-id="f98fa-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f98fa-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f98fa-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f98fa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f98fa-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f98fa-132">Request</span></span>
<span data-ttu-id="f98fa-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f98fa-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
```

### <a name="response"></a><span data-ttu-id="f98fa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f98fa-134">Response</span></span>
<span data-ttu-id="f98fa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f98fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





