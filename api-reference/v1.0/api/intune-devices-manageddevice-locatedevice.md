---
title: Ação locateDevice
description: Localizar um dispositivo
author: tfitzmac
ms.openlocfilehash: 08a5768cf7f08ac97929f40f5c04563d27c1fa93
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321221"
---
# <a name="locatedevice-action"></a><span data-ttu-id="64ffe-103">Ação locateDevice</span><span class="sxs-lookup"><span data-stu-id="64ffe-103">locateDevice action</span></span>

> <span data-ttu-id="64ffe-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="64ffe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64ffe-105">Localizar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="64ffe-105">Locate a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="64ffe-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64ffe-106">Prerequisites</span></span>
<span data-ttu-id="64ffe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64ffe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64ffe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64ffe-109">Permission type</span></span>|<span data-ttu-id="64ffe-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64ffe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64ffe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64ffe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="64ffe-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="64ffe-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="64ffe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64ffe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64ffe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64ffe-114">Not supported.</span></span>|
|<span data-ttu-id="64ffe-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64ffe-115">Application</span></span>|<span data-ttu-id="64ffe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64ffe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64ffe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64ffe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/locateDevice
```

## <a name="request-headers"></a><span data-ttu-id="64ffe-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64ffe-118">Request headers</span></span>
|<span data-ttu-id="64ffe-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64ffe-119">Header</span></span>|<span data-ttu-id="64ffe-120">Valor</span><span class="sxs-lookup"><span data-stu-id="64ffe-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64ffe-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="64ffe-121">Authorization</span></span>|<span data-ttu-id="64ffe-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64ffe-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64ffe-123">Accept</span><span class="sxs-lookup"><span data-stu-id="64ffe-123">Accept</span></span>|<span data-ttu-id="64ffe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="64ffe-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64ffe-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64ffe-125">Request body</span></span>
<span data-ttu-id="64ffe-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64ffe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64ffe-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="64ffe-127">Response</span></span>
<span data-ttu-id="64ffe-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="64ffe-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="64ffe-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64ffe-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="64ffe-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64ffe-130">Request</span></span>
<span data-ttu-id="64ffe-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64ffe-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/locateDevice
```

### <a name="response"></a><span data-ttu-id="64ffe-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="64ffe-132">Response</span></span>
<span data-ttu-id="64ffe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64ffe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



