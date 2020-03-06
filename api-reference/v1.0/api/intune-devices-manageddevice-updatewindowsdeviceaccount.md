---
title: Ação updateWindowsDeviceAccount
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b2b94682b3d2888283cd547ed2d9d45728506cd9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513466"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="b9511-103">Ação updateWindowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="b9511-103">updateWindowsDeviceAccount action</span></span>

<span data-ttu-id="b9511-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9511-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9511-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9511-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9511-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b9511-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9511-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9511-107">Prerequisites</span></span>
<span data-ttu-id="b9511-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9511-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9511-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9511-110">Permission type</span></span>|<span data-ttu-id="b9511-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9511-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9511-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9511-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9511-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b9511-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="b9511-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9511-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9511-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9511-115">Not supported.</span></span>|
|<span data-ttu-id="b9511-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9511-116">Application</span></span>|<span data-ttu-id="b9511-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9511-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9511-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9511-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="b9511-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9511-119">Request headers</span></span>
|<span data-ttu-id="b9511-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9511-120">Header</span></span>|<span data-ttu-id="b9511-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b9511-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9511-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9511-122">Authorization</span></span>|<span data-ttu-id="b9511-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9511-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9511-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9511-124">Accept</span></span>|<span data-ttu-id="b9511-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9511-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9511-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9511-126">Request body</span></span>
<span data-ttu-id="b9511-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b9511-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b9511-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b9511-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b9511-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9511-129">Property</span></span>|<span data-ttu-id="b9511-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9511-130">Type</span></span>|<span data-ttu-id="b9511-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9511-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9511-132">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="b9511-132">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="b9511-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="b9511-133">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="b9511-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b9511-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b9511-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9511-135">Response</span></span>
<span data-ttu-id="b9511-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b9511-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b9511-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9511-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9511-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9511-138">Request</span></span>
<span data-ttu-id="b9511-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9511-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b9511-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9511-140">Response</span></span>
<span data-ttu-id="b9511-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9511-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




