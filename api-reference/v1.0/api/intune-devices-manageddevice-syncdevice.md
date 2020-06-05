---
title: Ação syncDevice
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6ad60082606f1dd55c7836267b892e760395638f
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556195"
---
# <a name="syncdevice-action"></a><span data-ttu-id="57c84-103">Ação syncDevice</span><span class="sxs-lookup"><span data-stu-id="57c84-103">syncDevice action</span></span>

<span data-ttu-id="57c84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57c84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57c84-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57c84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57c84-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="57c84-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57c84-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57c84-107">Prerequisites</span></span>
<span data-ttu-id="57c84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57c84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57c84-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57c84-110">Permission type</span></span>|<span data-ttu-id="57c84-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57c84-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57c84-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57c84-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57c84-113">DeviceManagementManagedDevices.PrivilegedOperations.All</span><span class="sxs-lookup"><span data-stu-id="57c84-113">DeviceManagementManagedDevices.PrivilegedOperations.All</span></span>|
|<span data-ttu-id="57c84-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57c84-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57c84-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57c84-115">Not supported.</span></span>|
|<span data-ttu-id="57c84-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57c84-116">Application</span></span>|<span data-ttu-id="57c84-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57c84-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57c84-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57c84-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/syncDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/syncDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/syncDevice
```

## <a name="request-headers"></a><span data-ttu-id="57c84-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57c84-119">Request headers</span></span>
|<span data-ttu-id="57c84-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57c84-120">Header</span></span>|<span data-ttu-id="57c84-121">Valor</span><span class="sxs-lookup"><span data-stu-id="57c84-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57c84-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="57c84-122">Authorization</span></span>|<span data-ttu-id="57c84-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57c84-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57c84-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57c84-124">Accept</span></span>|<span data-ttu-id="57c84-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57c84-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57c84-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57c84-126">Request body</span></span>
<span data-ttu-id="57c84-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57c84-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57c84-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="57c84-128">Response</span></span>
<span data-ttu-id="57c84-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="57c84-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="57c84-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57c84-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="57c84-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57c84-131">Request</span></span>
<span data-ttu-id="57c84-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57c84-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/syncDevice
```

### <a name="response"></a><span data-ttu-id="57c84-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="57c84-133">Response</span></span>
<span data-ttu-id="57c84-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57c84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






