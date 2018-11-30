---
title: Ação removeAllDevicesFromManagement
description: Desativa todos os dispositivos de gerenciamento deste usuário
ms.openlocfilehash: 973c9ccba2829161189595f58e918e3be1790476
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004523"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="75684-103">Ação removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="75684-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="75684-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="75684-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75684-105">Desativa todos os dispositivos de gerenciamento deste usuário</span><span class="sxs-lookup"><span data-stu-id="75684-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75684-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75684-106">Prerequisites</span></span>
<span data-ttu-id="75684-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75684-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75684-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75684-109">Permission type</span></span>|<span data-ttu-id="75684-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="75684-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75684-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75684-111">Delegated (work or school account)</span></span>| <span data-ttu-id="75684-112">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="75684-112">_varies by context_</span></span> |
| <span data-ttu-id="75684-113">&nbsp;&nbsp; Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="75684-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="75684-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="75684-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="75684-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75684-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75684-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75684-116">Not supported.</span></span>|
|<span data-ttu-id="75684-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75684-117">Application</span></span>|<span data-ttu-id="75684-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75684-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75684-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75684-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="75684-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75684-120">Request headers</span></span>
|<span data-ttu-id="75684-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75684-121">Header</span></span>|<span data-ttu-id="75684-122">Valor</span><span class="sxs-lookup"><span data-stu-id="75684-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75684-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="75684-123">Authorization</span></span>|<span data-ttu-id="75684-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75684-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75684-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75684-125">Accept</span></span>|<span data-ttu-id="75684-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75684-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75684-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75684-127">Request body</span></span>
<span data-ttu-id="75684-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75684-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75684-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="75684-129">Response</span></span>
<span data-ttu-id="75684-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="75684-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="75684-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75684-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="75684-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75684-132">Request</span></span>
<span data-ttu-id="75684-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75684-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="75684-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="75684-134">Response</span></span>
<span data-ttu-id="75684-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75684-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



