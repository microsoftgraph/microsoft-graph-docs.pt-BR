---
title: Ação requestRemoteAssistance
description: Solicitar assistência remota
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04453110a7b324c9c07bf31298f6193a3b64904f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136381"
---
# <a name="requestremoteassistance-action"></a><span data-ttu-id="e2b52-103">Ação requestRemoteAssistance</span><span class="sxs-lookup"><span data-stu-id="e2b52-103">requestRemoteAssistance action</span></span>

<span data-ttu-id="e2b52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2b52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2b52-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2b52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2b52-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2b52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2b52-107">Solicitar assistência remota</span><span class="sxs-lookup"><span data-stu-id="e2b52-107">Request remote assistance</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2b52-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2b52-108">Prerequisites</span></span>
<span data-ttu-id="e2b52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2b52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2b52-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2b52-111">Permission type</span></span>|<span data-ttu-id="e2b52-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2b52-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2b52-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2b52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2b52-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2b52-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e2b52-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2b52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2b52-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2b52-116">Not supported.</span></span>|
|<span data-ttu-id="e2b52-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2b52-117">Application</span></span>|<span data-ttu-id="e2b52-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2b52-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2b52-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2b52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/comanagedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/requestRemoteAssistance
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/requestRemoteAssistance
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/requestRemoteAssistance
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

## <a name="request-headers"></a><span data-ttu-id="e2b52-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2b52-120">Request headers</span></span>
|<span data-ttu-id="e2b52-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2b52-121">Header</span></span>|<span data-ttu-id="e2b52-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e2b52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2b52-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2b52-123">Authorization</span></span>|<span data-ttu-id="e2b52-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2b52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2b52-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2b52-125">Accept</span></span>|<span data-ttu-id="e2b52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2b52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2b52-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2b52-127">Request body</span></span>
<span data-ttu-id="e2b52-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e2b52-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2b52-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2b52-129">Response</span></span>
<span data-ttu-id="e2b52-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e2b52-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e2b52-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2b52-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2b52-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2b52-132">Request</span></span>
<span data-ttu-id="e2b52-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2b52-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

### <a name="response"></a><span data-ttu-id="e2b52-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2b52-134">Response</span></span>
<span data-ttu-id="e2b52-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2b52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




