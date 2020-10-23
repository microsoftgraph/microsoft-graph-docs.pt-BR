---
title: Ação desativar
description: Desativa um dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8893558e7c70c59760bde19e962d3a8679d72c38
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727791"
---
# <a name="retire-action"></a><span data-ttu-id="4f541-103">Ação retire</span><span class="sxs-lookup"><span data-stu-id="4f541-103">retire action</span></span>

<span data-ttu-id="4f541-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f541-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f541-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f541-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f541-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f541-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f541-107">Desativa um dispositivo</span><span class="sxs-lookup"><span data-stu-id="4f541-107">Retire a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f541-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f541-108">Prerequisites</span></span>
<span data-ttu-id="4f541-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f541-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f541-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f541-111">Permission type</span></span>|<span data-ttu-id="4f541-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f541-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f541-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f541-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f541-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4f541-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="4f541-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f541-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f541-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f541-116">Not supported.</span></span>|
|<span data-ttu-id="4f541-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f541-117">Application</span></span>|<span data-ttu-id="4f541-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4f541-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f541-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f541-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/retire
POST /deviceManagement/comanagedDevices/{managedDeviceId}/retire
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/retire
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/retire
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/retire
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/retire
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/retire
```

## <a name="request-headers"></a><span data-ttu-id="4f541-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f541-120">Request headers</span></span>
|<span data-ttu-id="4f541-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f541-121">Header</span></span>|<span data-ttu-id="4f541-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4f541-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f541-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f541-123">Authorization</span></span>|<span data-ttu-id="4f541-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f541-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f541-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f541-125">Accept</span></span>|<span data-ttu-id="4f541-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f541-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f541-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f541-127">Request body</span></span>
<span data-ttu-id="4f541-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f541-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f541-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f541-129">Response</span></span>
<span data-ttu-id="4f541-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4f541-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4f541-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f541-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f541-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f541-132">Request</span></span>
<span data-ttu-id="4f541-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f541-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/retire
```

### <a name="response"></a><span data-ttu-id="4f541-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f541-134">Response</span></span>
<span data-ttu-id="4f541-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f541-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





