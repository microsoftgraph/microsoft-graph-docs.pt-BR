---
title: Ação wipe
description: Apagar um dispositivo
ms.openlocfilehash: 377b1c299885d042dd372f661410ea43d20fd021
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005193"
---
# <a name="wipe-action"></a><span data-ttu-id="80169-103">Ação wipe</span><span class="sxs-lookup"><span data-stu-id="80169-103">wipe action</span></span>

> <span data-ttu-id="80169-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="80169-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80169-105">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="80169-105">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80169-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80169-106">Prerequisites</span></span>
<span data-ttu-id="80169-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80169-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80169-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80169-109">Permission type</span></span>|<span data-ttu-id="80169-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80169-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80169-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80169-111">Delegated (work or school account)</span></span>|<span data-ttu-id="80169-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="80169-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="80169-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80169-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80169-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80169-114">Not supported.</span></span>|
|<span data-ttu-id="80169-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80169-115">Application</span></span>|<span data-ttu-id="80169-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80169-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80169-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80169-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="80169-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80169-118">Request headers</span></span>
|<span data-ttu-id="80169-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80169-119">Header</span></span>|<span data-ttu-id="80169-120">Valor</span><span class="sxs-lookup"><span data-stu-id="80169-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80169-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="80169-121">Authorization</span></span>|<span data-ttu-id="80169-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80169-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80169-123">Accept</span><span class="sxs-lookup"><span data-stu-id="80169-123">Accept</span></span>|<span data-ttu-id="80169-124">application/json</span><span class="sxs-lookup"><span data-stu-id="80169-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80169-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80169-125">Request body</span></span>
<span data-ttu-id="80169-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="80169-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="80169-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="80169-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="80169-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80169-128">Property</span></span>|<span data-ttu-id="80169-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="80169-129">Type</span></span>|<span data-ttu-id="80169-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="80169-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80169-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="80169-131">keepEnrollmentData</span></span>|<span data-ttu-id="80169-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="80169-132">Boolean</span></span>|<span data-ttu-id="80169-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="80169-133">Not yet documented</span></span>|
|<span data-ttu-id="80169-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="80169-134">keepUserData</span></span>|<span data-ttu-id="80169-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="80169-135">Boolean</span></span>|<span data-ttu-id="80169-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="80169-136">Not yet documented</span></span>|
|<span data-ttu-id="80169-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="80169-137">macOsUnlockCode</span></span>|<span data-ttu-id="80169-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80169-138">String</span></span>|<span data-ttu-id="80169-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="80169-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="80169-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="80169-140">Response</span></span>
<span data-ttu-id="80169-141">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="80169-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="80169-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80169-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="80169-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80169-143">Request</span></span>
<span data-ttu-id="80169-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80169-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80169-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="80169-145">Response</span></span>
<span data-ttu-id="80169-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80169-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



