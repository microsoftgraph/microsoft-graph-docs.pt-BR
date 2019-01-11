---
title: ação de setDeviceName
description: Definir o nome do dispositivo do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 006ca412c59df6c4e0184827e52b3d790d7ea8bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894100"
---
# <a name="setdevicename-action"></a><span data-ttu-id="adbef-103">ação de setDeviceName</span><span class="sxs-lookup"><span data-stu-id="adbef-103">setDeviceName action</span></span>

> <span data-ttu-id="adbef-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="adbef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adbef-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="adbef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adbef-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="adbef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="adbef-107">Definir o nome do dispositivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="adbef-107">Set device name of the device.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="adbef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="adbef-108">Prerequisites</span></span>
<span data-ttu-id="adbef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adbef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adbef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adbef-111">Permission type</span></span>|<span data-ttu-id="adbef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="adbef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adbef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adbef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adbef-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="adbef-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="adbef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adbef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adbef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adbef-116">Not supported.</span></span>|
|<span data-ttu-id="adbef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adbef-117">Application</span></span>|<span data-ttu-id="adbef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adbef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adbef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adbef-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="adbef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="adbef-120">Request headers</span></span>
|<span data-ttu-id="adbef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="adbef-121">Header</span></span>|<span data-ttu-id="adbef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="adbef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adbef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="adbef-123">Authorization</span></span>|<span data-ttu-id="adbef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adbef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adbef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="adbef-125">Accept</span></span>|<span data-ttu-id="adbef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="adbef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adbef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adbef-127">Request body</span></span>
<span data-ttu-id="adbef-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="adbef-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="adbef-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="adbef-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="adbef-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="adbef-130">Property</span></span>|<span data-ttu-id="adbef-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="adbef-131">Type</span></span>|<span data-ttu-id="adbef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="adbef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adbef-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="adbef-133">deviceName</span></span>|<span data-ttu-id="adbef-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adbef-134">String</span></span>|<span data-ttu-id="adbef-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="adbef-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="adbef-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="adbef-136">Response</span></span>
<span data-ttu-id="adbef-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="adbef-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="adbef-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="adbef-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="adbef-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adbef-139">Request</span></span>
<span data-ttu-id="adbef-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="adbef-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/setDeviceName

Content-type: application/json
Content-length: 41

{
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="adbef-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="adbef-141">Response</span></span>
<span data-ttu-id="adbef-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="adbef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





