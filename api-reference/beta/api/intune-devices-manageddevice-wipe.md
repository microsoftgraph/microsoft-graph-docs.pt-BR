---
title: Ação wipe
description: Apagar um dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91bdbd45355c986e7ef59bf5e8be6621db462001
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520036"
---
# <a name="wipe-action"></a><span data-ttu-id="1ef72-103">ação wipe</span><span class="sxs-lookup"><span data-stu-id="1ef72-103">wipe action</span></span>

> <span data-ttu-id="1ef72-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ef72-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ef72-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ef72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ef72-106">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="1ef72-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ef72-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ef72-107">Prerequisites</span></span>
<span data-ttu-id="1ef72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ef72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ef72-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ef72-110">Permission type</span></span>|<span data-ttu-id="1ef72-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ef72-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ef72-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ef72-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ef72-113">DeviceManagementManagedDevices. PriviligedOperation. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1ef72-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1ef72-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ef72-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ef72-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ef72-115">Not supported.</span></span>|
|<span data-ttu-id="1ef72-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ef72-116">Application</span></span>|<span data-ttu-id="1ef72-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ef72-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ef72-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ef72-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1ef72-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ef72-119">Request headers</span></span>
|<span data-ttu-id="1ef72-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ef72-120">Header</span></span>|<span data-ttu-id="1ef72-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1ef72-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ef72-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ef72-122">Authorization</span></span>|<span data-ttu-id="1ef72-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ef72-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ef72-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ef72-124">Accept</span></span>|<span data-ttu-id="1ef72-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ef72-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ef72-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ef72-126">Request body</span></span>
<span data-ttu-id="1ef72-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1ef72-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1ef72-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1ef72-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1ef72-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ef72-129">Property</span></span>|<span data-ttu-id="1ef72-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ef72-130">Type</span></span>|<span data-ttu-id="1ef72-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ef72-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ef72-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="1ef72-132">keepEnrollmentData</span></span>|<span data-ttu-id="1ef72-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="1ef72-133">Boolean</span></span>|<span data-ttu-id="1ef72-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1ef72-134">Not yet documented</span></span>|
|<span data-ttu-id="1ef72-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="1ef72-135">keepUserData</span></span>|<span data-ttu-id="1ef72-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="1ef72-136">Boolean</span></span>|<span data-ttu-id="1ef72-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1ef72-137">Not yet documented</span></span>|
|<span data-ttu-id="1ef72-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="1ef72-138">macOsUnlockCode</span></span>|<span data-ttu-id="1ef72-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ef72-139">String</span></span>|<span data-ttu-id="1ef72-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1ef72-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1ef72-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ef72-141">Response</span></span>
<span data-ttu-id="1ef72-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1ef72-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1ef72-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ef72-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ef72-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ef72-144">Request</span></span>
<span data-ttu-id="1ef72-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ef72-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1ef72-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ef72-146">Response</span></span>
<span data-ttu-id="1ef72-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ef72-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





