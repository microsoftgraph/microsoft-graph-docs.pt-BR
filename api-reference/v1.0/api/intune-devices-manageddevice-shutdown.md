---
title: Ação shutDown
description: Desligar o dispositivo
author: tfitzmac
ms.openlocfilehash: 3633b752216e84fb303b3ab4d1fb4535a3db2d61
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314011"
---
# <a name="shutdown-action"></a><span data-ttu-id="4576d-103">Ação shutDown</span><span class="sxs-lookup"><span data-stu-id="4576d-103">shutDown action</span></span>

> <span data-ttu-id="4576d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4576d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4576d-105">Desligar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="4576d-105">Shut down device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4576d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4576d-106">Prerequisites</span></span>
<span data-ttu-id="4576d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4576d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4576d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4576d-109">Permission type</span></span>|<span data-ttu-id="4576d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4576d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4576d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4576d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4576d-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4576d-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="4576d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4576d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4576d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4576d-114">Not supported.</span></span>|
|<span data-ttu-id="4576d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4576d-115">Application</span></span>|<span data-ttu-id="4576d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4576d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4576d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4576d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/shutDown
```

## <a name="request-headers"></a><span data-ttu-id="4576d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4576d-118">Request headers</span></span>
|<span data-ttu-id="4576d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4576d-119">Header</span></span>|<span data-ttu-id="4576d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4576d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4576d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4576d-121">Authorization</span></span>|<span data-ttu-id="4576d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4576d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4576d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4576d-123">Accept</span></span>|<span data-ttu-id="4576d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4576d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4576d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4576d-125">Request body</span></span>
<span data-ttu-id="4576d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4576d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4576d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4576d-127">Response</span></span>
<span data-ttu-id="4576d-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4576d-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4576d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4576d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4576d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4576d-130">Request</span></span>
<span data-ttu-id="4576d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4576d-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/shutDown
```

### <a name="response"></a><span data-ttu-id="4576d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4576d-132">Response</span></span>
<span data-ttu-id="4576d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4576d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



