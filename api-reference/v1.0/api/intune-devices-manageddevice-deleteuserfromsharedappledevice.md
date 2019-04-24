---
title: Ação deleteUserFromSharedAppleDevice
description: Excluir o usuário do dispositivo compartilhado da Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1602253d7b22c36b71056035491d0b18c35cd3a8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584779"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="1655d-103">Ação deleteUserFromSharedAppleDevice</span><span class="sxs-lookup"><span data-stu-id="1655d-103">deleteUserFromSharedAppleDevice action</span></span>

> <span data-ttu-id="1655d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1655d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1655d-105">Excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="1655d-105">Delete user from shared Apple device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1655d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1655d-106">Prerequisites</span></span>
<span data-ttu-id="1655d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1655d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1655d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1655d-109">Permission type</span></span>|<span data-ttu-id="1655d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1655d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1655d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1655d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1655d-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="1655d-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="1655d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1655d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1655d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1655d-114">Not supported.</span></span>|
|<span data-ttu-id="1655d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1655d-115">Application</span></span>|<span data-ttu-id="1655d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1655d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1655d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1655d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="1655d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1655d-118">Request headers</span></span>
|<span data-ttu-id="1655d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1655d-119">Header</span></span>|<span data-ttu-id="1655d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1655d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1655d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1655d-121">Authorization</span></span>|<span data-ttu-id="1655d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1655d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1655d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1655d-123">Accept</span></span>|<span data-ttu-id="1655d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1655d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1655d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1655d-125">Request body</span></span>
<span data-ttu-id="1655d-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1655d-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1655d-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1655d-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1655d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1655d-128">Property</span></span>|<span data-ttu-id="1655d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1655d-129">Type</span></span>|<span data-ttu-id="1655d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1655d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1655d-131">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1655d-131">userPrincipalName</span></span>|<span data-ttu-id="1655d-132">String</span><span class="sxs-lookup"><span data-stu-id="1655d-132">String</span></span>|<span data-ttu-id="1655d-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1655d-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1655d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1655d-134">Response</span></span>
<span data-ttu-id="1655d-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1655d-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1655d-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1655d-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="1655d-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1655d-137">Request</span></span>
<span data-ttu-id="1655d-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1655d-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="1655d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1655d-139">Response</span></span>
<span data-ttu-id="1655d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1655d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



