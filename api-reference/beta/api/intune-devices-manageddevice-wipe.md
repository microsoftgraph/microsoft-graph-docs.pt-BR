---
title: Ação wipe
description: Apagar um dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91bdbd45355c986e7ef59bf5e8be6621db462001
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790652"
---
# <a name="wipe-action"></a><span data-ttu-id="d6cb8-103">ação wipe</span><span class="sxs-lookup"><span data-stu-id="d6cb8-103">wipe action</span></span>

> <span data-ttu-id="d6cb8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6cb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6cb8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6cb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6cb8-106">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="d6cb8-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6cb8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6cb8-107">Prerequisites</span></span>
<span data-ttu-id="d6cb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6cb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6cb8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6cb8-110">Permission type</span></span>|<span data-ttu-id="d6cb8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6cb8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6cb8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6cb8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6cb8-113">DeviceManagementManagedDevices. PriviligedOperation. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d6cb8-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d6cb8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6cb8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6cb8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6cb8-115">Not supported.</span></span>|
|<span data-ttu-id="d6cb8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6cb8-116">Application</span></span>|<span data-ttu-id="d6cb8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6cb8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6cb8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6cb8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="d6cb8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6cb8-119">Request headers</span></span>
|<span data-ttu-id="d6cb8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6cb8-120">Header</span></span>|<span data-ttu-id="d6cb8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d6cb8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6cb8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6cb8-122">Authorization</span></span>|<span data-ttu-id="d6cb8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6cb8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6cb8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6cb8-124">Accept</span></span>|<span data-ttu-id="d6cb8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6cb8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6cb8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6cb8-126">Request body</span></span>
<span data-ttu-id="d6cb8-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d6cb8-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d6cb8-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d6cb8-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d6cb8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6cb8-129">Property</span></span>|<span data-ttu-id="d6cb8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6cb8-130">Type</span></span>|<span data-ttu-id="d6cb8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6cb8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6cb8-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="d6cb8-132">keepEnrollmentData</span></span>|<span data-ttu-id="d6cb8-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6cb8-133">Boolean</span></span>|<span data-ttu-id="d6cb8-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6cb8-134">Not yet documented</span></span>|
|<span data-ttu-id="d6cb8-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="d6cb8-135">keepUserData</span></span>|<span data-ttu-id="d6cb8-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6cb8-136">Boolean</span></span>|<span data-ttu-id="d6cb8-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6cb8-137">Not yet documented</span></span>|
|<span data-ttu-id="d6cb8-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="d6cb8-138">macOsUnlockCode</span></span>|<span data-ttu-id="d6cb8-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6cb8-139">String</span></span>|<span data-ttu-id="d6cb8-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6cb8-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d6cb8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6cb8-141">Response</span></span>
<span data-ttu-id="d6cb8-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d6cb8-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d6cb8-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6cb8-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6cb8-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6cb8-144">Request</span></span>
<span data-ttu-id="d6cb8-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6cb8-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="d6cb8-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6cb8-146">Response</span></span>
<span data-ttu-id="d6cb8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6cb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





