---
title: Ação remoteLock
description: Bloqueio remoto
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1cc86617a50634fd4e0a34e02f8846a857e4e13b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450556"
---
# <a name="remotelock-action"></a><span data-ttu-id="efbeb-103">Ação remoteLock</span><span class="sxs-lookup"><span data-stu-id="efbeb-103">remoteLock action</span></span>

<span data-ttu-id="efbeb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efbeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efbeb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="efbeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efbeb-106">Bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="efbeb-106">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efbeb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efbeb-107">Prerequisites</span></span>
<span data-ttu-id="efbeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efbeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efbeb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efbeb-110">Permission type</span></span>|<span data-ttu-id="efbeb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="efbeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efbeb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efbeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="efbeb-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="efbeb-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="efbeb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efbeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efbeb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efbeb-115">Not supported.</span></span>|
|<span data-ttu-id="efbeb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efbeb-116">Application</span></span>|<span data-ttu-id="efbeb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efbeb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efbeb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efbeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/remoteLock
```

## <a name="request-headers"></a><span data-ttu-id="efbeb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efbeb-119">Request headers</span></span>
|<span data-ttu-id="efbeb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efbeb-120">Header</span></span>|<span data-ttu-id="efbeb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="efbeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efbeb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="efbeb-122">Authorization</span></span>|<span data-ttu-id="efbeb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efbeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efbeb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="efbeb-124">Accept</span></span>|<span data-ttu-id="efbeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="efbeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efbeb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efbeb-126">Request body</span></span>
<span data-ttu-id="efbeb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="efbeb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efbeb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="efbeb-128">Response</span></span>
<span data-ttu-id="efbeb-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="efbeb-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="efbeb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efbeb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="efbeb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efbeb-131">Request</span></span>
<span data-ttu-id="efbeb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efbeb-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="efbeb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="efbeb-133">Response</span></span>
<span data-ttu-id="efbeb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efbeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






