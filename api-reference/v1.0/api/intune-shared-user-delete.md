---
title: Excluir usuário
description: Exclui usuário.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d983e4506b55ac5e3af05e214fb0c90b2f8d883
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511996"
---
# <a name="delete-user"></a><span data-ttu-id="8e4fc-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="8e4fc-103">Delete user</span></span>

<span data-ttu-id="8e4fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e4fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e4fc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e4fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e4fc-106">Exclui [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="8e4fc-106">Deletes a [user](../resources/intune-shared-user.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e4fc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e4fc-107">Prerequisites</span></span>
<span data-ttu-id="8e4fc-108">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8e4fc-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8e4fc-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e4fc-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="8e4fc-110">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="8e4fc-110">The specific permission required depends on context.</span></span>

|<span data-ttu-id="8e4fc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e4fc-111">Permission type</span></span>|<span data-ttu-id="8e4fc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e4fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e4fc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e4fc-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8e4fc-114">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="8e4fc-114">_varies by context_</span></span>|
| <span data-ttu-id="8e4fc-115">&nbsp;&nbsp; Dispositivos</span><span class="sxs-lookup"><span data-stu-id="8e4fc-115">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="8e4fc-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e4fc-116">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="8e4fc-117">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="8e4fc-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="8e4fc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e4fc-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="8e4fc-119">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="8e4fc-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="8e4fc-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e4fc-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="8e4fc-121">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="8e4fc-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="8e4fc-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e4fc-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="8e4fc-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e4fc-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e4fc-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e4fc-124">Not supported.</span></span>|
|<span data-ttu-id="8e4fc-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e4fc-125">Application</span></span>|<span data-ttu-id="8e4fc-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e4fc-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e4fc-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e4fc-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="8e4fc-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e4fc-128">Request headers</span></span>
|<span data-ttu-id="8e4fc-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e4fc-129">Header</span></span>|<span data-ttu-id="8e4fc-130">Valor</span><span class="sxs-lookup"><span data-stu-id="8e4fc-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e4fc-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e4fc-131">Authorization</span></span>|<span data-ttu-id="8e4fc-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e4fc-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e4fc-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e4fc-133">Accept</span></span>|<span data-ttu-id="8e4fc-134">application/json</span><span class="sxs-lookup"><span data-stu-id="8e4fc-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e4fc-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e4fc-135">Request body</span></span>
<span data-ttu-id="8e4fc-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e4fc-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e4fc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e4fc-137">Response</span></span>
<span data-ttu-id="8e4fc-138">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8e4fc-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8e4fc-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e4fc-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e4fc-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e4fc-140">Request</span></span>
<span data-ttu-id="8e4fc-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e4fc-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="8e4fc-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e4fc-142">Response</span></span>
<span data-ttu-id="8e4fc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e4fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




