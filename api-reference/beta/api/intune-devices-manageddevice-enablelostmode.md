---
title: Ação enableLostMode
description: Habilitar modo perdido
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86a23d9a55247308e169c296352f8e704671cf85
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985837"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="e7561-103">Ação enableLostMode</span><span class="sxs-lookup"><span data-stu-id="e7561-103">enableLostMode action</span></span>

> <span data-ttu-id="e7561-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7561-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7561-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7561-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7561-106">Habilitar modo perdido</span><span class="sxs-lookup"><span data-stu-id="e7561-106">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7561-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7561-107">Prerequisites</span></span>
<span data-ttu-id="e7561-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7561-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7561-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7561-110">Permission type</span></span>|<span data-ttu-id="e7561-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7561-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7561-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7561-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7561-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e7561-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e7561-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7561-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7561-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7561-115">Not supported.</span></span>|
|<span data-ttu-id="e7561-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7561-116">Application</span></span>|<span data-ttu-id="e7561-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7561-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7561-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7561-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e7561-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7561-119">Request headers</span></span>
|<span data-ttu-id="e7561-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7561-120">Header</span></span>|<span data-ttu-id="e7561-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e7561-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7561-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7561-122">Authorization</span></span>|<span data-ttu-id="e7561-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7561-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7561-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7561-124">Accept</span></span>|<span data-ttu-id="e7561-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7561-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7561-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7561-126">Request body</span></span>
<span data-ttu-id="e7561-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e7561-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e7561-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="e7561-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e7561-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7561-129">Property</span></span>|<span data-ttu-id="e7561-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7561-130">Type</span></span>|<span data-ttu-id="e7561-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7561-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7561-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="e7561-132">message</span></span>|<span data-ttu-id="e7561-133">String</span><span class="sxs-lookup"><span data-stu-id="e7561-133">String</span></span>|<span data-ttu-id="e7561-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7561-134">Not yet documented</span></span>|
|<span data-ttu-id="e7561-135">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="e7561-135">phoneNumber</span></span>|<span data-ttu-id="e7561-136">String</span><span class="sxs-lookup"><span data-stu-id="e7561-136">String</span></span>|<span data-ttu-id="e7561-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7561-137">Not yet documented</span></span>|
|<span data-ttu-id="e7561-138">cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7561-138">footer</span></span>|<span data-ttu-id="e7561-139">String</span><span class="sxs-lookup"><span data-stu-id="e7561-139">String</span></span>|<span data-ttu-id="e7561-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7561-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e7561-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7561-141">Response</span></span>
<span data-ttu-id="e7561-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e7561-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e7561-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7561-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7561-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7561-144">Request</span></span>
<span data-ttu-id="e7561-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7561-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e7561-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7561-146">Response</span></span>
<span data-ttu-id="e7561-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7561-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





