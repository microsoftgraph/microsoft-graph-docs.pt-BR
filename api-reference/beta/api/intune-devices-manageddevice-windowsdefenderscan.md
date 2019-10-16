---
title: Ação windowsDefenderScan
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 654b637b717f52e2c41bfe8bfb9d54cd1ad11dfa
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37528154"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="7743a-103">Ação windowsDefenderScan</span><span class="sxs-lookup"><span data-stu-id="7743a-103">windowsDefenderScan action</span></span>

> <span data-ttu-id="7743a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7743a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7743a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7743a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7743a-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7743a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7743a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7743a-107">Prerequisites</span></span>
<span data-ttu-id="7743a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7743a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7743a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7743a-110">Permission type</span></span>|<span data-ttu-id="7743a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7743a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7743a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7743a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7743a-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="7743a-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="7743a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7743a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7743a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7743a-115">Not supported.</span></span>|
|<span data-ttu-id="7743a-116">Application</span><span class="sxs-lookup"><span data-stu-id="7743a-116">Application</span></span>|<span data-ttu-id="7743a-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="7743a-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7743a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7743a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="7743a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7743a-119">Request headers</span></span>
|<span data-ttu-id="7743a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7743a-120">Header</span></span>|<span data-ttu-id="7743a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7743a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7743a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7743a-122">Authorization</span></span>|<span data-ttu-id="7743a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7743a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7743a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7743a-124">Accept</span></span>|<span data-ttu-id="7743a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7743a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7743a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7743a-126">Request body</span></span>
<span data-ttu-id="7743a-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7743a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7743a-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7743a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7743a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7743a-129">Property</span></span>|<span data-ttu-id="7743a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7743a-130">Type</span></span>|<span data-ttu-id="7743a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7743a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7743a-132">quickScan</span><span class="sxs-lookup"><span data-stu-id="7743a-132">quickScan</span></span>|<span data-ttu-id="7743a-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="7743a-133">Boolean</span></span>|<span data-ttu-id="7743a-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7743a-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7743a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7743a-135">Response</span></span>
<span data-ttu-id="7743a-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7743a-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7743a-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7743a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7743a-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7743a-138">Request</span></span>
<span data-ttu-id="7743a-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7743a-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="7743a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7743a-140">Response</span></span>
<span data-ttu-id="7743a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7743a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






