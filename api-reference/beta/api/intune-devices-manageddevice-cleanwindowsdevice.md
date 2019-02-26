---
title: Ação cleanWindowsDevice
description: Limpar dispositivo Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ead20ba5d585739f9900d7dc96ad1fa7fce2bc6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147597"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="16712-103">Ação cleanWindowsDevice</span><span class="sxs-lookup"><span data-stu-id="16712-103">cleanWindowsDevice action</span></span>

> <span data-ttu-id="16712-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="16712-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16712-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16712-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16712-106">Limpar dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="16712-106">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16712-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16712-107">Prerequisites</span></span>
<span data-ttu-id="16712-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="16712-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="16712-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16712-110">Permission type</span></span>|<span data-ttu-id="16712-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16712-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16712-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16712-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16712-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="16712-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="16712-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16712-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16712-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16712-115">Not supported.</span></span>|
|<span data-ttu-id="16712-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16712-116">Application</span></span>|<span data-ttu-id="16712-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16712-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16712-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16712-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="16712-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16712-119">Request headers</span></span>
|<span data-ttu-id="16712-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16712-120">Header</span></span>|<span data-ttu-id="16712-121">Valor</span><span class="sxs-lookup"><span data-stu-id="16712-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16712-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="16712-122">Authorization</span></span>|<span data-ttu-id="16712-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16712-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16712-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16712-124">Accept</span></span>|<span data-ttu-id="16712-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16712-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16712-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16712-126">Request body</span></span>
<span data-ttu-id="16712-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="16712-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="16712-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="16712-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="16712-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16712-129">Property</span></span>|<span data-ttu-id="16712-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="16712-130">Type</span></span>|<span data-ttu-id="16712-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="16712-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16712-132">keepUserData</span><span class="sxs-lookup"><span data-stu-id="16712-132">keepUserData</span></span>|<span data-ttu-id="16712-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="16712-133">Boolean</span></span>|<span data-ttu-id="16712-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="16712-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="16712-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="16712-135">Response</span></span>
<span data-ttu-id="16712-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="16712-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="16712-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16712-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="16712-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16712-138">Request</span></span>
<span data-ttu-id="16712-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16712-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="16712-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="16712-140">Response</span></span>
<span data-ttu-id="16712-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16712-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




