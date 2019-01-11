---
title: Ação disableLostMode
description: Desabilitar o modo perdido
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 882a7da9e11a76984d233d374c5b0493660f7626
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874358"
---
# <a name="disablelostmode-action"></a><span data-ttu-id="d3748-103">Ação disableLostMode</span><span class="sxs-lookup"><span data-stu-id="d3748-103">disableLostMode action</span></span>

> <span data-ttu-id="d3748-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d3748-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3748-105">Desabilitar o modo perdido</span><span class="sxs-lookup"><span data-stu-id="d3748-105">Disable lost mode</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3748-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3748-106">Prerequisites</span></span>
<span data-ttu-id="d3748-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3748-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3748-109">Permission type</span></span>|<span data-ttu-id="d3748-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3748-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3748-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3748-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3748-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="d3748-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="d3748-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3748-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3748-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3748-114">Not supported.</span></span>|
|<span data-ttu-id="d3748-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3748-115">Application</span></span>|<span data-ttu-id="d3748-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3748-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3748-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3748-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/disableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="d3748-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3748-118">Request headers</span></span>
|<span data-ttu-id="d3748-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3748-119">Header</span></span>|<span data-ttu-id="d3748-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d3748-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3748-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3748-121">Authorization</span></span>|<span data-ttu-id="d3748-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3748-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3748-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3748-123">Accept</span></span>|<span data-ttu-id="d3748-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d3748-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3748-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3748-125">Request body</span></span>
<span data-ttu-id="d3748-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3748-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3748-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3748-127">Response</span></span>
<span data-ttu-id="d3748-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d3748-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d3748-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3748-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3748-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3748-130">Request</span></span>
<span data-ttu-id="d3748-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3748-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/disableLostMode
```

### <a name="response"></a><span data-ttu-id="d3748-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3748-132">Response</span></span>
<span data-ttu-id="d3748-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3748-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



