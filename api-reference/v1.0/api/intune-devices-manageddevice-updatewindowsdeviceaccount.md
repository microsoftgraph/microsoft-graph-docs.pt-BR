---
title: Ação updateWindowsDeviceAccount
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5ede62413a25aa3dc5af3ad08b8912a126598ff5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965597"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="ff130-103">Ação updateWindowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="ff130-103">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="ff130-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ff130-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff130-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ff130-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff130-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff130-106">Prerequisites</span></span>
<span data-ttu-id="ff130-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff130-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff130-109">Permission type</span></span>|<span data-ttu-id="ff130-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff130-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff130-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff130-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff130-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ff130-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ff130-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff130-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff130-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff130-114">Not supported.</span></span>|
|<span data-ttu-id="ff130-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff130-115">Application</span></span>|<span data-ttu-id="ff130-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff130-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff130-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff130-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="ff130-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff130-118">Request headers</span></span>
|<span data-ttu-id="ff130-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff130-119">Header</span></span>|<span data-ttu-id="ff130-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ff130-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff130-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff130-121">Authorization</span></span>|<span data-ttu-id="ff130-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff130-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff130-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff130-123">Accept</span></span>|<span data-ttu-id="ff130-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ff130-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff130-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff130-125">Request body</span></span>
<span data-ttu-id="ff130-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ff130-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ff130-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ff130-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ff130-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff130-128">Property</span></span>|<span data-ttu-id="ff130-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff130-129">Type</span></span>|<span data-ttu-id="ff130-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff130-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff130-131">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="ff130-131">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="ff130-132">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="ff130-132">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="ff130-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ff130-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ff130-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff130-134">Response</span></span>
<span data-ttu-id="ff130-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ff130-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff130-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff130-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff130-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff130-137">Request</span></span>
<span data-ttu-id="ff130-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff130-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

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

### <a name="response"></a><span data-ttu-id="ff130-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff130-139">Response</span></span>
<span data-ttu-id="ff130-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff130-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



