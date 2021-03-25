---
title: Ação wipe
description: Apagar um dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 340e5fc55e85a58dab5b5d2805e94744c493d49d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158280"
---
# <a name="wipe-action"></a><span data-ttu-id="26bb7-103">ação wipe</span><span class="sxs-lookup"><span data-stu-id="26bb7-103">wipe action</span></span>

<span data-ttu-id="26bb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26bb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26bb7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26bb7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26bb7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26bb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26bb7-107">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="26bb7-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26bb7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26bb7-108">Prerequisites</span></span>
<span data-ttu-id="26bb7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26bb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26bb7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26bb7-111">Permission type</span></span>|<span data-ttu-id="26bb7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26bb7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26bb7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26bb7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26bb7-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="26bb7-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="26bb7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26bb7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26bb7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26bb7-116">Not supported.</span></span>|
|<span data-ttu-id="26bb7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26bb7-117">Application</span></span>|<span data-ttu-id="26bb7-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="26bb7-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26bb7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26bb7-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="26bb7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26bb7-120">Request headers</span></span>
|<span data-ttu-id="26bb7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26bb7-121">Header</span></span>|<span data-ttu-id="26bb7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="26bb7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26bb7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="26bb7-123">Authorization</span></span>|<span data-ttu-id="26bb7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26bb7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26bb7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26bb7-125">Accept</span></span>|<span data-ttu-id="26bb7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26bb7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26bb7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26bb7-127">Request body</span></span>
<span data-ttu-id="26bb7-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="26bb7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="26bb7-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="26bb7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="26bb7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26bb7-130">Property</span></span>|<span data-ttu-id="26bb7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="26bb7-131">Type</span></span>|<span data-ttu-id="26bb7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="26bb7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26bb7-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="26bb7-133">keepEnrollmentData</span></span>|<span data-ttu-id="26bb7-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="26bb7-134">Boolean</span></span>|<span data-ttu-id="26bb7-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="26bb7-135">Not yet documented</span></span>|
|<span data-ttu-id="26bb7-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="26bb7-136">keepUserData</span></span>|<span data-ttu-id="26bb7-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="26bb7-137">Boolean</span></span>|<span data-ttu-id="26bb7-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="26bb7-138">Not yet documented</span></span>|
|<span data-ttu-id="26bb7-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="26bb7-139">macOsUnlockCode</span></span>|<span data-ttu-id="26bb7-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26bb7-140">String</span></span>|<span data-ttu-id="26bb7-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="26bb7-141">Not yet documented</span></span>|
|<span data-ttu-id="26bb7-142">useProtectedWipe</span><span class="sxs-lookup"><span data-stu-id="26bb7-142">useProtectedWipe</span></span>|<span data-ttu-id="26bb7-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="26bb7-143">Boolean</span></span>|<span data-ttu-id="26bb7-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="26bb7-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="26bb7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="26bb7-145">Response</span></span>
<span data-ttu-id="26bb7-146">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="26bb7-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="26bb7-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26bb7-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="26bb7-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26bb7-148">Request</span></span>
<span data-ttu-id="26bb7-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26bb7-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26bb7-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="26bb7-150">Response</span></span>
<span data-ttu-id="26bb7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26bb7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




