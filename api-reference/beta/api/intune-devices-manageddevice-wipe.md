---
title: Ação wipe
description: Apagar um dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2979333890626d197e596d6e768ac26205888276
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139358"
---
# <a name="wipe-action"></a><span data-ttu-id="ad19e-103">ação wipe</span><span class="sxs-lookup"><span data-stu-id="ad19e-103">wipe action</span></span>

> <span data-ttu-id="ad19e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ad19e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad19e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ad19e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad19e-106">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="ad19e-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad19e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ad19e-107">Prerequisites</span></span>
<span data-ttu-id="ad19e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ad19e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ad19e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad19e-110">Permission type</span></span>|<span data-ttu-id="ad19e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ad19e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad19e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad19e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad19e-113">DeviceManagementManagedDevices. PriviligedOperation. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ad19e-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ad19e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad19e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad19e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad19e-115">Not supported.</span></span>|
|<span data-ttu-id="ad19e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad19e-116">Application</span></span>|<span data-ttu-id="ad19e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad19e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad19e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad19e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="ad19e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad19e-119">Request headers</span></span>
|<span data-ttu-id="ad19e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad19e-120">Header</span></span>|<span data-ttu-id="ad19e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ad19e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad19e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad19e-122">Authorization</span></span>|<span data-ttu-id="ad19e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad19e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad19e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ad19e-124">Accept</span></span>|<span data-ttu-id="ad19e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad19e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad19e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad19e-126">Request body</span></span>
<span data-ttu-id="ad19e-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ad19e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ad19e-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ad19e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ad19e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad19e-129">Property</span></span>|<span data-ttu-id="ad19e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad19e-130">Type</span></span>|<span data-ttu-id="ad19e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad19e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad19e-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="ad19e-132">keepEnrollmentData</span></span>|<span data-ttu-id="ad19e-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="ad19e-133">Boolean</span></span>|<span data-ttu-id="ad19e-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ad19e-134">Not yet documented</span></span>|
|<span data-ttu-id="ad19e-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="ad19e-135">keepUserData</span></span>|<span data-ttu-id="ad19e-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="ad19e-136">Boolean</span></span>|<span data-ttu-id="ad19e-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ad19e-137">Not yet documented</span></span>|
|<span data-ttu-id="ad19e-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="ad19e-138">macOsUnlockCode</span></span>|<span data-ttu-id="ad19e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad19e-139">String</span></span>|<span data-ttu-id="ad19e-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ad19e-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ad19e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad19e-141">Response</span></span>
<span data-ttu-id="ad19e-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ad19e-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ad19e-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad19e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad19e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad19e-144">Request</span></span>
<span data-ttu-id="ad19e-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad19e-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="ad19e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad19e-146">Response</span></span>
<span data-ttu-id="ad19e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad19e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




