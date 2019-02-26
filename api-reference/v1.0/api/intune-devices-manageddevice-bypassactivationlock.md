---
title: Ação bypassActivationLock
description: Ignorar bloqueio de ativação
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8abc365a0c37566f5cb1933870c0b39e2cf06564
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258776"
---
# <a name="bypassactivationlock-action"></a><span data-ttu-id="51f11-103">Ação bypassActivationLock</span><span class="sxs-lookup"><span data-stu-id="51f11-103">bypassActivationLock action</span></span>

> <span data-ttu-id="51f11-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51f11-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51f11-105">Ignorar bloqueio de ativação</span><span class="sxs-lookup"><span data-stu-id="51f11-105">Bypass activation lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51f11-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51f11-106">Prerequisites</span></span>
<span data-ttu-id="51f11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="51f11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="51f11-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51f11-109">Permission type</span></span>|<span data-ttu-id="51f11-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51f11-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51f11-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51f11-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51f11-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="51f11-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="51f11-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51f11-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51f11-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51f11-114">Not supported.</span></span>|
|<span data-ttu-id="51f11-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51f11-115">Application</span></span>|<span data-ttu-id="51f11-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51f11-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51f11-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51f11-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/bypassActivationLock
POST /deviceManagement/managedDevices/{managedDeviceId}/bypassActivationLock
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/bypassActivationLock
```

## <a name="request-headers"></a><span data-ttu-id="51f11-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51f11-118">Request headers</span></span>
|<span data-ttu-id="51f11-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51f11-119">Header</span></span>|<span data-ttu-id="51f11-120">Valor</span><span class="sxs-lookup"><span data-stu-id="51f11-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51f11-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="51f11-121">Authorization</span></span>|<span data-ttu-id="51f11-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51f11-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51f11-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51f11-123">Accept</span></span>|<span data-ttu-id="51f11-124">application/json</span><span class="sxs-lookup"><span data-stu-id="51f11-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51f11-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51f11-125">Request body</span></span>
<span data-ttu-id="51f11-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51f11-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51f11-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="51f11-127">Response</span></span>
<span data-ttu-id="51f11-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="51f11-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="51f11-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51f11-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="51f11-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51f11-130">Request</span></span>
<span data-ttu-id="51f11-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51f11-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/bypassActivationLock
```

### <a name="response"></a><span data-ttu-id="51f11-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="51f11-132">Response</span></span>
<span data-ttu-id="51f11-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51f11-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



