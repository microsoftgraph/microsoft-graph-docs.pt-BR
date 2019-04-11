---
title: Ação enableLostMode
description: Habilitar modo perdido
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 735ee2659c603b03718a0e0031973dd5addb21eb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791625"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="c2f4d-103">Ação enableLostMode</span><span class="sxs-lookup"><span data-stu-id="c2f4d-103">enableLostMode action</span></span>

> <span data-ttu-id="c2f4d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c2f4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2f4d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2f4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2f4d-106">Habilitar modo perdido</span><span class="sxs-lookup"><span data-stu-id="c2f4d-106">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2f4d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c2f4d-107">Prerequisites</span></span>
<span data-ttu-id="c2f4d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2f4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2f4d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2f4d-110">Permission type</span></span>|<span data-ttu-id="c2f4d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c2f4d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2f4d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2f4d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c2f4d-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c2f4d-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="c2f4d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2f4d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2f4d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2f4d-115">Not supported.</span></span>|
|<span data-ttu-id="c2f4d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2f4d-116">Application</span></span>|<span data-ttu-id="c2f4d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2f4d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2f4d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2f4d-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c2f4d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2f4d-119">Request headers</span></span>
|<span data-ttu-id="c2f4d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2f4d-120">Header</span></span>|<span data-ttu-id="c2f4d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c2f4d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2f4d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2f4d-122">Authorization</span></span>|<span data-ttu-id="c2f4d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2f4d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2f4d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c2f4d-124">Accept</span></span>|<span data-ttu-id="c2f4d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c2f4d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2f4d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2f4d-126">Request body</span></span>
<span data-ttu-id="c2f4d-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c2f4d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c2f4d-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c2f4d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c2f4d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2f4d-129">Property</span></span>|<span data-ttu-id="c2f4d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2f4d-130">Type</span></span>|<span data-ttu-id="c2f4d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2f4d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2f4d-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="c2f4d-132">message</span></span>|<span data-ttu-id="c2f4d-133">String</span><span class="sxs-lookup"><span data-stu-id="c2f4d-133">String</span></span>|<span data-ttu-id="c2f4d-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c2f4d-134">Not yet documented</span></span>|
|<span data-ttu-id="c2f4d-135">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="c2f4d-135">phoneNumber</span></span>|<span data-ttu-id="c2f4d-136">String</span><span class="sxs-lookup"><span data-stu-id="c2f4d-136">String</span></span>|<span data-ttu-id="c2f4d-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c2f4d-137">Not yet documented</span></span>|
|<span data-ttu-id="c2f4d-138">cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2f4d-138">footer</span></span>|<span data-ttu-id="c2f4d-139">String</span><span class="sxs-lookup"><span data-stu-id="c2f4d-139">String</span></span>|<span data-ttu-id="c2f4d-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c2f4d-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c2f4d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2f4d-141">Response</span></span>
<span data-ttu-id="c2f4d-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c2f4d-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c2f4d-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2f4d-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2f4d-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2f4d-144">Request</span></span>
<span data-ttu-id="c2f4d-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2f4d-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c2f4d-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2f4d-146">Response</span></span>
<span data-ttu-id="c2f4d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2f4d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





