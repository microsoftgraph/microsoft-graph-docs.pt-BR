---
title: Excluir usuário
description: Exclui usuário.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 876a155a5bc6a1cd609d446682195f1198e3ca01
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361312"
---
# <a name="delete-user"></a><span data-ttu-id="51a8f-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="51a8f-103">Delete user</span></span>

> <span data-ttu-id="51a8f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51a8f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51a8f-105">Exclui [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="51a8f-105">Deletes a [user](../resources/intune-shared-user.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51a8f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51a8f-106">Prerequisites</span></span>
<span data-ttu-id="51a8f-107">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="51a8f-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="51a8f-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51a8f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="51a8f-109">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="51a8f-109">The specific permission required depends on context.</span></span>

|<span data-ttu-id="51a8f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51a8f-110">Permission type</span></span>|<span data-ttu-id="51a8f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51a8f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51a8f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51a8f-112">Delegated (work or school account)</span></span>| <span data-ttu-id="51a8f-113">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="51a8f-113">_varies by context_</span></span>|
| <span data-ttu-id="51a8f-114">&nbsp;&nbsp; Dispositivos</span><span class="sxs-lookup"><span data-stu-id="51a8f-114">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="51a8f-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51a8f-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="51a8f-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="51a8f-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="51a8f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51a8f-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="51a8f-118">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="51a8f-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="51a8f-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51a8f-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="51a8f-120">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="51a8f-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="51a8f-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51a8f-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="51a8f-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51a8f-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51a8f-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51a8f-123">Not supported.</span></span>|
|<span data-ttu-id="51a8f-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51a8f-124">Application</span></span>|<span data-ttu-id="51a8f-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51a8f-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51a8f-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51a8f-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="51a8f-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51a8f-127">Request headers</span></span>
|<span data-ttu-id="51a8f-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51a8f-128">Header</span></span>|<span data-ttu-id="51a8f-129">Valor</span><span class="sxs-lookup"><span data-stu-id="51a8f-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51a8f-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="51a8f-130">Authorization</span></span>|<span data-ttu-id="51a8f-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51a8f-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51a8f-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51a8f-132">Accept</span></span>|<span data-ttu-id="51a8f-133">application/json</span><span class="sxs-lookup"><span data-stu-id="51a8f-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51a8f-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51a8f-134">Request body</span></span>
<span data-ttu-id="51a8f-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51a8f-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51a8f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="51a8f-136">Response</span></span>
<span data-ttu-id="51a8f-137">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="51a8f-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="51a8f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51a8f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="51a8f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51a8f-139">Request</span></span>
<span data-ttu-id="51a8f-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51a8f-140">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="51a8f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="51a8f-141">Response</span></span>
<span data-ttu-id="51a8f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51a8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




