---
title: Ação enableLostMode
description: Habilitar modo perdido
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ebe6ceb4c8ad845b6452c035694a2b7a55dfe29f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529919"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="cd119-103">Ação enableLostMode</span><span class="sxs-lookup"><span data-stu-id="cd119-103">enableLostMode action</span></span>

> <span data-ttu-id="cd119-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cd119-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd119-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd119-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd119-106">Habilitar modo perdido</span><span class="sxs-lookup"><span data-stu-id="cd119-106">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd119-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cd119-107">Prerequisites</span></span>
<span data-ttu-id="cd119-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd119-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd119-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd119-110">Permission type</span></span>|<span data-ttu-id="cd119-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cd119-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd119-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd119-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd119-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="cd119-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="cd119-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd119-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd119-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd119-115">Not supported.</span></span>|
|<span data-ttu-id="cd119-116">Application</span><span class="sxs-lookup"><span data-stu-id="cd119-116">Application</span></span>|<span data-ttu-id="cd119-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="cd119-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd119-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd119-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="cd119-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd119-119">Request headers</span></span>
|<span data-ttu-id="cd119-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd119-120">Header</span></span>|<span data-ttu-id="cd119-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cd119-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd119-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd119-122">Authorization</span></span>|<span data-ttu-id="cd119-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd119-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd119-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cd119-124">Accept</span></span>|<span data-ttu-id="cd119-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd119-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd119-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd119-126">Request body</span></span>
<span data-ttu-id="cd119-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="cd119-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cd119-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="cd119-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cd119-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd119-129">Property</span></span>|<span data-ttu-id="cd119-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd119-130">Type</span></span>|<span data-ttu-id="cd119-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd119-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd119-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="cd119-132">message</span></span>|<span data-ttu-id="cd119-133">String</span><span class="sxs-lookup"><span data-stu-id="cd119-133">String</span></span>|<span data-ttu-id="cd119-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cd119-134">Not yet documented</span></span>|
|<span data-ttu-id="cd119-135">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="cd119-135">phoneNumber</span></span>|<span data-ttu-id="cd119-136">String</span><span class="sxs-lookup"><span data-stu-id="cd119-136">String</span></span>|<span data-ttu-id="cd119-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cd119-137">Not yet documented</span></span>|
|<span data-ttu-id="cd119-138">cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd119-138">footer</span></span>|<span data-ttu-id="cd119-139">String</span><span class="sxs-lookup"><span data-stu-id="cd119-139">String</span></span>|<span data-ttu-id="cd119-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cd119-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cd119-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd119-141">Response</span></span>
<span data-ttu-id="cd119-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cd119-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd119-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd119-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd119-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd119-144">Request</span></span>
<span data-ttu-id="cd119-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd119-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cd119-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd119-146">Response</span></span>
<span data-ttu-id="cd119-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd119-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






