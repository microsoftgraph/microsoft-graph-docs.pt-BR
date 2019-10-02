---
title: Ação windowsDefenderScan
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 69cf648d2c41592bb696b83558648bc995341b43
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364239"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="68e30-103">Ação windowsDefenderScan</span><span class="sxs-lookup"><span data-stu-id="68e30-103">windowsDefenderScan action</span></span>

> <span data-ttu-id="68e30-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68e30-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68e30-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="68e30-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68e30-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68e30-106">Prerequisites</span></span>
<span data-ttu-id="68e30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68e30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68e30-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68e30-109">Permission type</span></span>|<span data-ttu-id="68e30-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="68e30-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68e30-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68e30-111">Delegated (work or school account)</span></span>|<span data-ttu-id="68e30-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="68e30-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="68e30-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68e30-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68e30-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68e30-114">Not supported.</span></span>|
|<span data-ttu-id="68e30-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68e30-115">Application</span></span>|<span data-ttu-id="68e30-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68e30-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68e30-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68e30-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="68e30-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68e30-118">Request headers</span></span>
|<span data-ttu-id="68e30-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68e30-119">Header</span></span>|<span data-ttu-id="68e30-120">Valor</span><span class="sxs-lookup"><span data-stu-id="68e30-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68e30-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="68e30-121">Authorization</span></span>|<span data-ttu-id="68e30-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68e30-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68e30-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="68e30-123">Accept</span></span>|<span data-ttu-id="68e30-124">application/json</span><span class="sxs-lookup"><span data-stu-id="68e30-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68e30-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68e30-125">Request body</span></span>
<span data-ttu-id="68e30-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="68e30-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="68e30-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="68e30-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="68e30-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68e30-128">Property</span></span>|<span data-ttu-id="68e30-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="68e30-129">Type</span></span>|<span data-ttu-id="68e30-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="68e30-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68e30-131">quickScan</span><span class="sxs-lookup"><span data-stu-id="68e30-131">quickScan</span></span>|<span data-ttu-id="68e30-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="68e30-132">Boolean</span></span>|<span data-ttu-id="68e30-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="68e30-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="68e30-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="68e30-134">Response</span></span>
<span data-ttu-id="68e30-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="68e30-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="68e30-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68e30-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="68e30-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68e30-137">Request</span></span>
<span data-ttu-id="68e30-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68e30-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="68e30-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="68e30-139">Response</span></span>
<span data-ttu-id="68e30-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68e30-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




