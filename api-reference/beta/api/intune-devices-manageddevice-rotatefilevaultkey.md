---
title: ação rotateFileVaultKey
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f885e1b61bd2b82ce98a76fc304f8a17d1dd4fae
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698649"
---
# <a name="rotatefilevaultkey-action"></a><span data-ttu-id="8a849-103">ação rotateFileVaultKey</span><span class="sxs-lookup"><span data-stu-id="8a849-103">rotateFileVaultKey action</span></span>

<span data-ttu-id="8a849-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a849-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a849-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8a849-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a849-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8a849-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a849-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8a849-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a849-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a849-108">Prerequisites</span></span>
<span data-ttu-id="8a849-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a849-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a849-111">Permission type</span></span>|<span data-ttu-id="8a849-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a849-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a849-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a849-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a849-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="8a849-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="8a849-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a849-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a849-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a849-116">Not supported.</span></span>|
|<span data-ttu-id="8a849-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a849-117">Application</span></span>|<span data-ttu-id="8a849-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="8a849-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a849-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a849-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/rotateFileVaultKey
POST /deviceManagement/comanagedDevices/{managedDeviceId}/rotateFileVaultKey
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/rotateFileVaultKey
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/rotateFileVaultKey
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/rotateFileVaultKey
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/rotateFileVaultKey
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/rotateFileVaultKey
```

## <a name="request-headers"></a><span data-ttu-id="8a849-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a849-120">Request headers</span></span>
|<span data-ttu-id="8a849-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a849-121">Header</span></span>|<span data-ttu-id="8a849-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8a849-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a849-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a849-123">Authorization</span></span>|<span data-ttu-id="8a849-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a849-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a849-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a849-125">Accept</span></span>|<span data-ttu-id="8a849-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a849-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a849-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a849-127">Request body</span></span>
<span data-ttu-id="8a849-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a849-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a849-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a849-129">Response</span></span>
<span data-ttu-id="8a849-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8a849-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8a849-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a849-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a849-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a849-132">Request</span></span>
<span data-ttu-id="8a849-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a849-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/rotateFileVaultKey
```

### <a name="response"></a><span data-ttu-id="8a849-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a849-134">Response</span></span>
<span data-ttu-id="8a849-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a849-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





