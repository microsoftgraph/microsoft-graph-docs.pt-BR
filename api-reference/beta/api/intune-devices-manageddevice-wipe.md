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
# <a name="wipe-action"></a><span data-ttu-id="d65db-103">ação wipe</span><span class="sxs-lookup"><span data-stu-id="d65db-103">wipe action</span></span>

<span data-ttu-id="d65db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d65db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d65db-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d65db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d65db-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d65db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d65db-107">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="d65db-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d65db-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d65db-108">Prerequisites</span></span>
<span data-ttu-id="d65db-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d65db-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d65db-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d65db-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d65db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d65db-111">Permission type</span></span>|<span data-ttu-id="d65db-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d65db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d65db-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d65db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d65db-114">DeviceManagementManagedDevices. PriviligedOperation. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d65db-114">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d65db-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d65db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d65db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d65db-116">Not supported.</span></span>|
|<span data-ttu-id="d65db-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d65db-117">Application</span></span>|<span data-ttu-id="d65db-118">DeviceManagementManagedDevices. PriviligedOperation. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d65db-118">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d65db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d65db-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d65db-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d65db-120">Request headers</span></span>
|<span data-ttu-id="d65db-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d65db-121">Header</span></span>|<span data-ttu-id="d65db-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d65db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d65db-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d65db-123">Authorization</span></span>|<span data-ttu-id="d65db-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d65db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d65db-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d65db-125">Accept</span></span>|<span data-ttu-id="d65db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d65db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d65db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d65db-127">Request body</span></span>
<span data-ttu-id="d65db-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d65db-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d65db-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d65db-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d65db-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d65db-130">Property</span></span>|<span data-ttu-id="d65db-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d65db-131">Type</span></span>|<span data-ttu-id="d65db-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d65db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d65db-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="d65db-133">keepEnrollmentData</span></span>|<span data-ttu-id="d65db-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="d65db-134">Boolean</span></span>|<span data-ttu-id="d65db-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d65db-135">Not yet documented</span></span>|
|<span data-ttu-id="d65db-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="d65db-136">keepUserData</span></span>|<span data-ttu-id="d65db-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="d65db-137">Boolean</span></span>|<span data-ttu-id="d65db-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d65db-138">Not yet documented</span></span>|
|<span data-ttu-id="d65db-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="d65db-139">macOsUnlockCode</span></span>|<span data-ttu-id="d65db-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d65db-140">String</span></span>|<span data-ttu-id="d65db-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d65db-141">Not yet documented</span></span>|
|<span data-ttu-id="d65db-142">useProtectedWipe</span><span class="sxs-lookup"><span data-stu-id="d65db-142">useProtectedWipe</span></span>|<span data-ttu-id="d65db-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="d65db-143">Boolean</span></span>|<span data-ttu-id="d65db-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d65db-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d65db-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d65db-145">Response</span></span>
<span data-ttu-id="d65db-146">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d65db-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d65db-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d65db-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d65db-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d65db-148">Request</span></span>
<span data-ttu-id="d65db-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d65db-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d65db-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d65db-150">Response</span></span>
<span data-ttu-id="d65db-151">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d65db-151">Here is an example of the response.</span></span> <span data-ttu-id="d65db-152">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d65db-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d65db-153">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d65db-153">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



