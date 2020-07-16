---
title: Ação windowsDefenderScan
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 63a32fd568ba5af56d15ee80ee8afec937248f7a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792146"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="35345-103">Ação windowsDefenderScan</span><span class="sxs-lookup"><span data-stu-id="35345-103">windowsDefenderScan action</span></span>

<span data-ttu-id="35345-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35345-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35345-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35345-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35345-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35345-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35345-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="35345-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35345-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="35345-108">Prerequisites</span></span>
<span data-ttu-id="35345-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35345-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35345-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35345-111">Permission type</span></span>|<span data-ttu-id="35345-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="35345-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35345-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35345-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35345-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="35345-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="35345-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35345-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35345-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35345-116">Not supported.</span></span>|
|<span data-ttu-id="35345-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35345-117">Application</span></span>|<span data-ttu-id="35345-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="35345-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35345-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35345-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="35345-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35345-120">Request headers</span></span>
|<span data-ttu-id="35345-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35345-121">Header</span></span>|<span data-ttu-id="35345-122">Valor</span><span class="sxs-lookup"><span data-stu-id="35345-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35345-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="35345-123">Authorization</span></span>|<span data-ttu-id="35345-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35345-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35345-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="35345-125">Accept</span></span>|<span data-ttu-id="35345-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35345-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35345-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35345-127">Request body</span></span>
<span data-ttu-id="35345-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="35345-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="35345-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="35345-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="35345-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35345-130">Property</span></span>|<span data-ttu-id="35345-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="35345-131">Type</span></span>|<span data-ttu-id="35345-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="35345-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35345-133">quickScan</span><span class="sxs-lookup"><span data-stu-id="35345-133">quickScan</span></span>|<span data-ttu-id="35345-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="35345-134">Boolean</span></span>|<span data-ttu-id="35345-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="35345-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="35345-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="35345-136">Response</span></span>
<span data-ttu-id="35345-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="35345-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="35345-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35345-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="35345-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35345-139">Request</span></span>
<span data-ttu-id="35345-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35345-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="35345-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="35345-141">Response</span></span>
<span data-ttu-id="35345-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35345-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



