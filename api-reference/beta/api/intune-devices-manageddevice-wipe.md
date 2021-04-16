---
title: Ação wipe
description: Apagar um dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 760631b115d6a458556b476b28f6f996e259d2bd
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866619"
---
# <a name="wipe-action"></a><span data-ttu-id="1bc70-103">ação wipe</span><span class="sxs-lookup"><span data-stu-id="1bc70-103">wipe action</span></span>

<span data-ttu-id="1bc70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bc70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bc70-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1bc70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bc70-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bc70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bc70-107">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="1bc70-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bc70-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1bc70-108">Prerequisites</span></span>
<span data-ttu-id="1bc70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bc70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bc70-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bc70-111">Permission type</span></span>|<span data-ttu-id="1bc70-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1bc70-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bc70-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bc70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bc70-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="1bc70-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="1bc70-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bc70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bc70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bc70-116">Not supported.</span></span>|
|<span data-ttu-id="1bc70-117">Application</span><span class="sxs-lookup"><span data-stu-id="1bc70-117">Application</span></span>|<span data-ttu-id="1bc70-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="1bc70-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bc70-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bc70-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1bc70-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bc70-120">Request headers</span></span>
|<span data-ttu-id="1bc70-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bc70-121">Header</span></span>|<span data-ttu-id="1bc70-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1bc70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bc70-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bc70-123">Authorization</span></span>|<span data-ttu-id="1bc70-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bc70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bc70-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1bc70-125">Accept</span></span>|<span data-ttu-id="1bc70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bc70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bc70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bc70-127">Request body</span></span>
<span data-ttu-id="1bc70-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1bc70-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1bc70-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1bc70-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1bc70-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bc70-130">Property</span></span>|<span data-ttu-id="1bc70-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bc70-131">Type</span></span>|<span data-ttu-id="1bc70-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bc70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bc70-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="1bc70-133">keepEnrollmentData</span></span>|<span data-ttu-id="1bc70-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="1bc70-134">Boolean</span></span>|<span data-ttu-id="1bc70-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1bc70-135">Not yet documented</span></span>|
|<span data-ttu-id="1bc70-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="1bc70-136">keepUserData</span></span>|<span data-ttu-id="1bc70-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="1bc70-137">Boolean</span></span>|<span data-ttu-id="1bc70-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1bc70-138">Not yet documented</span></span>|
|<span data-ttu-id="1bc70-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="1bc70-139">macOsUnlockCode</span></span>|<span data-ttu-id="1bc70-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bc70-140">String</span></span>|<span data-ttu-id="1bc70-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1bc70-141">Not yet documented</span></span>|
|<span data-ttu-id="1bc70-142">persistEsimDataPlan</span><span class="sxs-lookup"><span data-stu-id="1bc70-142">persistEsimDataPlan</span></span>|<span data-ttu-id="1bc70-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="1bc70-143">Boolean</span></span>|<span data-ttu-id="1bc70-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1bc70-144">Not yet documented</span></span>|
|<span data-ttu-id="1bc70-145">useProtectedWipe</span><span class="sxs-lookup"><span data-stu-id="1bc70-145">useProtectedWipe</span></span>|<span data-ttu-id="1bc70-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="1bc70-146">Boolean</span></span>|<span data-ttu-id="1bc70-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1bc70-147">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1bc70-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bc70-148">Response</span></span>
<span data-ttu-id="1bc70-149">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1bc70-149">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1bc70-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bc70-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bc70-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bc70-151">Request</span></span>
<span data-ttu-id="1bc70-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bc70-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 170

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value",
  "persistEsimDataPlan": true,
  "useProtectedWipe": true
}
```

### <a name="response"></a><span data-ttu-id="1bc70-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bc70-153">Response</span></span>
<span data-ttu-id="1bc70-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bc70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




