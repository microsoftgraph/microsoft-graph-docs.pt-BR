---
title: Ação deleteUserFromSharedAppleDevice
description: Excluir o usuário do dispositivo compartilhado da Apple
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1276351b8d0624bf8c54198f5e5d5b839a0e7406
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792314"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="dc10e-103">Ação deleteUserFromSharedAppleDevice</span><span class="sxs-lookup"><span data-stu-id="dc10e-103">deleteUserFromSharedAppleDevice action</span></span>

<span data-ttu-id="dc10e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc10e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc10e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc10e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc10e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc10e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc10e-107">Excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="dc10e-107">Delete user from shared Apple device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc10e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc10e-108">Prerequisites</span></span>
<span data-ttu-id="dc10e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="dc10e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="dc10e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc10e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc10e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc10e-111">Permission type</span></span>|<span data-ttu-id="dc10e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc10e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc10e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc10e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc10e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="dc10e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="dc10e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc10e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc10e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc10e-116">Not supported.</span></span>|
|<span data-ttu-id="dc10e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc10e-117">Application</span></span>|<span data-ttu-id="dc10e-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="dc10e-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc10e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc10e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/comanagedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="dc10e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc10e-120">Request headers</span></span>
|<span data-ttu-id="dc10e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc10e-121">Header</span></span>|<span data-ttu-id="dc10e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dc10e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc10e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc10e-123">Authorization</span></span>|<span data-ttu-id="dc10e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc10e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc10e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc10e-125">Accept</span></span>|<span data-ttu-id="dc10e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc10e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc10e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc10e-127">Request body</span></span>
<span data-ttu-id="dc10e-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="dc10e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dc10e-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="dc10e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dc10e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc10e-130">Property</span></span>|<span data-ttu-id="dc10e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc10e-131">Type</span></span>|<span data-ttu-id="dc10e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc10e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc10e-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dc10e-133">userPrincipalName</span></span>|<span data-ttu-id="dc10e-134">String</span><span class="sxs-lookup"><span data-stu-id="dc10e-134">String</span></span>|<span data-ttu-id="dc10e-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dc10e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dc10e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc10e-136">Response</span></span>
<span data-ttu-id="dc10e-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc10e-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc10e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc10e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc10e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc10e-139">Request</span></span>
<span data-ttu-id="dc10e-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc10e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="dc10e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc10e-141">Response</span></span>
<span data-ttu-id="dc10e-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="dc10e-142">Here is an example of the response.</span></span> <span data-ttu-id="dc10e-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="dc10e-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dc10e-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="dc10e-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



