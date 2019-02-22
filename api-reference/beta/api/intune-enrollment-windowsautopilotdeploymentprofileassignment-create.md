---
title: Criar windowsAutopilotDeploymentProfileAssignment
description: Criar um novo objeto windowsAutopilotDeploymentProfileAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30a6b1b64c4c434dfe364a49c6bf6fe080880a90
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175070"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="fa3d9-103">Criar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="fa3d9-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="fa3d9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fa3d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa3d9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa3d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa3d9-106">Criar um novo objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fa3d9-106">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa3d9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa3d9-107">Prerequisites</span></span>
<span data-ttu-id="fa3d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa3d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fa3d9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa3d9-110">Permission type</span></span>|<span data-ttu-id="fa3d9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fa3d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa3d9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa3d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa3d9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa3d9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fa3d9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa3d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa3d9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa3d9-115">Not supported.</span></span>|
|<span data-ttu-id="fa3d9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa3d9-116">Application</span></span>|<span data-ttu-id="fa3d9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa3d9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa3d9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa3d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="fa3d9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa3d9-119">Request headers</span></span>
|<span data-ttu-id="fa3d9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa3d9-120">Header</span></span>|<span data-ttu-id="fa3d9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fa3d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa3d9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa3d9-122">Authorization</span></span>|<span data-ttu-id="fa3d9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa3d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa3d9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fa3d9-124">Accept</span></span>|<span data-ttu-id="fa3d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa3d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa3d9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa3d9-126">Request body</span></span>
<span data-ttu-id="fa3d9-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="fa3d9-127">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="fa3d9-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="fa3d9-128">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="fa3d9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa3d9-129">Property</span></span>|<span data-ttu-id="fa3d9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa3d9-130">Type</span></span>|<span data-ttu-id="fa3d9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa3d9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa3d9-132">id</span><span class="sxs-lookup"><span data-stu-id="fa3d9-132">id</span></span>|<span data-ttu-id="fa3d9-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa3d9-133">String</span></span>|<span data-ttu-id="fa3d9-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="fa3d9-134">The key of the assignment.</span></span>|
|<span data-ttu-id="fa3d9-135">destino</span><span class="sxs-lookup"><span data-stu-id="fa3d9-135">target</span></span>|[<span data-ttu-id="fa3d9-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fa3d9-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fa3d9-137">O destino de atribuição para o perfil de implantação do piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="fa3d9-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="fa3d9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa3d9-138">Response</span></span>
<span data-ttu-id="fa3d9-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa3d9-139">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa3d9-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa3d9-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa3d9-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa3d9-141">Request</span></span>
<span data-ttu-id="fa3d9-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa3d9-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fa3d9-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa3d9-143">Response</span></span>
<span data-ttu-id="fa3d9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa3d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




