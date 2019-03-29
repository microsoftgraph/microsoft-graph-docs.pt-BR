---
title: Ação disableLostMode
description: Desabilitar o modo perdido
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a377869d236f06921bd2a3d7fe5d5dea8659c81a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956818"
---
# <a name="disablelostmode-action"></a><span data-ttu-id="0a526-103">Ação disableLostMode</span><span class="sxs-lookup"><span data-stu-id="0a526-103">disableLostMode action</span></span>

> <span data-ttu-id="0a526-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a526-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a526-105">Desabilitar o modo perdido</span><span class="sxs-lookup"><span data-stu-id="0a526-105">Disable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a526-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a526-106">Prerequisites</span></span>
<span data-ttu-id="0a526-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a526-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a526-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a526-109">Permission type</span></span>|<span data-ttu-id="0a526-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a526-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a526-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a526-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a526-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="0a526-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="0a526-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a526-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a526-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a526-114">Not supported.</span></span>|
|<span data-ttu-id="0a526-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a526-115">Application</span></span>|<span data-ttu-id="0a526-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a526-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a526-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a526-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/disableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="0a526-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a526-118">Request headers</span></span>
|<span data-ttu-id="0a526-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a526-119">Header</span></span>|<span data-ttu-id="0a526-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0a526-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a526-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a526-121">Authorization</span></span>|<span data-ttu-id="0a526-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a526-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a526-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a526-123">Accept</span></span>|<span data-ttu-id="0a526-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0a526-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a526-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a526-125">Request body</span></span>
<span data-ttu-id="0a526-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a526-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a526-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a526-127">Response</span></span>
<span data-ttu-id="0a526-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0a526-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0a526-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a526-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a526-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a526-130">Request</span></span>
<span data-ttu-id="0a526-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a526-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/disableLostMode
```

### <a name="response"></a><span data-ttu-id="0a526-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a526-132">Response</span></span>
<span data-ttu-id="0a526-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a526-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



