---
title: Excluir usuário
description: Exclui usuário.
ms.openlocfilehash: 3b580e46fe15e81e0325f9b673217e41274b8721
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006028"
---
# <a name="delete-user"></a><span data-ttu-id="68a94-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="68a94-103">Delete user</span></span>

> <span data-ttu-id="68a94-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="68a94-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68a94-105">Exclui [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="68a94-105">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68a94-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68a94-106">Prerequisites</span></span>
<span data-ttu-id="68a94-107">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="68a94-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="68a94-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68a94-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="68a94-109">A permissão específica necessária depende de contexto.</span><span class="sxs-lookup"><span data-stu-id="68a94-109">The specific permission required depends on context.</span></span>

|<span data-ttu-id="68a94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68a94-110">Permission type</span></span>|<span data-ttu-id="68a94-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="68a94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68a94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68a94-112">Delegated (work or school account)</span></span>| <span data-ttu-id="68a94-113">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="68a94-113">_varies by context_</span></span>|
| <span data-ttu-id="68a94-114">&nbsp;&nbsp; Dispositivos</span><span class="sxs-lookup"><span data-stu-id="68a94-114">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="68a94-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68a94-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="68a94-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="68a94-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="68a94-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68a94-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="68a94-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="68a94-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="68a94-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68a94-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="68a94-120">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="68a94-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="68a94-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68a94-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="68a94-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68a94-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68a94-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68a94-123">Not supported.</span></span>|
|<span data-ttu-id="68a94-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68a94-124">Application</span></span>|<span data-ttu-id="68a94-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68a94-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68a94-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68a94-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="68a94-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68a94-127">Request headers</span></span>
|<span data-ttu-id="68a94-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68a94-128">Header</span></span>|<span data-ttu-id="68a94-129">Valor</span><span class="sxs-lookup"><span data-stu-id="68a94-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68a94-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="68a94-130">Authorization</span></span>|<span data-ttu-id="68a94-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68a94-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68a94-132">Accept</span><span class="sxs-lookup"><span data-stu-id="68a94-132">Accept</span></span>|<span data-ttu-id="68a94-133">application/json</span><span class="sxs-lookup"><span data-stu-id="68a94-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68a94-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68a94-134">Request body</span></span>
<span data-ttu-id="68a94-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="68a94-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68a94-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="68a94-136">Response</span></span>
<span data-ttu-id="68a94-137">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="68a94-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="68a94-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68a94-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="68a94-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68a94-139">Request</span></span>
<span data-ttu-id="68a94-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68a94-140">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="68a94-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="68a94-141">Response</span></span>
<span data-ttu-id="68a94-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68a94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



