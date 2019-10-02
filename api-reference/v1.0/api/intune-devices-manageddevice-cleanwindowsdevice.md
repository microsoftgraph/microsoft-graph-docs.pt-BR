---
title: Ação cleanWindowsDevice
description: Limpar dispositivo Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b21b986c3ffeb1338461e7fdffd7829a7eae1348
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364512"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="fdf00-103">Ação cleanWindowsDevice</span><span class="sxs-lookup"><span data-stu-id="fdf00-103">cleanWindowsDevice action</span></span>

> <span data-ttu-id="fdf00-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fdf00-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdf00-105">Limpar dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="fdf00-105">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdf00-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fdf00-106">Prerequisites</span></span>
<span data-ttu-id="fdf00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdf00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdf00-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdf00-109">Permission type</span></span>|<span data-ttu-id="fdf00-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fdf00-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdf00-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdf00-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fdf00-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="fdf00-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="fdf00-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdf00-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdf00-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdf00-114">Not supported.</span></span>|
|<span data-ttu-id="fdf00-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdf00-115">Application</span></span>|<span data-ttu-id="fdf00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdf00-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdf00-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdf00-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="fdf00-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf00-118">Request headers</span></span>
|<span data-ttu-id="fdf00-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdf00-119">Header</span></span>|<span data-ttu-id="fdf00-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fdf00-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdf00-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdf00-121">Authorization</span></span>|<span data-ttu-id="fdf00-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdf00-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdf00-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fdf00-123">Accept</span></span>|<span data-ttu-id="fdf00-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fdf00-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdf00-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf00-125">Request body</span></span>
<span data-ttu-id="fdf00-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fdf00-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fdf00-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="fdf00-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fdf00-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdf00-128">Property</span></span>|<span data-ttu-id="fdf00-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdf00-129">Type</span></span>|<span data-ttu-id="fdf00-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdf00-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdf00-131">keepUserData</span><span class="sxs-lookup"><span data-stu-id="fdf00-131">keepUserData</span></span>|<span data-ttu-id="fdf00-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="fdf00-132">Boolean</span></span>|<span data-ttu-id="fdf00-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fdf00-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fdf00-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdf00-134">Response</span></span>
<span data-ttu-id="fdf00-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fdf00-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fdf00-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdf00-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdf00-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf00-137">Request</span></span>
<span data-ttu-id="fdf00-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdf00-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="fdf00-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdf00-139">Response</span></span>
<span data-ttu-id="fdf00-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdf00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




