---
title: Ação shutDown
description: Desligar o dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd41fae748d25407893860923dfb1dfe09e406e4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136248"
---
# <a name="shutdown-action"></a><span data-ttu-id="c9347-103">Ação shutDown</span><span class="sxs-lookup"><span data-stu-id="c9347-103">shutDown action</span></span>

<span data-ttu-id="c9347-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9347-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9347-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c9347-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9347-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9347-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9347-107">Desligar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="c9347-107">Shut down device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9347-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c9347-108">Prerequisites</span></span>
<span data-ttu-id="c9347-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9347-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9347-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9347-111">Permission type</span></span>|<span data-ttu-id="c9347-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9347-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9347-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9347-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9347-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c9347-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="c9347-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9347-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9347-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9347-116">Not supported.</span></span>|
|<span data-ttu-id="c9347-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9347-117">Application</span></span>|<span data-ttu-id="c9347-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c9347-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9347-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9347-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c9347-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9347-120">Request headers</span></span>
|<span data-ttu-id="c9347-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9347-121">Header</span></span>|<span data-ttu-id="c9347-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c9347-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9347-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9347-123">Authorization</span></span>|<span data-ttu-id="c9347-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9347-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9347-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c9347-125">Accept</span></span>|<span data-ttu-id="c9347-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9347-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9347-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9347-127">Request body</span></span>
<span data-ttu-id="c9347-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9347-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9347-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9347-129">Response</span></span>
<span data-ttu-id="c9347-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c9347-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c9347-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9347-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9347-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9347-132">Request</span></span>
<span data-ttu-id="c9347-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9347-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/shutDown
```

### <a name="response"></a><span data-ttu-id="c9347-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9347-134">Response</span></span>
<span data-ttu-id="c9347-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9347-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




