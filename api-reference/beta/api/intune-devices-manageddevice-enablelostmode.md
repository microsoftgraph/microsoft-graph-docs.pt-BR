---
title: Ação enableLostMode
description: Habilitar modo perdido
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e8103e113ab97f117d32b4fb50aaa828700f490
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909670"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="9b7e5-103">Ação enableLostMode</span><span class="sxs-lookup"><span data-stu-id="9b7e5-103">enableLostMode action</span></span>

> <span data-ttu-id="9b7e5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b7e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b7e5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b7e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b7e5-106">Habilitar modo perdido</span><span class="sxs-lookup"><span data-stu-id="9b7e5-106">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b7e5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b7e5-107">Prerequisites</span></span>
<span data-ttu-id="9b7e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b7e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b7e5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b7e5-110">Permission type</span></span>|<span data-ttu-id="9b7e5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b7e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b7e5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b7e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b7e5-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9b7e5-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="9b7e5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b7e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b7e5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b7e5-115">Not supported.</span></span>|
|<span data-ttu-id="9b7e5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b7e5-116">Application</span></span>|<span data-ttu-id="9b7e5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b7e5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b7e5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b7e5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="9b7e5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b7e5-119">Request headers</span></span>
|<span data-ttu-id="9b7e5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b7e5-120">Header</span></span>|<span data-ttu-id="9b7e5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9b7e5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b7e5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b7e5-122">Authorization</span></span>|<span data-ttu-id="9b7e5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b7e5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b7e5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b7e5-124">Accept</span></span>|<span data-ttu-id="9b7e5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b7e5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b7e5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b7e5-126">Request body</span></span>
<span data-ttu-id="9b7e5-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9b7e5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9b7e5-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="9b7e5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9b7e5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b7e5-129">Property</span></span>|<span data-ttu-id="9b7e5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b7e5-130">Type</span></span>|<span data-ttu-id="9b7e5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b7e5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b7e5-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="9b7e5-132">message</span></span>|<span data-ttu-id="9b7e5-133">String</span><span class="sxs-lookup"><span data-stu-id="9b7e5-133">String</span></span>|<span data-ttu-id="9b7e5-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b7e5-134">Not yet documented</span></span>|
|<span data-ttu-id="9b7e5-135">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="9b7e5-135">phoneNumber</span></span>|<span data-ttu-id="9b7e5-136">String</span><span class="sxs-lookup"><span data-stu-id="9b7e5-136">String</span></span>|<span data-ttu-id="9b7e5-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b7e5-137">Not yet documented</span></span>|
|<span data-ttu-id="9b7e5-138">cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b7e5-138">footer</span></span>|<span data-ttu-id="9b7e5-139">String</span><span class="sxs-lookup"><span data-stu-id="9b7e5-139">String</span></span>|<span data-ttu-id="9b7e5-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b7e5-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9b7e5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b7e5-141">Response</span></span>
<span data-ttu-id="9b7e5-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9b7e5-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9b7e5-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b7e5-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b7e5-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b7e5-144">Request</span></span>
<span data-ttu-id="9b7e5-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b7e5-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/enableLostMode

Content-type: application/json
Content-length: 103

{
  "message": "Message value",
  "phoneNumber": "Phone Number value",
  "footer": "Footer value"
}
```

### <a name="response"></a><span data-ttu-id="9b7e5-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b7e5-146">Response</span></span>
<span data-ttu-id="9b7e5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b7e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




