---
title: Ação deleteUserFromSharedAppleDevice
description: Excluir o usuário do dispositivo compartilhado da Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c074bddbf3c249cf9effc39b4db04c0e773ffd94
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140002"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="67b3f-103">Ação deleteUserFromSharedAppleDevice</span><span class="sxs-lookup"><span data-stu-id="67b3f-103">deleteUserFromSharedAppleDevice action</span></span>

> <span data-ttu-id="67b3f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67b3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67b3f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67b3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67b3f-106">Excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="67b3f-106">Delete user from shared Apple device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67b3f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67b3f-107">Prerequisites</span></span>
<span data-ttu-id="67b3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="67b3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="67b3f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67b3f-110">Permission type</span></span>|<span data-ttu-id="67b3f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67b3f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67b3f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67b3f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67b3f-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="67b3f-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="67b3f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67b3f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67b3f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67b3f-115">Not supported.</span></span>|
|<span data-ttu-id="67b3f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67b3f-116">Application</span></span>|<span data-ttu-id="67b3f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67b3f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67b3f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67b3f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="67b3f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67b3f-119">Request headers</span></span>
|<span data-ttu-id="67b3f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67b3f-120">Header</span></span>|<span data-ttu-id="67b3f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="67b3f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67b3f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="67b3f-122">Authorization</span></span>|<span data-ttu-id="67b3f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67b3f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67b3f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67b3f-124">Accept</span></span>|<span data-ttu-id="67b3f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67b3f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67b3f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67b3f-126">Request body</span></span>
<span data-ttu-id="67b3f-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="67b3f-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="67b3f-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="67b3f-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="67b3f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67b3f-129">Property</span></span>|<span data-ttu-id="67b3f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="67b3f-130">Type</span></span>|<span data-ttu-id="67b3f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="67b3f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67b3f-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="67b3f-132">userPrincipalName</span></span>|<span data-ttu-id="67b3f-133">String</span><span class="sxs-lookup"><span data-stu-id="67b3f-133">String</span></span>|<span data-ttu-id="67b3f-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="67b3f-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="67b3f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="67b3f-135">Response</span></span>
<span data-ttu-id="67b3f-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="67b3f-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="67b3f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67b3f-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="67b3f-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67b3f-138">Request</span></span>
<span data-ttu-id="67b3f-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67b3f-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="67b3f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="67b3f-140">Response</span></span>
<span data-ttu-id="67b3f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67b3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




