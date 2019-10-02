---
title: Ação wipe
description: Apagar um dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56d29523f42f1948548bc9a3c16fd988a32ae6c4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364225"
---
# <a name="wipe-action"></a><span data-ttu-id="bb4c1-103">ação wipe</span><span class="sxs-lookup"><span data-stu-id="bb4c1-103">wipe action</span></span>

> <span data-ttu-id="bb4c1-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb4c1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb4c1-105">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="bb4c1-105">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb4c1-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb4c1-106">Prerequisites</span></span>
<span data-ttu-id="bb4c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb4c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb4c1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb4c1-109">Permission type</span></span>|<span data-ttu-id="bb4c1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb4c1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb4c1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb4c1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb4c1-112">DeviceManagementManagedDevices. PriviligedOperation. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bb4c1-112">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bb4c1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb4c1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb4c1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb4c1-114">Not supported.</span></span>|
|<span data-ttu-id="bb4c1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb4c1-115">Application</span></span>|<span data-ttu-id="bb4c1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb4c1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb4c1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb4c1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="bb4c1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb4c1-118">Request headers</span></span>
|<span data-ttu-id="bb4c1-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb4c1-119">Header</span></span>|<span data-ttu-id="bb4c1-120">Valor</span><span class="sxs-lookup"><span data-stu-id="bb4c1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb4c1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb4c1-121">Authorization</span></span>|<span data-ttu-id="bb4c1-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb4c1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb4c1-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb4c1-123">Accept</span></span>|<span data-ttu-id="bb4c1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb4c1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb4c1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb4c1-125">Request body</span></span>
<span data-ttu-id="bb4c1-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="bb4c1-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bb4c1-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="bb4c1-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bb4c1-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb4c1-128">Property</span></span>|<span data-ttu-id="bb4c1-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb4c1-129">Type</span></span>|<span data-ttu-id="bb4c1-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb4c1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb4c1-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="bb4c1-131">keepEnrollmentData</span></span>|<span data-ttu-id="bb4c1-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb4c1-132">Boolean</span></span>|<span data-ttu-id="bb4c1-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bb4c1-133">Not yet documented</span></span>|
|<span data-ttu-id="bb4c1-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="bb4c1-134">keepUserData</span></span>|<span data-ttu-id="bb4c1-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb4c1-135">Boolean</span></span>|<span data-ttu-id="bb4c1-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bb4c1-136">Not yet documented</span></span>|
|<span data-ttu-id="bb4c1-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="bb4c1-137">macOsUnlockCode</span></span>|<span data-ttu-id="bb4c1-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb4c1-138">String</span></span>|<span data-ttu-id="bb4c1-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bb4c1-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bb4c1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb4c1-140">Response</span></span>
<span data-ttu-id="bb4c1-141">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bb4c1-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bb4c1-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb4c1-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb4c1-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb4c1-143">Request</span></span>
<span data-ttu-id="bb4c1-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb4c1-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="bb4c1-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb4c1-145">Response</span></span>
<span data-ttu-id="bb4c1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb4c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




