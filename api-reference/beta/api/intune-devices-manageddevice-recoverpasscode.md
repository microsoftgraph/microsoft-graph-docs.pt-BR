---
title: Ação recoverPasscode
description: Recuperar senha
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1950587e61f5bceba442a3514a020e382e2e4ee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310147"
---
# <a name="recoverpasscode-action"></a><span data-ttu-id="00982-103">Ação recoverPasscode</span><span class="sxs-lookup"><span data-stu-id="00982-103">recoverPasscode action</span></span>

> <span data-ttu-id="00982-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00982-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00982-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00982-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00982-106">Recuperar senha</span><span class="sxs-lookup"><span data-stu-id="00982-106">Recover passcode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00982-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00982-107">Prerequisites</span></span>
<span data-ttu-id="00982-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00982-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00982-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00982-110">Permission type</span></span>|<span data-ttu-id="00982-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="00982-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00982-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00982-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00982-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="00982-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="00982-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00982-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00982-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00982-115">Not supported.</span></span>|
|<span data-ttu-id="00982-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00982-116">Application</span></span>|<span data-ttu-id="00982-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="00982-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00982-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00982-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/recoverPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/recoverPasscode
```

## <a name="request-headers"></a><span data-ttu-id="00982-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00982-119">Request headers</span></span>
|<span data-ttu-id="00982-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00982-120">Header</span></span>|<span data-ttu-id="00982-121">Valor</span><span class="sxs-lookup"><span data-stu-id="00982-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00982-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="00982-122">Authorization</span></span>|<span data-ttu-id="00982-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00982-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00982-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="00982-124">Accept</span></span>|<span data-ttu-id="00982-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00982-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00982-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00982-126">Request body</span></span>
<span data-ttu-id="00982-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00982-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00982-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="00982-128">Response</span></span>
<span data-ttu-id="00982-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="00982-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="00982-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00982-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="00982-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00982-131">Request</span></span>
<span data-ttu-id="00982-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00982-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/recoverPasscode
```

### <a name="response"></a><span data-ttu-id="00982-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="00982-133">Response</span></span>
<span data-ttu-id="00982-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00982-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






