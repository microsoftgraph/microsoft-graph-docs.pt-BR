---
title: Ação removeAllDevicesFromManagement
description: Desativa todos os dispositivos de gerenciamento deste usuário
ms.openlocfilehash: db3c4331f2d61730608275c07fd42c5e189bb28b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040662"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="df4a8-103">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="df4a8-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="df4a8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="df4a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df4a8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="df4a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df4a8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="df4a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df4a8-107">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="df4a8-107">Retire all devices from management for this user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df4a8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df4a8-108">Prerequisites</span></span>
<span data-ttu-id="df4a8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df4a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df4a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df4a8-111">Permission type</span></span>|<span data-ttu-id="df4a8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df4a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df4a8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df4a8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="df4a8-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="df4a8-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="df4a8-115">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="df4a8-115">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="df4a8-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df4a8-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df4a8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df4a8-117">Not supported.</span></span>|
|<span data-ttu-id="df4a8-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df4a8-118">Application</span></span>|<span data-ttu-id="df4a8-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df4a8-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df4a8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df4a8-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="df4a8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df4a8-121">Request headers</span></span>
|<span data-ttu-id="df4a8-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df4a8-122">Header</span></span>|<span data-ttu-id="df4a8-123">Valor</span><span class="sxs-lookup"><span data-stu-id="df4a8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df4a8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="df4a8-124">Authorization</span></span>|<span data-ttu-id="df4a8-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df4a8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df4a8-126">Accept</span><span class="sxs-lookup"><span data-stu-id="df4a8-126">Accept</span></span>|<span data-ttu-id="df4a8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="df4a8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df4a8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df4a8-128">Request body</span></span>
<span data-ttu-id="df4a8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df4a8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df4a8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="df4a8-130">Response</span></span>
<span data-ttu-id="df4a8-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="df4a8-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df4a8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df4a8-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="df4a8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df4a8-133">Request</span></span>
<span data-ttu-id="df4a8-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df4a8-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="df4a8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="df4a8-135">Response</span></span>
<span data-ttu-id="df4a8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df4a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





