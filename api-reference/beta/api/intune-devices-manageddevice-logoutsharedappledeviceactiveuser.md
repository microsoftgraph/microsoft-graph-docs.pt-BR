---
title: Ação logoutSharedAppleDeviceActiveUser
description: Sair do usuário ativo no dispositivo Apple compartilhado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2ab50bbc742c713bff617efd7074b62b8f03fd3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909628"
---
# <a name="logoutsharedappledeviceactiveuser-action"></a><span data-ttu-id="51c4c-103">Ação logoutSharedAppleDeviceActiveUser</span><span class="sxs-lookup"><span data-stu-id="51c4c-103">logoutSharedAppleDeviceActiveUser action</span></span>

> <span data-ttu-id="51c4c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51c4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51c4c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51c4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51c4c-106">Sair do usuário ativo no dispositivo Apple compartilhado</span><span class="sxs-lookup"><span data-stu-id="51c4c-106">Logout shared Apple device active user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51c4c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51c4c-107">Prerequisites</span></span>
<span data-ttu-id="51c4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51c4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51c4c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51c4c-110">Permission type</span></span>|<span data-ttu-id="51c4c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51c4c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51c4c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51c4c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51c4c-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="51c4c-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="51c4c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51c4c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51c4c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51c4c-115">Not supported.</span></span>|
|<span data-ttu-id="51c4c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51c4c-116">Application</span></span>|<span data-ttu-id="51c4c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51c4c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51c4c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51c4c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
```

## <a name="request-headers"></a><span data-ttu-id="51c4c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51c4c-119">Request headers</span></span>
|<span data-ttu-id="51c4c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51c4c-120">Header</span></span>|<span data-ttu-id="51c4c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="51c4c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51c4c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="51c4c-122">Authorization</span></span>|<span data-ttu-id="51c4c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51c4c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51c4c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51c4c-124">Accept</span></span>|<span data-ttu-id="51c4c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51c4c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51c4c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51c4c-126">Request body</span></span>
<span data-ttu-id="51c4c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51c4c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51c4c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="51c4c-128">Response</span></span>
<span data-ttu-id="51c4c-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="51c4c-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="51c4c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51c4c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="51c4c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51c4c-131">Request</span></span>
<span data-ttu-id="51c4c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51c4c-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
```

### <a name="response"></a><span data-ttu-id="51c4c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="51c4c-133">Response</span></span>
<span data-ttu-id="51c4c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51c4c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




