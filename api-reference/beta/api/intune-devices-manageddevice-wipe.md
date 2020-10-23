---
title: Ação wipe
description: Apagar um dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 86676dd636decb822cab5549f1fcc619c033f179
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704074"
---
# <a name="wipe-action"></a><span data-ttu-id="7427e-103">ação wipe</span><span class="sxs-lookup"><span data-stu-id="7427e-103">wipe action</span></span>

<span data-ttu-id="7427e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7427e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7427e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7427e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7427e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7427e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7427e-107">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="7427e-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7427e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7427e-108">Prerequisites</span></span>
<span data-ttu-id="7427e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7427e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7427e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7427e-111">Permission type</span></span>|<span data-ttu-id="7427e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7427e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7427e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7427e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7427e-114">DeviceManagementManagedDevices. PriviligedOperation. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7427e-114">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7427e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7427e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7427e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7427e-116">Not supported.</span></span>|
|<span data-ttu-id="7427e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7427e-117">Application</span></span>|<span data-ttu-id="7427e-118">DeviceManagementManagedDevices. PriviligedOperation. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7427e-118">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7427e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7427e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7427e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7427e-120">Request headers</span></span>
|<span data-ttu-id="7427e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7427e-121">Header</span></span>|<span data-ttu-id="7427e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7427e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7427e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7427e-123">Authorization</span></span>|<span data-ttu-id="7427e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7427e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7427e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7427e-125">Accept</span></span>|<span data-ttu-id="7427e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7427e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7427e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7427e-127">Request body</span></span>
<span data-ttu-id="7427e-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7427e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7427e-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7427e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7427e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7427e-130">Property</span></span>|<span data-ttu-id="7427e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7427e-131">Type</span></span>|<span data-ttu-id="7427e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7427e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7427e-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="7427e-133">keepEnrollmentData</span></span>|<span data-ttu-id="7427e-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="7427e-134">Boolean</span></span>|<span data-ttu-id="7427e-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7427e-135">Not yet documented</span></span>|
|<span data-ttu-id="7427e-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="7427e-136">keepUserData</span></span>|<span data-ttu-id="7427e-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="7427e-137">Boolean</span></span>|<span data-ttu-id="7427e-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7427e-138">Not yet documented</span></span>|
|<span data-ttu-id="7427e-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="7427e-139">macOsUnlockCode</span></span>|<span data-ttu-id="7427e-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7427e-140">String</span></span>|<span data-ttu-id="7427e-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7427e-141">Not yet documented</span></span>|
|<span data-ttu-id="7427e-142">useProtectedWipe</span><span class="sxs-lookup"><span data-stu-id="7427e-142">useProtectedWipe</span></span>|<span data-ttu-id="7427e-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="7427e-143">Boolean</span></span>|<span data-ttu-id="7427e-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7427e-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7427e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7427e-145">Response</span></span>
<span data-ttu-id="7427e-146">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7427e-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7427e-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7427e-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="7427e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7427e-148">Request</span></span>
<span data-ttu-id="7427e-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7427e-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7427e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7427e-150">Response</span></span>
<span data-ttu-id="7427e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7427e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





