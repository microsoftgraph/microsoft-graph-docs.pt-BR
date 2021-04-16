---
title: Ação activateDeviceEsim
description: Ative o eSIM no dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10b57e0a9c337f1c82cbc30547e57edd3c08f002
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868260"
---
# <a name="activatedeviceesim-action"></a><span data-ttu-id="13428-103">Ação activateDeviceEsim</span><span class="sxs-lookup"><span data-stu-id="13428-103">activateDeviceEsim action</span></span>

<span data-ttu-id="13428-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13428-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13428-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13428-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13428-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13428-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13428-107">Ative o eSIM no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13428-107">Activate eSIM on the device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13428-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13428-108">Prerequisites</span></span>
<span data-ttu-id="13428-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13428-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13428-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13428-111">Permission type</span></span>|<span data-ttu-id="13428-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13428-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13428-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13428-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13428-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="13428-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="13428-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13428-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13428-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13428-116">Not supported.</span></span>|
|<span data-ttu-id="13428-117">Application</span><span class="sxs-lookup"><span data-stu-id="13428-117">Application</span></span>|<span data-ttu-id="13428-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="13428-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13428-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13428-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/activateDeviceEsim
POST /deviceManagement/comanagedDevices/{managedDeviceId}/activateDeviceEsim
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/activateDeviceEsim
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/activateDeviceEsim
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/activateDeviceEsim
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/activateDeviceEsim
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/activateDeviceEsim
```

## <a name="request-headers"></a><span data-ttu-id="13428-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13428-120">Request headers</span></span>
|<span data-ttu-id="13428-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13428-121">Header</span></span>|<span data-ttu-id="13428-122">Valor</span><span class="sxs-lookup"><span data-stu-id="13428-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13428-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="13428-123">Authorization</span></span>|<span data-ttu-id="13428-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13428-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13428-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13428-125">Accept</span></span>|<span data-ttu-id="13428-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13428-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13428-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13428-127">Request body</span></span>
<span data-ttu-id="13428-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="13428-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="13428-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="13428-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="13428-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13428-130">Property</span></span>|<span data-ttu-id="13428-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="13428-131">Type</span></span>|<span data-ttu-id="13428-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="13428-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13428-133">carrierUrl</span><span class="sxs-lookup"><span data-stu-id="13428-133">carrierUrl</span></span>|<span data-ttu-id="13428-134">String</span><span class="sxs-lookup"><span data-stu-id="13428-134">String</span></span>|<span data-ttu-id="13428-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="13428-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="13428-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="13428-136">Response</span></span>
<span data-ttu-id="13428-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="13428-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="13428-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13428-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="13428-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13428-139">Request</span></span>
<span data-ttu-id="13428-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13428-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/activateDeviceEsim

Content-type: application/json
Content-length: 55

{
  "carrierUrl": "https://example.com/carrierUrl/"
}
```

### <a name="response"></a><span data-ttu-id="13428-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="13428-141">Response</span></span>
<span data-ttu-id="13428-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13428-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




