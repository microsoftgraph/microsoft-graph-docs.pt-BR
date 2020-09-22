---
title: Ação windowsDefenderScan
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2f0f26cc0f0694358d01b746293c1c0660cc583
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072442"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="d9907-103">Ação windowsDefenderScan</span><span class="sxs-lookup"><span data-stu-id="d9907-103">windowsDefenderScan action</span></span>

<span data-ttu-id="d9907-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9907-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9907-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9907-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9907-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9907-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9907-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d9907-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9907-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9907-108">Prerequisites</span></span>
<span data-ttu-id="d9907-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9907-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9907-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9907-111">Permission type</span></span>|<span data-ttu-id="d9907-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9907-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9907-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9907-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9907-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="d9907-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="d9907-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9907-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9907-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9907-116">Not supported.</span></span>|
|<span data-ttu-id="d9907-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9907-117">Application</span></span>|<span data-ttu-id="d9907-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="d9907-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9907-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9907-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/comanagedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsDefenderScan
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="d9907-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9907-120">Request headers</span></span>
|<span data-ttu-id="d9907-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9907-121">Header</span></span>|<span data-ttu-id="d9907-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d9907-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9907-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9907-123">Authorization</span></span>|<span data-ttu-id="d9907-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9907-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9907-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9907-125">Accept</span></span>|<span data-ttu-id="d9907-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9907-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9907-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9907-127">Request body</span></span>
<span data-ttu-id="d9907-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d9907-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d9907-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d9907-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d9907-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9907-130">Property</span></span>|<span data-ttu-id="d9907-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9907-131">Type</span></span>|<span data-ttu-id="d9907-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9907-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9907-133">quickScan</span><span class="sxs-lookup"><span data-stu-id="d9907-133">quickScan</span></span>|<span data-ttu-id="d9907-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9907-134">Boolean</span></span>|<span data-ttu-id="d9907-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d9907-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d9907-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9907-136">Response</span></span>
<span data-ttu-id="d9907-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d9907-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d9907-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9907-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9907-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9907-139">Request</span></span>
<span data-ttu-id="d9907-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9907-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="d9907-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9907-141">Response</span></span>
<span data-ttu-id="d9907-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9907-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






