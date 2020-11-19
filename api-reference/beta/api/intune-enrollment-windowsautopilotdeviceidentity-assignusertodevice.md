---
title: ação assignUserToDevice
description: Atribui um usuário aos dispositivos do AutoPilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b76fd48ccfca4403fbe9243de7ecaa0a4afca91
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228068"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="999f6-103">ação assignUserToDevice</span><span class="sxs-lookup"><span data-stu-id="999f6-103">assignUserToDevice action</span></span>

<span data-ttu-id="999f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="999f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="999f6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="999f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="999f6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="999f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="999f6-107">Atribui um usuário aos dispositivos do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="999f6-107">Assigns user to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="999f6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="999f6-108">Prerequisites</span></span>
<span data-ttu-id="999f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="999f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="999f6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="999f6-111">Permission type</span></span>|<span data-ttu-id="999f6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="999f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="999f6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="999f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="999f6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="999f6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="999f6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="999f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="999f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="999f6-116">Not supported.</span></span>|
|<span data-ttu-id="999f6-117">Application</span><span class="sxs-lookup"><span data-stu-id="999f6-117">Application</span></span>|<span data-ttu-id="999f6-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="999f6-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="999f6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="999f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="999f6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="999f6-120">Request headers</span></span>
|<span data-ttu-id="999f6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="999f6-121">Header</span></span>|<span data-ttu-id="999f6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="999f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="999f6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="999f6-123">Authorization</span></span>|<span data-ttu-id="999f6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="999f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="999f6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="999f6-125">Accept</span></span>|<span data-ttu-id="999f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="999f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="999f6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="999f6-127">Request body</span></span>
<span data-ttu-id="999f6-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="999f6-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="999f6-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="999f6-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="999f6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="999f6-130">Property</span></span>|<span data-ttu-id="999f6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="999f6-131">Type</span></span>|<span data-ttu-id="999f6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="999f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="999f6-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="999f6-133">userPrincipalName</span></span>|<span data-ttu-id="999f6-134">String</span><span class="sxs-lookup"><span data-stu-id="999f6-134">String</span></span>|<span data-ttu-id="999f6-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="999f6-135">Not yet documented</span></span>|
|<span data-ttu-id="999f6-136">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="999f6-136">addressableUserName</span></span>|<span data-ttu-id="999f6-137">String</span><span class="sxs-lookup"><span data-stu-id="999f6-137">String</span></span>|<span data-ttu-id="999f6-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="999f6-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="999f6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="999f6-139">Response</span></span>
<span data-ttu-id="999f6-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="999f6-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="999f6-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="999f6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="999f6-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="999f6-142">Request</span></span>
<span data-ttu-id="999f6-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="999f6-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="999f6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="999f6-144">Response</span></span>
<span data-ttu-id="999f6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="999f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




