---
title: Ação enableLostMode
description: Habilitar o modo perdido
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3e0b147cb182c2054c0f6f70741eea14e7b3a5ef
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150063"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="e120f-103">Ação enableLostMode</span><span class="sxs-lookup"><span data-stu-id="e120f-103">enableLostMode action</span></span>

<span data-ttu-id="e120f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e120f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e120f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e120f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e120f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e120f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e120f-107">Habilitar o modo perdido</span><span class="sxs-lookup"><span data-stu-id="e120f-107">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e120f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e120f-108">Prerequisites</span></span>
<span data-ttu-id="e120f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e120f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e120f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e120f-111">Permission type</span></span>|<span data-ttu-id="e120f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e120f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e120f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e120f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e120f-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e120f-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e120f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e120f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e120f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e120f-116">Not supported.</span></span>|
|<span data-ttu-id="e120f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e120f-117">Application</span></span>|<span data-ttu-id="e120f-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e120f-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e120f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e120f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/comanagedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="e120f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e120f-120">Request headers</span></span>
|<span data-ttu-id="e120f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e120f-121">Header</span></span>|<span data-ttu-id="e120f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e120f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e120f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e120f-123">Authorization</span></span>|<span data-ttu-id="e120f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e120f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e120f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e120f-125">Accept</span></span>|<span data-ttu-id="e120f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e120f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e120f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e120f-127">Request body</span></span>
<span data-ttu-id="e120f-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e120f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e120f-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="e120f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e120f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e120f-130">Property</span></span>|<span data-ttu-id="e120f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e120f-131">Type</span></span>|<span data-ttu-id="e120f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e120f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e120f-133">mensagem</span><span class="sxs-lookup"><span data-stu-id="e120f-133">message</span></span>|<span data-ttu-id="e120f-134">String</span><span class="sxs-lookup"><span data-stu-id="e120f-134">String</span></span>|<span data-ttu-id="e120f-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e120f-135">Not yet documented</span></span>|
|<span data-ttu-id="e120f-136">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="e120f-136">phoneNumber</span></span>|<span data-ttu-id="e120f-137">String</span><span class="sxs-lookup"><span data-stu-id="e120f-137">String</span></span>|<span data-ttu-id="e120f-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e120f-138">Not yet documented</span></span>|
|<span data-ttu-id="e120f-139">rodapé</span><span class="sxs-lookup"><span data-stu-id="e120f-139">footer</span></span>|<span data-ttu-id="e120f-140">String</span><span class="sxs-lookup"><span data-stu-id="e120f-140">String</span></span>|<span data-ttu-id="e120f-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e120f-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e120f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e120f-142">Response</span></span>
<span data-ttu-id="e120f-143">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e120f-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e120f-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e120f-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="e120f-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e120f-145">Request</span></span>
<span data-ttu-id="e120f-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e120f-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e120f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e120f-147">Response</span></span>
<span data-ttu-id="e120f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e120f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




