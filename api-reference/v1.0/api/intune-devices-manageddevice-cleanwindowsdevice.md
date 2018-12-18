---
title: Ação cleanWindowsDevice
description: Limpar dispositivo Windows
author: tfitzmac
ms.openlocfilehash: 9d19b71f200381c10b7501eadf9007162ff9fff3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301761"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="0f7f3-103">Ação cleanWindowsDevice</span><span class="sxs-lookup"><span data-stu-id="0f7f3-103">cleanWindowsDevice action</span></span>

> <span data-ttu-id="0f7f3-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0f7f3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f7f3-105">Limpar dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="0f7f3-105">Clean Windows device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f7f3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f7f3-106">Prerequisites</span></span>
<span data-ttu-id="0f7f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f7f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f7f3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f7f3-109">Permission type</span></span>|<span data-ttu-id="0f7f3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f7f3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f7f3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f7f3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f7f3-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="0f7f3-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="0f7f3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f7f3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f7f3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f7f3-114">Not supported.</span></span>|
|<span data-ttu-id="0f7f3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f7f3-115">Application</span></span>|<span data-ttu-id="0f7f3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f7f3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f7f3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f7f3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="0f7f3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f7f3-118">Request headers</span></span>
|<span data-ttu-id="0f7f3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f7f3-119">Header</span></span>|<span data-ttu-id="0f7f3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0f7f3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f7f3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f7f3-121">Authorization</span></span>|<span data-ttu-id="0f7f3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f7f3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f7f3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0f7f3-123">Accept</span></span>|<span data-ttu-id="0f7f3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0f7f3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f7f3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f7f3-125">Request body</span></span>
<span data-ttu-id="0f7f3-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0f7f3-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0f7f3-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0f7f3-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0f7f3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f7f3-128">Property</span></span>|<span data-ttu-id="0f7f3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f7f3-129">Type</span></span>|<span data-ttu-id="0f7f3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f7f3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f7f3-131">keepUserData</span><span class="sxs-lookup"><span data-stu-id="0f7f3-131">keepUserData</span></span>|<span data-ttu-id="0f7f3-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f7f3-132">Boolean</span></span>|<span data-ttu-id="0f7f3-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0f7f3-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0f7f3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f7f3-134">Response</span></span>
<span data-ttu-id="0f7f3-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0f7f3-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0f7f3-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f7f3-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f7f3-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f7f3-137">Request</span></span>
<span data-ttu-id="0f7f3-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f7f3-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="0f7f3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f7f3-139">Response</span></span>
<span data-ttu-id="0f7f3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f7f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



