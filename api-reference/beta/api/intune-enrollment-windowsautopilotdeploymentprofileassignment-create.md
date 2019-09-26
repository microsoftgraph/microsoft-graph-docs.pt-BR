---
title: Criar windowsAutopilotDeploymentProfileAssignment
description: Criar um novo objeto windowsAutopilotDeploymentProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bff01991a56b5a4fd6c63f591fb973c430987e98
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187734"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="90639-103">Criar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="90639-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="90639-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90639-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90639-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90639-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90639-106">Criar um novo objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="90639-106">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90639-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90639-107">Prerequisites</span></span>
<span data-ttu-id="90639-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90639-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90639-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90639-110">Permission type</span></span>|<span data-ttu-id="90639-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90639-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90639-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90639-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90639-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90639-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="90639-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90639-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90639-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90639-115">Not supported.</span></span>|
|<span data-ttu-id="90639-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90639-116">Application</span></span>|<span data-ttu-id="90639-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90639-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90639-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90639-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="90639-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90639-119">Request headers</span></span>
|<span data-ttu-id="90639-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90639-120">Header</span></span>|<span data-ttu-id="90639-121">Valor</span><span class="sxs-lookup"><span data-stu-id="90639-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90639-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90639-122">Authorization</span></span>|<span data-ttu-id="90639-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90639-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90639-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90639-124">Accept</span></span>|<span data-ttu-id="90639-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90639-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90639-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90639-126">Request body</span></span>
<span data-ttu-id="90639-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="90639-127">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="90639-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="90639-128">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="90639-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90639-129">Property</span></span>|<span data-ttu-id="90639-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="90639-130">Type</span></span>|<span data-ttu-id="90639-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="90639-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90639-132">id</span><span class="sxs-lookup"><span data-stu-id="90639-132">id</span></span>|<span data-ttu-id="90639-133">String</span><span class="sxs-lookup"><span data-stu-id="90639-133">String</span></span>|<span data-ttu-id="90639-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="90639-134">The key of the assignment.</span></span>|
|<span data-ttu-id="90639-135">destino</span><span class="sxs-lookup"><span data-stu-id="90639-135">target</span></span>|[<span data-ttu-id="90639-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="90639-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="90639-137">O destino de atribuição para o perfil de implantação do piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="90639-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="90639-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="90639-138">Response</span></span>
<span data-ttu-id="90639-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90639-139">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90639-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90639-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="90639-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90639-141">Request</span></span>
<span data-ttu-id="90639-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90639-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="90639-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="90639-143">Response</span></span>
<span data-ttu-id="90639-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90639-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




