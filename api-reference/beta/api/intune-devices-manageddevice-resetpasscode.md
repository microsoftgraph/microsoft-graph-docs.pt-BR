---
title: Ação resetPasscode
description: Redefinir senha
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7638b2fcdee88128adfc31a0d1ce5cd41f26cf6c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49234894"
---
# <a name="resetpasscode-action"></a><span data-ttu-id="5b970-103">Ação resetPasscode</span><span class="sxs-lookup"><span data-stu-id="5b970-103">resetPasscode action</span></span>

<span data-ttu-id="5b970-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b970-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b970-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b970-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b970-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b970-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b970-107">Redefinir senha</span><span class="sxs-lookup"><span data-stu-id="5b970-107">Reset passcode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b970-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b970-108">Prerequisites</span></span>
<span data-ttu-id="5b970-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b970-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b970-111">Permission type</span></span>|<span data-ttu-id="5b970-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b970-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b970-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b970-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b970-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="5b970-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="5b970-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b970-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b970-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b970-116">Not supported.</span></span>|
|<span data-ttu-id="5b970-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b970-117">Application</span></span>|<span data-ttu-id="5b970-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="5b970-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b970-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b970-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/resetPasscode
POST /deviceManagement/comanagedDevices/{managedDeviceId}/resetPasscode
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/resetPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/resetPasscode
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/resetPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/resetPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/resetPasscode
```

## <a name="request-headers"></a><span data-ttu-id="5b970-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b970-120">Request headers</span></span>
|<span data-ttu-id="5b970-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b970-121">Header</span></span>|<span data-ttu-id="5b970-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5b970-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b970-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b970-123">Authorization</span></span>|<span data-ttu-id="5b970-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b970-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b970-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b970-125">Accept</span></span>|<span data-ttu-id="5b970-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b970-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b970-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b970-127">Request body</span></span>
<span data-ttu-id="5b970-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b970-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b970-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b970-129">Response</span></span>
<span data-ttu-id="5b970-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5b970-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5b970-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b970-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b970-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b970-132">Request</span></span>
<span data-ttu-id="5b970-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b970-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/resetPasscode
```

### <a name="response"></a><span data-ttu-id="5b970-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b970-134">Response</span></span>
<span data-ttu-id="5b970-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b970-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




