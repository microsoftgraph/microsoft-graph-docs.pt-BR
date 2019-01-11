---
title: Excluir usuário
description: Exclui usuário.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cc1979284cada76f76a98acc8956271b7224aa53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837832"
---
# <a name="delete-user"></a><span data-ttu-id="db3c7-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="db3c7-103">Delete user</span></span>

> <span data-ttu-id="db3c7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="db3c7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db3c7-105">Exclui [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="db3c7-105">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db3c7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db3c7-106">Prerequisites</span></span>
<span data-ttu-id="db3c7-107">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="db3c7-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="db3c7-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db3c7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="db3c7-109">A permissão específica necessária depende de contexto.</span><span class="sxs-lookup"><span data-stu-id="db3c7-109">The specific permission required depends on context.</span></span>

|<span data-ttu-id="db3c7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db3c7-110">Permission type</span></span>|<span data-ttu-id="db3c7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="db3c7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db3c7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db3c7-112">Delegated (work or school account)</span></span>| <span data-ttu-id="db3c7-113">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="db3c7-113">_varies by context_</span></span>|
| <span data-ttu-id="db3c7-114">&nbsp;&nbsp; Dispositivos</span><span class="sxs-lookup"><span data-stu-id="db3c7-114">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="db3c7-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db3c7-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="db3c7-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="db3c7-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="db3c7-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db3c7-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="db3c7-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="db3c7-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="db3c7-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db3c7-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="db3c7-120">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="db3c7-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="db3c7-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db3c7-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="db3c7-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db3c7-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db3c7-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db3c7-123">Not supported.</span></span>|
|<span data-ttu-id="db3c7-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db3c7-124">Application</span></span>|<span data-ttu-id="db3c7-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db3c7-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db3c7-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db3c7-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="db3c7-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db3c7-127">Request headers</span></span>
|<span data-ttu-id="db3c7-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db3c7-128">Header</span></span>|<span data-ttu-id="db3c7-129">Valor</span><span class="sxs-lookup"><span data-stu-id="db3c7-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db3c7-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="db3c7-130">Authorization</span></span>|<span data-ttu-id="db3c7-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db3c7-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db3c7-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db3c7-132">Accept</span></span>|<span data-ttu-id="db3c7-133">application/json</span><span class="sxs-lookup"><span data-stu-id="db3c7-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db3c7-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db3c7-134">Request body</span></span>
<span data-ttu-id="db3c7-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db3c7-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db3c7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="db3c7-136">Response</span></span>
<span data-ttu-id="db3c7-137">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="db3c7-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="db3c7-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db3c7-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="db3c7-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db3c7-139">Request</span></span>
<span data-ttu-id="db3c7-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db3c7-140">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="db3c7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="db3c7-141">Response</span></span>
<span data-ttu-id="db3c7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db3c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



