---
title: Ação recoverPasscode
description: Recuperar senha
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c1479fc585f460997d032315e0e6f9e71bcc0a23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513522"
---
# <a name="recoverpasscode-action"></a><span data-ttu-id="e98be-103">Ação recoverPasscode</span><span class="sxs-lookup"><span data-stu-id="e98be-103">recoverPasscode action</span></span>

<span data-ttu-id="e98be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e98be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e98be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e98be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e98be-106">Recuperar senha</span><span class="sxs-lookup"><span data-stu-id="e98be-106">Recover passcode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e98be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e98be-107">Prerequisites</span></span>
<span data-ttu-id="e98be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e98be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e98be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e98be-110">Permission type</span></span>|<span data-ttu-id="e98be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e98be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e98be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e98be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e98be-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e98be-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e98be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e98be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e98be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e98be-115">Not supported.</span></span>|
|<span data-ttu-id="e98be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e98be-116">Application</span></span>|<span data-ttu-id="e98be-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e98be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e98be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e98be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/recoverPasscode
```

## <a name="request-headers"></a><span data-ttu-id="e98be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e98be-119">Request headers</span></span>
|<span data-ttu-id="e98be-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e98be-120">Header</span></span>|<span data-ttu-id="e98be-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e98be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e98be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e98be-122">Authorization</span></span>|<span data-ttu-id="e98be-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e98be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e98be-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e98be-124">Accept</span></span>|<span data-ttu-id="e98be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e98be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e98be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e98be-126">Request body</span></span>
<span data-ttu-id="e98be-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e98be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e98be-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e98be-128">Response</span></span>
<span data-ttu-id="e98be-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e98be-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e98be-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e98be-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e98be-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e98be-131">Request</span></span>
<span data-ttu-id="e98be-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e98be-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/recoverPasscode
```

### <a name="response"></a><span data-ttu-id="e98be-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e98be-133">Response</span></span>
<span data-ttu-id="e98be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e98be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




