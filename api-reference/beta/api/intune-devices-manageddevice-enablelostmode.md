---
title: Ação enableLostMode
description: Habilitar modo perdido
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4ab803faeda3cdde39c7c00cdd905ab8d4f02855
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469052"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="5b383-103">Ação enableLostMode</span><span class="sxs-lookup"><span data-stu-id="5b383-103">enableLostMode action</span></span>

<span data-ttu-id="5b383-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5b383-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b383-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b383-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b383-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b383-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b383-107">Habilitar modo perdido</span><span class="sxs-lookup"><span data-stu-id="5b383-107">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b383-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b383-108">Prerequisites</span></span>
<span data-ttu-id="5b383-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b383-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b383-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b383-111">Permission type</span></span>|<span data-ttu-id="5b383-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b383-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b383-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b383-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b383-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="5b383-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="5b383-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b383-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b383-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b383-116">Not supported.</span></span>|
|<span data-ttu-id="5b383-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b383-117">Application</span></span>|<span data-ttu-id="5b383-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="5b383-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b383-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b383-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="5b383-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b383-120">Request headers</span></span>
|<span data-ttu-id="5b383-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b383-121">Header</span></span>|<span data-ttu-id="5b383-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5b383-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b383-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b383-123">Authorization</span></span>|<span data-ttu-id="5b383-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b383-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b383-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b383-125">Accept</span></span>|<span data-ttu-id="5b383-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b383-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b383-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b383-127">Request body</span></span>
<span data-ttu-id="5b383-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5b383-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5b383-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="5b383-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5b383-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b383-130">Property</span></span>|<span data-ttu-id="5b383-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b383-131">Type</span></span>|<span data-ttu-id="5b383-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b383-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b383-133">mensagem</span><span class="sxs-lookup"><span data-stu-id="5b383-133">message</span></span>|<span data-ttu-id="5b383-134">String</span><span class="sxs-lookup"><span data-stu-id="5b383-134">String</span></span>|<span data-ttu-id="5b383-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5b383-135">Not yet documented</span></span>|
|<span data-ttu-id="5b383-136">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="5b383-136">phoneNumber</span></span>|<span data-ttu-id="5b383-137">String</span><span class="sxs-lookup"><span data-stu-id="5b383-137">String</span></span>|<span data-ttu-id="5b383-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5b383-138">Not yet documented</span></span>|
|<span data-ttu-id="5b383-139">cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b383-139">footer</span></span>|<span data-ttu-id="5b383-140">String</span><span class="sxs-lookup"><span data-stu-id="5b383-140">String</span></span>|<span data-ttu-id="5b383-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5b383-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5b383-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b383-142">Response</span></span>
<span data-ttu-id="5b383-143">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5b383-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5b383-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b383-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b383-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b383-145">Request</span></span>
<span data-ttu-id="5b383-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b383-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b383-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b383-147">Response</span></span>
<span data-ttu-id="5b383-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b383-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





