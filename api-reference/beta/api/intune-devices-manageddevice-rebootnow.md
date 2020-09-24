---
title: Ação rebootNow
description: Reinicie o dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 458ddfe2b7571075c194ef28309f4d57b929b2eb
ms.sourcegitcommit: b7e82d0d64f640a09f5da76b38d8ed9f13684f95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2020
ms.locfileid: "48258419"
---
# <a name="rebootnow-action"></a><span data-ttu-id="2b6d4-103">Ação rebootNow</span><span class="sxs-lookup"><span data-stu-id="2b6d4-103">rebootNow action</span></span>

<span data-ttu-id="2b6d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b6d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> <span data-ttu-id="2b6d4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b6d4-106">Reinicialize o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-106">Reboot device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b6d4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b6d4-107">Prerequisites</span></span>
<span data-ttu-id="2b6d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b6d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b6d4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b6d4-110">Permission type</span></span>|<span data-ttu-id="2b6d4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b6d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b6d4-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b6d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2b6d4-113">DeviceManagementManagedDevices.PrivilegedOperations.All</span><span class="sxs-lookup"><span data-stu-id="2b6d4-113">DeviceManagementManagedDevices.PrivilegedOperations.All</span></span>|
|<span data-ttu-id="2b6d4-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b6d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b6d4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-115">Not supported.</span></span>|
|<span data-ttu-id="2b6d4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b6d4-116">Application</span></span>|<span data-ttu-id="2b6d4-117">DeviceManagementManagedDevices.PrivilegedOperations.All</span><span class="sxs-lookup"><span data-stu-id="2b6d4-117">DeviceManagementManagedDevices.PrivilegedOperations.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b6d4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b6d4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/comanagedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/rebootNow
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/rebootNow
```

## <a name="request-headers"></a><span data-ttu-id="2b6d4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b6d4-119">Request headers</span></span>
|<span data-ttu-id="2b6d4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b6d4-120">Header</span></span>|<span data-ttu-id="2b6d4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2b6d4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b6d4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b6d4-122">Authorization</span></span>|<span data-ttu-id="2b6d4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b6d4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b6d4-124">Accept</span></span>|<span data-ttu-id="2b6d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2b6d4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b6d4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b6d4-126">Request body</span></span>
<span data-ttu-id="2b6d4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b6d4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b6d4-128">Response</span></span>
<span data-ttu-id="2b6d4-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2b6d4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b6d4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b6d4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b6d4-131">Request</span></span>
<span data-ttu-id="2b6d4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/rebootNow
```

### <a name="response"></a><span data-ttu-id="2b6d4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b6d4-133">Response</span></span>
<span data-ttu-id="2b6d4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b6d4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






