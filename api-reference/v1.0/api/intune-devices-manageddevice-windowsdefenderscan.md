---
title: Ação windowsDefenderScan
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 96bf4d8c10ee48883d2e63f0f283db776cbf3628
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513459"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="ada33-103">Ação windowsDefenderScan</span><span class="sxs-lookup"><span data-stu-id="ada33-103">windowsDefenderScan action</span></span>

<span data-ttu-id="ada33-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ada33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ada33-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ada33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ada33-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ada33-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ada33-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ada33-107">Prerequisites</span></span>
<span data-ttu-id="ada33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ada33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ada33-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ada33-110">Permission type</span></span>|<span data-ttu-id="ada33-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ada33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ada33-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ada33-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ada33-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ada33-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ada33-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ada33-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ada33-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ada33-115">Not supported.</span></span>|
|<span data-ttu-id="ada33-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ada33-116">Application</span></span>|<span data-ttu-id="ada33-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ada33-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ada33-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ada33-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="ada33-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ada33-119">Request headers</span></span>
|<span data-ttu-id="ada33-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ada33-120">Header</span></span>|<span data-ttu-id="ada33-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ada33-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ada33-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ada33-122">Authorization</span></span>|<span data-ttu-id="ada33-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ada33-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ada33-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ada33-124">Accept</span></span>|<span data-ttu-id="ada33-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ada33-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ada33-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ada33-126">Request body</span></span>
<span data-ttu-id="ada33-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ada33-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ada33-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ada33-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ada33-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ada33-129">Property</span></span>|<span data-ttu-id="ada33-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ada33-130">Type</span></span>|<span data-ttu-id="ada33-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ada33-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ada33-132">quickScan</span><span class="sxs-lookup"><span data-stu-id="ada33-132">quickScan</span></span>|<span data-ttu-id="ada33-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="ada33-133">Boolean</span></span>|<span data-ttu-id="ada33-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ada33-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ada33-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ada33-135">Response</span></span>
<span data-ttu-id="ada33-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ada33-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ada33-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ada33-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="ada33-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ada33-138">Request</span></span>
<span data-ttu-id="ada33-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ada33-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="ada33-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ada33-140">Response</span></span>
<span data-ttu-id="ada33-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ada33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




