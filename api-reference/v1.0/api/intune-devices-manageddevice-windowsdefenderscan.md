---
title: Ação windowsDefenderScan
description: Ainda não documentado
ms.openlocfilehash: ef4dcf4845bfc2d2e4883071abad42be01405445
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005798"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="a9255-103">Ação windowsDefenderScan</span><span class="sxs-lookup"><span data-stu-id="a9255-103">windowsDefenderScan action</span></span>

> <span data-ttu-id="a9255-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a9255-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9255-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a9255-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9255-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9255-106">Prerequisites</span></span>
<span data-ttu-id="a9255-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9255-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9255-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9255-109">Permission type</span></span>|<span data-ttu-id="a9255-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9255-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9255-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9255-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9255-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a9255-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a9255-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9255-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9255-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9255-114">Not supported.</span></span>|
|<span data-ttu-id="a9255-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9255-115">Application</span></span>|<span data-ttu-id="a9255-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9255-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9255-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9255-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="a9255-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9255-118">Request headers</span></span>
|<span data-ttu-id="a9255-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9255-119">Header</span></span>|<span data-ttu-id="a9255-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a9255-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9255-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9255-121">Authorization</span></span>|<span data-ttu-id="a9255-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9255-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9255-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a9255-123">Accept</span></span>|<span data-ttu-id="a9255-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a9255-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9255-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9255-125">Request body</span></span>
<span data-ttu-id="a9255-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a9255-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a9255-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="a9255-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a9255-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9255-128">Property</span></span>|<span data-ttu-id="a9255-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9255-129">Type</span></span>|<span data-ttu-id="a9255-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9255-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9255-131">quickScan</span><span class="sxs-lookup"><span data-stu-id="a9255-131">quickScan</span></span>|<span data-ttu-id="a9255-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9255-132">Boolean</span></span>|<span data-ttu-id="a9255-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a9255-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a9255-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9255-134">Response</span></span>
<span data-ttu-id="a9255-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a9255-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a9255-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9255-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9255-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9255-137">Request</span></span>
<span data-ttu-id="a9255-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9255-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="a9255-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9255-139">Response</span></span>
<span data-ttu-id="a9255-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9255-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



