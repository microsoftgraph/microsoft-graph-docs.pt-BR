---
title: Ação wipe
description: Apagar um dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f3a7f8c7bea6439b810bf7cc9df0be7dd06a81c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35981385"
---
# <a name="wipe-action"></a><span data-ttu-id="09b48-103">ação wipe</span><span class="sxs-lookup"><span data-stu-id="09b48-103">wipe action</span></span>

> <span data-ttu-id="09b48-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09b48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09b48-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09b48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09b48-106">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="09b48-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09b48-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="09b48-107">Prerequisites</span></span>
<span data-ttu-id="09b48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09b48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09b48-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09b48-110">Permission type</span></span>|<span data-ttu-id="09b48-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="09b48-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09b48-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09b48-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09b48-113">DeviceManagementManagedDevices. PriviligedOperation. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="09b48-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="09b48-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09b48-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09b48-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09b48-115">Not supported.</span></span>|
|<span data-ttu-id="09b48-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09b48-116">Application</span></span>|<span data-ttu-id="09b48-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09b48-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09b48-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09b48-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="09b48-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09b48-119">Request headers</span></span>
|<span data-ttu-id="09b48-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09b48-120">Header</span></span>|<span data-ttu-id="09b48-121">Valor</span><span class="sxs-lookup"><span data-stu-id="09b48-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09b48-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="09b48-122">Authorization</span></span>|<span data-ttu-id="09b48-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09b48-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09b48-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09b48-124">Accept</span></span>|<span data-ttu-id="09b48-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09b48-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09b48-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09b48-126">Request body</span></span>
<span data-ttu-id="09b48-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="09b48-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="09b48-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="09b48-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="09b48-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09b48-129">Property</span></span>|<span data-ttu-id="09b48-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="09b48-130">Type</span></span>|<span data-ttu-id="09b48-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="09b48-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09b48-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="09b48-132">keepEnrollmentData</span></span>|<span data-ttu-id="09b48-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="09b48-133">Boolean</span></span>|<span data-ttu-id="09b48-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="09b48-134">Not yet documented</span></span>|
|<span data-ttu-id="09b48-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="09b48-135">keepUserData</span></span>|<span data-ttu-id="09b48-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="09b48-136">Boolean</span></span>|<span data-ttu-id="09b48-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="09b48-137">Not yet documented</span></span>|
|<span data-ttu-id="09b48-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="09b48-138">macOsUnlockCode</span></span>|<span data-ttu-id="09b48-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09b48-139">String</span></span>|<span data-ttu-id="09b48-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="09b48-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="09b48-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="09b48-141">Response</span></span>
<span data-ttu-id="09b48-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="09b48-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="09b48-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09b48-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="09b48-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09b48-144">Request</span></span>
<span data-ttu-id="09b48-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09b48-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="09b48-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="09b48-146">Response</span></span>
<span data-ttu-id="09b48-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09b48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





