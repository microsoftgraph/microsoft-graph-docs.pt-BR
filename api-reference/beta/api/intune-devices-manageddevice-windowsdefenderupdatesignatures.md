---
title: Ação windowsDefenderUpdateSignatures
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ded617da6d1248ca77ff606231d6a585d5188156
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693203"
---
# <a name="windowsdefenderupdatesignatures-action"></a><span data-ttu-id="e5cbc-103">Ação windowsDefenderUpdateSignatures</span><span class="sxs-lookup"><span data-stu-id="e5cbc-103">windowsDefenderUpdateSignatures action</span></span>

<span data-ttu-id="e5cbc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5cbc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5cbc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5cbc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5cbc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5cbc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5cbc-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e5cbc-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5cbc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e5cbc-108">Prerequisites</span></span>
<span data-ttu-id="e5cbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5cbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5cbc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5cbc-111">Permission type</span></span>|<span data-ttu-id="e5cbc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e5cbc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5cbc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5cbc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5cbc-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e5cbc-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e5cbc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5cbc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5cbc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5cbc-116">Not supported.</span></span>|
|<span data-ttu-id="e5cbc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5cbc-117">Application</span></span>|<span data-ttu-id="e5cbc-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e5cbc-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5cbc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5cbc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/comanagedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/windowsDefenderUpdateSignatures
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsDefenderUpdateSignatures
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/windowsDefenderUpdateSignatures
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

## <a name="request-headers"></a><span data-ttu-id="e5cbc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5cbc-120">Request headers</span></span>
|<span data-ttu-id="e5cbc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5cbc-121">Header</span></span>|<span data-ttu-id="e5cbc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e5cbc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5cbc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5cbc-123">Authorization</span></span>|<span data-ttu-id="e5cbc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5cbc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5cbc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e5cbc-125">Accept</span></span>|<span data-ttu-id="e5cbc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5cbc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5cbc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5cbc-127">Request body</span></span>
<span data-ttu-id="e5cbc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5cbc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5cbc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5cbc-129">Response</span></span>
<span data-ttu-id="e5cbc-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e5cbc-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e5cbc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5cbc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5cbc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5cbc-132">Request</span></span>
<span data-ttu-id="e5cbc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5cbc-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

### <a name="response"></a><span data-ttu-id="e5cbc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5cbc-134">Response</span></span>
<span data-ttu-id="e5cbc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5cbc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





