---
title: Ação updateWindowsDeviceAccount
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72e11dc56bde0ab621c1aa985e8cf1fa390decef
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967969"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="08ac8-103">Ação updateWindowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="08ac8-103">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="08ac8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08ac8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08ac8-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="08ac8-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08ac8-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="08ac8-106">Prerequisites</span></span>
<span data-ttu-id="08ac8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08ac8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08ac8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08ac8-109">Permission type</span></span>|<span data-ttu-id="08ac8-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="08ac8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08ac8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08ac8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="08ac8-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="08ac8-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="08ac8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08ac8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08ac8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08ac8-114">Not supported.</span></span>|
|<span data-ttu-id="08ac8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08ac8-115">Application</span></span>|<span data-ttu-id="08ac8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08ac8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08ac8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08ac8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="08ac8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08ac8-118">Request headers</span></span>
|<span data-ttu-id="08ac8-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08ac8-119">Header</span></span>|<span data-ttu-id="08ac8-120">Valor</span><span class="sxs-lookup"><span data-stu-id="08ac8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08ac8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="08ac8-121">Authorization</span></span>|<span data-ttu-id="08ac8-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08ac8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08ac8-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="08ac8-123">Accept</span></span>|<span data-ttu-id="08ac8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="08ac8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08ac8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08ac8-125">Request body</span></span>
<span data-ttu-id="08ac8-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="08ac8-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="08ac8-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="08ac8-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="08ac8-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08ac8-128">Property</span></span>|<span data-ttu-id="08ac8-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="08ac8-129">Type</span></span>|<span data-ttu-id="08ac8-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="08ac8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08ac8-131">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="08ac8-131">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="08ac8-132">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="08ac8-132">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="08ac8-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="08ac8-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="08ac8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="08ac8-134">Response</span></span>
<span data-ttu-id="08ac8-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="08ac8-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="08ac8-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08ac8-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="08ac8-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08ac8-137">Request</span></span>
<span data-ttu-id="08ac8-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08ac8-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08ac8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="08ac8-139">Response</span></span>
<span data-ttu-id="08ac8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08ac8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



