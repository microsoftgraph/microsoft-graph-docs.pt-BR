---
title: Ação shutDown
description: Desligar o dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58c68c21abec4dc670914e1bf5ee064aba953eb1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450480"
---
# <a name="shutdown-action"></a><span data-ttu-id="acf23-103">Ação shutDown</span><span class="sxs-lookup"><span data-stu-id="acf23-103">shutDown action</span></span>

<span data-ttu-id="acf23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acf23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="acf23-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="acf23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acf23-106">Desligar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="acf23-106">Shut down device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acf23-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="acf23-107">Prerequisites</span></span>
<span data-ttu-id="acf23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acf23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acf23-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="acf23-110">Permission type</span></span>|<span data-ttu-id="acf23-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="acf23-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acf23-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="acf23-112">Delegated (work or school account)</span></span>|<span data-ttu-id="acf23-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="acf23-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="acf23-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="acf23-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acf23-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acf23-115">Not supported.</span></span>|
|<span data-ttu-id="acf23-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="acf23-116">Application</span></span>|<span data-ttu-id="acf23-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acf23-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acf23-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acf23-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/shutDown
```

## <a name="request-headers"></a><span data-ttu-id="acf23-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="acf23-119">Request headers</span></span>
|<span data-ttu-id="acf23-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="acf23-120">Header</span></span>|<span data-ttu-id="acf23-121">Valor</span><span class="sxs-lookup"><span data-stu-id="acf23-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acf23-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="acf23-122">Authorization</span></span>|<span data-ttu-id="acf23-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acf23-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acf23-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="acf23-124">Accept</span></span>|<span data-ttu-id="acf23-125">application/json</span><span class="sxs-lookup"><span data-stu-id="acf23-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acf23-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="acf23-126">Request body</span></span>
<span data-ttu-id="acf23-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="acf23-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acf23-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="acf23-128">Response</span></span>
<span data-ttu-id="acf23-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="acf23-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="acf23-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="acf23-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="acf23-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acf23-131">Request</span></span>
<span data-ttu-id="acf23-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="acf23-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/shutDown
```

### <a name="response"></a><span data-ttu-id="acf23-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="acf23-133">Response</span></span>
<span data-ttu-id="acf23-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="acf23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






