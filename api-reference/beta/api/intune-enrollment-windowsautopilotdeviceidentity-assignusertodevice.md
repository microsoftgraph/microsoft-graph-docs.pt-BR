---
title: ação assignUserToDevice
description: Atribui um usuário aos dispositivos do AutoPilot.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60e21b15d239c3485bf1e09880a188ed80d4de84
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452420"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="019fe-103">ação assignUserToDevice</span><span class="sxs-lookup"><span data-stu-id="019fe-103">assignUserToDevice action</span></span>

<span data-ttu-id="019fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="019fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="019fe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="019fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="019fe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="019fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="019fe-107">Atribui um usuário aos dispositivos do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="019fe-107">Assigns user to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="019fe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="019fe-108">Prerequisites</span></span>
<span data-ttu-id="019fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="019fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="019fe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="019fe-111">Permission type</span></span>|<span data-ttu-id="019fe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="019fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="019fe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="019fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="019fe-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="019fe-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="019fe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="019fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="019fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="019fe-116">Not supported.</span></span>|
|<span data-ttu-id="019fe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="019fe-117">Application</span></span>|<span data-ttu-id="019fe-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="019fe-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="019fe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="019fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="019fe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="019fe-120">Request headers</span></span>
|<span data-ttu-id="019fe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="019fe-121">Header</span></span>|<span data-ttu-id="019fe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="019fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="019fe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="019fe-123">Authorization</span></span>|<span data-ttu-id="019fe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="019fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="019fe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="019fe-125">Accept</span></span>|<span data-ttu-id="019fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="019fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="019fe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="019fe-127">Request body</span></span>
<span data-ttu-id="019fe-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="019fe-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="019fe-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="019fe-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="019fe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="019fe-130">Property</span></span>|<span data-ttu-id="019fe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="019fe-131">Type</span></span>|<span data-ttu-id="019fe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="019fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="019fe-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="019fe-133">userPrincipalName</span></span>|<span data-ttu-id="019fe-134">String</span><span class="sxs-lookup"><span data-stu-id="019fe-134">String</span></span>|<span data-ttu-id="019fe-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="019fe-135">Not yet documented</span></span>|
|<span data-ttu-id="019fe-136">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="019fe-136">addressableUserName</span></span>|<span data-ttu-id="019fe-137">String</span><span class="sxs-lookup"><span data-stu-id="019fe-137">String</span></span>|<span data-ttu-id="019fe-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="019fe-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="019fe-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="019fe-139">Response</span></span>
<span data-ttu-id="019fe-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="019fe-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="019fe-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="019fe-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="019fe-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="019fe-142">Request</span></span>
<span data-ttu-id="019fe-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="019fe-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="019fe-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="019fe-144">Response</span></span>
<span data-ttu-id="019fe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="019fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



