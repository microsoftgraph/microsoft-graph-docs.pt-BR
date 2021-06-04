---
title: Excluir usuário
description: Exclui usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f516c1386d828412e71fa35668b4c86a496f6af
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732246"
---
# <a name="delete-user"></a><span data-ttu-id="c4d54-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="c4d54-103">Delete user</span></span>

<span data-ttu-id="c4d54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4d54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4d54-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4d54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4d54-106">Exclui [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="c4d54-106">Deletes a [user](../resources/intune-shared-user.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4d54-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4d54-107">Prerequisites</span></span>
<span data-ttu-id="c4d54-108">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c4d54-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c4d54-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4d54-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="c4d54-110">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="c4d54-110">The specific permission required depends on context.</span></span>

|<span data-ttu-id="c4d54-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4d54-111">Permission type</span></span>|<span data-ttu-id="c4d54-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4d54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4d54-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4d54-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c4d54-114">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="c4d54-114">_varies by context_</span></span>|
| <span data-ttu-id="c4d54-115">&nbsp;&nbsp;Dispositivos</span><span class="sxs-lookup"><span data-stu-id="c4d54-115">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="c4d54-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4d54-116">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c4d54-117">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="c4d54-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="c4d54-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4d54-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="c4d54-119">&nbsp;&nbsp;Integração</span><span class="sxs-lookup"><span data-stu-id="c4d54-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="c4d54-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4d54-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c4d54-121">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="c4d54-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="c4d54-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4d54-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="c4d54-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4d54-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4d54-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4d54-124">Not supported.</span></span>|
|<span data-ttu-id="c4d54-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4d54-125">Application</span></span>|<span data-ttu-id="c4d54-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4d54-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4d54-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4d54-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="c4d54-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4d54-128">Request headers</span></span>
|<span data-ttu-id="c4d54-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4d54-129">Header</span></span>|<span data-ttu-id="c4d54-130">Valor</span><span class="sxs-lookup"><span data-stu-id="c4d54-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4d54-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4d54-131">Authorization</span></span>|<span data-ttu-id="c4d54-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4d54-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4d54-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4d54-133">Accept</span></span>|<span data-ttu-id="c4d54-134">application/json</span><span class="sxs-lookup"><span data-stu-id="c4d54-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4d54-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4d54-135">Request body</span></span>
<span data-ttu-id="c4d54-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4d54-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4d54-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4d54-137">Response</span></span>
<span data-ttu-id="c4d54-138">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c4d54-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c4d54-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4d54-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4d54-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4d54-140">Request</span></span>
<span data-ttu-id="c4d54-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4d54-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="c4d54-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4d54-142">Response</span></span>
<span data-ttu-id="c4d54-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4d54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









