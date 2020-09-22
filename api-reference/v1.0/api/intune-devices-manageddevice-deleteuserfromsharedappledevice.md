---
title: Ação deleteUserFromSharedAppleDevice
description: Excluir o usuário do dispositivo compartilhado da Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b3d67c83a5593d05fcb1ec47ac829d02c3697e5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009489"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="d3902-103">Ação deleteUserFromSharedAppleDevice</span><span class="sxs-lookup"><span data-stu-id="d3902-103">deleteUserFromSharedAppleDevice action</span></span>

<span data-ttu-id="d3902-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3902-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3902-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3902-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3902-106">Excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="d3902-106">Delete user from shared Apple device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3902-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3902-107">Prerequisites</span></span>
<span data-ttu-id="d3902-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3902-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3902-110">Permission type</span></span>|<span data-ttu-id="d3902-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3902-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3902-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3902-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3902-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="d3902-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="d3902-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3902-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3902-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3902-115">Not supported.</span></span>|
|<span data-ttu-id="d3902-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3902-116">Application</span></span>|<span data-ttu-id="d3902-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3902-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3902-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3902-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="d3902-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3902-119">Request headers</span></span>
|<span data-ttu-id="d3902-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3902-120">Header</span></span>|<span data-ttu-id="d3902-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d3902-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3902-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3902-122">Authorization</span></span>|<span data-ttu-id="d3902-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3902-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3902-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3902-124">Accept</span></span>|<span data-ttu-id="d3902-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3902-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3902-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3902-126">Request body</span></span>
<span data-ttu-id="d3902-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d3902-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d3902-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d3902-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d3902-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3902-129">Property</span></span>|<span data-ttu-id="d3902-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3902-130">Type</span></span>|<span data-ttu-id="d3902-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3902-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3902-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d3902-132">userPrincipalName</span></span>|<span data-ttu-id="d3902-133">String</span><span class="sxs-lookup"><span data-stu-id="d3902-133">String</span></span>|<span data-ttu-id="d3902-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d3902-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d3902-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3902-135">Response</span></span>
<span data-ttu-id="d3902-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d3902-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d3902-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3902-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3902-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3902-138">Request</span></span>
<span data-ttu-id="d3902-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3902-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="d3902-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3902-140">Response</span></span>
<span data-ttu-id="d3902-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3902-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









