---
title: Ação deleteUserFromSharedAppleDevice
description: Excluir o usuário do dispositivo compartilhado da Apple
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7e8c2fad909c6caf58d294d7a9426878882fdfcc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985830"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="0a3a2-103">Ação deleteUserFromSharedAppleDevice</span><span class="sxs-lookup"><span data-stu-id="0a3a2-103">deleteUserFromSharedAppleDevice action</span></span>

> <span data-ttu-id="0a3a2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0a3a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a3a2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a3a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a3a2-106">Excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="0a3a2-106">Delete user from shared Apple device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a3a2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a3a2-107">Prerequisites</span></span>
<span data-ttu-id="0a3a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a3a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a3a2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a3a2-110">Permission type</span></span>|<span data-ttu-id="0a3a2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a3a2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a3a2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a3a2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a3a2-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="0a3a2-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="0a3a2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a3a2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a3a2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a3a2-115">Not supported.</span></span>|
|<span data-ttu-id="0a3a2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a3a2-116">Application</span></span>|<span data-ttu-id="0a3a2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a3a2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a3a2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a3a2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="0a3a2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a3a2-119">Request headers</span></span>
|<span data-ttu-id="0a3a2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a3a2-120">Header</span></span>|<span data-ttu-id="0a3a2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0a3a2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a3a2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a3a2-122">Authorization</span></span>|<span data-ttu-id="0a3a2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a3a2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a3a2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a3a2-124">Accept</span></span>|<span data-ttu-id="0a3a2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a3a2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a3a2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a3a2-126">Request body</span></span>
<span data-ttu-id="0a3a2-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0a3a2-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0a3a2-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0a3a2-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0a3a2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a3a2-129">Property</span></span>|<span data-ttu-id="0a3a2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a3a2-130">Type</span></span>|<span data-ttu-id="0a3a2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a3a2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a3a2-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0a3a2-132">userPrincipalName</span></span>|<span data-ttu-id="0a3a2-133">String</span><span class="sxs-lookup"><span data-stu-id="0a3a2-133">String</span></span>|<span data-ttu-id="0a3a2-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0a3a2-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0a3a2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a3a2-135">Response</span></span>
<span data-ttu-id="0a3a2-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0a3a2-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0a3a2-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a3a2-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a3a2-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a3a2-138">Request</span></span>
<span data-ttu-id="0a3a2-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a3a2-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="0a3a2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a3a2-140">Response</span></span>
<span data-ttu-id="0a3a2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a3a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





