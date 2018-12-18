---
title: Ação requestRemoteAssistance
description: Solicitar assistência remota
author: tfitzmac
ms.openlocfilehash: d2668ff42571f285f7b7f40f0a514e42d78f9fd0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336803"
---
# <a name="requestremoteassistance-action"></a><span data-ttu-id="a3446-103">Ação requestRemoteAssistance</span><span class="sxs-lookup"><span data-stu-id="a3446-103">requestRemoteAssistance action</span></span>

> <span data-ttu-id="a3446-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a3446-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3446-105">Solicitar assistência remota</span><span class="sxs-lookup"><span data-stu-id="a3446-105">Request remote assistance</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3446-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3446-106">Prerequisites</span></span>
<span data-ttu-id="a3446-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3446-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3446-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3446-109">Permission type</span></span>|<span data-ttu-id="a3446-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a3446-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3446-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3446-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3446-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3446-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a3446-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3446-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3446-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3446-114">Not supported.</span></span>|
|<span data-ttu-id="a3446-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3446-115">Application</span></span>|<span data-ttu-id="a3446-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3446-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3446-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3446-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

## <a name="request-headers"></a><span data-ttu-id="a3446-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3446-118">Request headers</span></span>
|<span data-ttu-id="a3446-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3446-119">Header</span></span>|<span data-ttu-id="a3446-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a3446-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3446-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3446-121">Authorization</span></span>|<span data-ttu-id="a3446-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3446-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3446-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a3446-123">Accept</span></span>|<span data-ttu-id="a3446-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3446-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3446-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3446-125">Request body</span></span>
<span data-ttu-id="a3446-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3446-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3446-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3446-127">Response</span></span>
<span data-ttu-id="a3446-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a3446-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a3446-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3446-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3446-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3446-130">Request</span></span>
<span data-ttu-id="a3446-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3446-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

### <a name="response"></a><span data-ttu-id="a3446-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3446-132">Response</span></span>
<span data-ttu-id="a3446-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3446-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



