---
title: Ação requestRemoteAssistance
description: Solicitar assistência remota
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ffac9091275408fa4d68310ac9be11167422bba
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974815"
---
# <a name="requestremoteassistance-action"></a><span data-ttu-id="5f02a-103">Ação requestRemoteAssistance</span><span class="sxs-lookup"><span data-stu-id="5f02a-103">requestRemoteAssistance action</span></span>

> <span data-ttu-id="5f02a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5f02a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f02a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f02a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f02a-106">Solicitar assistência remota</span><span class="sxs-lookup"><span data-stu-id="5f02a-106">Request remote assistance</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f02a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5f02a-107">Prerequisites</span></span>
<span data-ttu-id="5f02a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f02a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f02a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f02a-110">Permission type</span></span>|<span data-ttu-id="5f02a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5f02a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f02a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f02a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f02a-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f02a-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5f02a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f02a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f02a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f02a-115">Not supported.</span></span>|
|<span data-ttu-id="5f02a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f02a-116">Application</span></span>|<span data-ttu-id="5f02a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f02a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f02a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f02a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/requestRemoteAssistance
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

## <a name="request-headers"></a><span data-ttu-id="5f02a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f02a-119">Request headers</span></span>
|<span data-ttu-id="5f02a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f02a-120">Header</span></span>|<span data-ttu-id="5f02a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5f02a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f02a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f02a-122">Authorization</span></span>|<span data-ttu-id="5f02a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f02a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f02a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f02a-124">Accept</span></span>|<span data-ttu-id="5f02a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f02a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f02a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f02a-126">Request body</span></span>
<span data-ttu-id="5f02a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f02a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f02a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f02a-128">Response</span></span>
<span data-ttu-id="5f02a-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5f02a-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5f02a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f02a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f02a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f02a-131">Request</span></span>
<span data-ttu-id="5f02a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f02a-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

### <a name="response"></a><span data-ttu-id="5f02a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f02a-133">Response</span></span>
<span data-ttu-id="5f02a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f02a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




