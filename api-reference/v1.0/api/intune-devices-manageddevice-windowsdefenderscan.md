---
title: Ação windowsDefenderScan
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: abd1cd6bfe2d4d0f9ebb96e433ad0db191b76366
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752627"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="3189f-103">Ação windowsDefenderScan</span><span class="sxs-lookup"><span data-stu-id="3189f-103">windowsDefenderScan action</span></span>

<span data-ttu-id="3189f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3189f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3189f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3189f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3189f-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3189f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3189f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3189f-107">Prerequisites</span></span>
<span data-ttu-id="3189f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3189f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3189f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3189f-110">Permission type</span></span>|<span data-ttu-id="3189f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3189f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3189f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3189f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3189f-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="3189f-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="3189f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3189f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3189f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3189f-115">Not supported.</span></span>|
|<span data-ttu-id="3189f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3189f-116">Application</span></span>|<span data-ttu-id="3189f-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="3189f-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3189f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3189f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="3189f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3189f-119">Request headers</span></span>
|<span data-ttu-id="3189f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3189f-120">Header</span></span>|<span data-ttu-id="3189f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3189f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3189f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3189f-122">Authorization</span></span>|<span data-ttu-id="3189f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3189f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3189f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3189f-124">Accept</span></span>|<span data-ttu-id="3189f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3189f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3189f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3189f-126">Request body</span></span>
<span data-ttu-id="3189f-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3189f-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3189f-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3189f-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3189f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3189f-129">Property</span></span>|<span data-ttu-id="3189f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3189f-130">Type</span></span>|<span data-ttu-id="3189f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3189f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3189f-132">quickScan</span><span class="sxs-lookup"><span data-stu-id="3189f-132">quickScan</span></span>|<span data-ttu-id="3189f-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="3189f-133">Boolean</span></span>|<span data-ttu-id="3189f-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3189f-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3189f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3189f-135">Response</span></span>
<span data-ttu-id="3189f-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3189f-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3189f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3189f-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="3189f-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3189f-138">Request</span></span>
<span data-ttu-id="3189f-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3189f-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="3189f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3189f-140">Response</span></span>
<span data-ttu-id="3189f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3189f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




