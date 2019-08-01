---
title: Ação locateDevice
description: Localizar um dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a5ad1606494373d5183df4e3b53efc670dfd7514
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020973"
---
# <a name="locatedevice-action"></a><span data-ttu-id="a9e80-103">Ação locateDevice</span><span class="sxs-lookup"><span data-stu-id="a9e80-103">locateDevice action</span></span>

> <span data-ttu-id="a9e80-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9e80-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9e80-105">Localizar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="a9e80-105">Locate a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9e80-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9e80-106">Prerequisites</span></span>
<span data-ttu-id="a9e80-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9e80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9e80-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9e80-109">Permission type</span></span>|<span data-ttu-id="a9e80-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9e80-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9e80-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9e80-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9e80-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a9e80-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a9e80-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9e80-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9e80-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9e80-114">Not supported.</span></span>|
|<span data-ttu-id="a9e80-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9e80-115">Application</span></span>|<span data-ttu-id="a9e80-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9e80-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9e80-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9e80-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/locateDevice
```

## <a name="request-headers"></a><span data-ttu-id="a9e80-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9e80-118">Request headers</span></span>
|<span data-ttu-id="a9e80-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9e80-119">Header</span></span>|<span data-ttu-id="a9e80-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a9e80-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9e80-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9e80-121">Authorization</span></span>|<span data-ttu-id="a9e80-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9e80-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9e80-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9e80-123">Accept</span></span>|<span data-ttu-id="a9e80-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a9e80-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9e80-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9e80-125">Request body</span></span>
<span data-ttu-id="a9e80-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9e80-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9e80-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9e80-127">Response</span></span>
<span data-ttu-id="a9e80-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a9e80-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a9e80-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9e80-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9e80-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9e80-130">Request</span></span>
<span data-ttu-id="a9e80-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9e80-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/locateDevice
```

### <a name="response"></a><span data-ttu-id="a9e80-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9e80-132">Response</span></span>
<span data-ttu-id="a9e80-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9e80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



