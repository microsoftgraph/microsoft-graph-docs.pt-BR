---
title: ação de setDeviceName
description: Definir o nome do dispositivo do dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a73ec88c96b80fd6d8a2cd6843cacf0ff81807bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411852"
---
# <a name="setdevicename-action"></a><span data-ttu-id="97e57-103">ação de setDeviceName</span><span class="sxs-lookup"><span data-stu-id="97e57-103">setDeviceName action</span></span>

> <span data-ttu-id="97e57-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="97e57-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="97e57-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="97e57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97e57-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="97e57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97e57-107">Definir o nome do dispositivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97e57-107">Set device name of the device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97e57-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97e57-108">Prerequisites</span></span>
<span data-ttu-id="97e57-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="97e57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="97e57-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97e57-111">Permission type</span></span>|<span data-ttu-id="97e57-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97e57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97e57-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97e57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97e57-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="97e57-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="97e57-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97e57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97e57-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97e57-116">Not supported.</span></span>|
|<span data-ttu-id="97e57-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97e57-117">Application</span></span>|<span data-ttu-id="97e57-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97e57-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97e57-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97e57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/managedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/setDeviceName
```

## <a name="request-headers"></a><span data-ttu-id="97e57-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97e57-120">Request headers</span></span>
|<span data-ttu-id="97e57-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97e57-121">Header</span></span>|<span data-ttu-id="97e57-122">Valor</span><span class="sxs-lookup"><span data-stu-id="97e57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97e57-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97e57-123">Authorization</span></span>|<span data-ttu-id="97e57-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97e57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97e57-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97e57-125">Accept</span></span>|<span data-ttu-id="97e57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97e57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97e57-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97e57-127">Request body</span></span>
<span data-ttu-id="97e57-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="97e57-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="97e57-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="97e57-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="97e57-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97e57-130">Property</span></span>|<span data-ttu-id="97e57-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="97e57-131">Type</span></span>|<span data-ttu-id="97e57-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="97e57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97e57-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="97e57-133">deviceName</span></span>|<span data-ttu-id="97e57-134">String</span><span class="sxs-lookup"><span data-stu-id="97e57-134">String</span></span>|<span data-ttu-id="97e57-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="97e57-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="97e57-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="97e57-136">Response</span></span>
<span data-ttu-id="97e57-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="97e57-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="97e57-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97e57-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="97e57-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97e57-139">Request</span></span>
<span data-ttu-id="97e57-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97e57-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/setDeviceName

Content-type: application/json
Content-length: 41

{
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="97e57-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="97e57-141">Response</span></span>
<span data-ttu-id="97e57-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97e57-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




