---
title: Ação updateWindowsDeviceAccount
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2990410bbdc343f85f422e1bf40dc1b6fe120864
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954089"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="3cc0d-103">Ação updateWindowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="3cc0d-103">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="3cc0d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3cc0d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3cc0d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3cc0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3cc0d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3cc0d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cc0d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3cc0d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3cc0d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3cc0d-108">Prerequisites</span></span>
<span data-ttu-id="3cc0d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cc0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cc0d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cc0d-111">Permission type</span></span>|<span data-ttu-id="3cc0d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3cc0d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cc0d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cc0d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3cc0d-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="3cc0d-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="3cc0d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cc0d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cc0d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cc0d-116">Not supported.</span></span>|
|<span data-ttu-id="3cc0d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cc0d-117">Application</span></span>|<span data-ttu-id="3cc0d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cc0d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cc0d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cc0d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="3cc0d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc0d-120">Request headers</span></span>
|<span data-ttu-id="3cc0d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3cc0d-121">Header</span></span>|<span data-ttu-id="3cc0d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3cc0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cc0d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cc0d-123">Authorization</span></span>|<span data-ttu-id="3cc0d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cc0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cc0d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3cc0d-125">Accept</span></span>|<span data-ttu-id="3cc0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3cc0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cc0d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc0d-127">Request body</span></span>
<span data-ttu-id="3cc0d-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3cc0d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3cc0d-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3cc0d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3cc0d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cc0d-130">Property</span></span>|<span data-ttu-id="3cc0d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cc0d-131">Type</span></span>|<span data-ttu-id="3cc0d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cc0d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cc0d-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="3cc0d-133">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="3cc0d-134">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="3cc0d-134">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="3cc0d-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3cc0d-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3cc0d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cc0d-136">Response</span></span>
<span data-ttu-id="3cc0d-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3cc0d-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3cc0d-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cc0d-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="3cc0d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc0d-139">Request</span></span>
<span data-ttu-id="3cc0d-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cc0d-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a><span data-ttu-id="3cc0d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cc0d-141">Response</span></span>
<span data-ttu-id="3cc0d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3cc0d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





