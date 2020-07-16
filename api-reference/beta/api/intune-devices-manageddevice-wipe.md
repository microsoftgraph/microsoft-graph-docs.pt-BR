---
title: Ação wipe
description: Apagar um dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ea07fd650a00e91896639d0312b48bb787b2b54
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792124"
---
# <a name="wipe-action"></a><span data-ttu-id="db7b9-103">ação wipe</span><span class="sxs-lookup"><span data-stu-id="db7b9-103">wipe action</span></span>

<span data-ttu-id="db7b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db7b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db7b9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db7b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db7b9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db7b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db7b9-107">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="db7b9-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db7b9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db7b9-108">Prerequisites</span></span>
<span data-ttu-id="db7b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db7b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db7b9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db7b9-111">Permission type</span></span>|<span data-ttu-id="db7b9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="db7b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db7b9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db7b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db7b9-114">DeviceManagementManagedDevices. PriviligedOperation. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="db7b9-114">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="db7b9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db7b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db7b9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db7b9-116">Not supported.</span></span>|
|<span data-ttu-id="db7b9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db7b9-117">Application</span></span>|<span data-ttu-id="db7b9-118">DeviceManagementManagedDevices. PriviligedOperation. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="db7b9-118">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db7b9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db7b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/comanagedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="db7b9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db7b9-120">Request headers</span></span>
|<span data-ttu-id="db7b9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db7b9-121">Header</span></span>|<span data-ttu-id="db7b9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="db7b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db7b9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="db7b9-123">Authorization</span></span>|<span data-ttu-id="db7b9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db7b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db7b9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db7b9-125">Accept</span></span>|<span data-ttu-id="db7b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db7b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db7b9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db7b9-127">Request body</span></span>
<span data-ttu-id="db7b9-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="db7b9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="db7b9-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="db7b9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="db7b9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db7b9-130">Property</span></span>|<span data-ttu-id="db7b9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="db7b9-131">Type</span></span>|<span data-ttu-id="db7b9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="db7b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db7b9-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="db7b9-133">keepEnrollmentData</span></span>|<span data-ttu-id="db7b9-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="db7b9-134">Boolean</span></span>|<span data-ttu-id="db7b9-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="db7b9-135">Not yet documented</span></span>|
|<span data-ttu-id="db7b9-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="db7b9-136">keepUserData</span></span>|<span data-ttu-id="db7b9-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="db7b9-137">Boolean</span></span>|<span data-ttu-id="db7b9-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="db7b9-138">Not yet documented</span></span>|
|<span data-ttu-id="db7b9-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="db7b9-139">macOsUnlockCode</span></span>|<span data-ttu-id="db7b9-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db7b9-140">String</span></span>|<span data-ttu-id="db7b9-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="db7b9-141">Not yet documented</span></span>|
|<span data-ttu-id="db7b9-142">useProtectedWipe</span><span class="sxs-lookup"><span data-stu-id="db7b9-142">useProtectedWipe</span></span>|<span data-ttu-id="db7b9-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="db7b9-143">Boolean</span></span>|<span data-ttu-id="db7b9-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="db7b9-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="db7b9-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="db7b9-145">Response</span></span>
<span data-ttu-id="db7b9-146">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="db7b9-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="db7b9-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db7b9-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="db7b9-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db7b9-148">Request</span></span>
<span data-ttu-id="db7b9-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db7b9-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 138

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value",
  "useProtectedWipe": true
}
```

### <a name="response"></a><span data-ttu-id="db7b9-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="db7b9-150">Response</span></span>
<span data-ttu-id="db7b9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db7b9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



