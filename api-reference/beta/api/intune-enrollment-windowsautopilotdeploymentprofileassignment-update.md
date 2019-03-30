---
title: Atualizar windowsAutopilotDeploymentProfileAssignment
description: Atualiza as propriedades de um objeto windowsAutopilotDeploymentProfileAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32a8be36d4c426a316dc5dc86df76276b2bb6981
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986443"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="b1828-103">Atualizar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="b1828-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="b1828-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1828-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1828-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1828-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1828-106">Atualiza as propriedades de um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b1828-106">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1828-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1828-107">Prerequisites</span></span>
<span data-ttu-id="b1828-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1828-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1828-110">Permission type</span></span>|<span data-ttu-id="b1828-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b1828-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1828-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1828-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1828-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1828-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b1828-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1828-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1828-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1828-115">Not supported.</span></span>|
|<span data-ttu-id="b1828-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1828-116">Application</span></span>|<span data-ttu-id="b1828-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1828-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1828-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1828-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b1828-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1828-119">Request headers</span></span>
|<span data-ttu-id="b1828-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1828-120">Header</span></span>|<span data-ttu-id="b1828-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b1828-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1828-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1828-122">Authorization</span></span>|<span data-ttu-id="b1828-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1828-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1828-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1828-124">Accept</span></span>|<span data-ttu-id="b1828-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1828-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1828-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1828-126">Request body</span></span>
<span data-ttu-id="b1828-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b1828-127">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="b1828-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b1828-128">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="b1828-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1828-129">Property</span></span>|<span data-ttu-id="b1828-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1828-130">Type</span></span>|<span data-ttu-id="b1828-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1828-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1828-132">id</span><span class="sxs-lookup"><span data-stu-id="b1828-132">id</span></span>|<span data-ttu-id="b1828-133">String</span><span class="sxs-lookup"><span data-stu-id="b1828-133">String</span></span>|<span data-ttu-id="b1828-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="b1828-134">The key of the assignment.</span></span>|
|<span data-ttu-id="b1828-135">destino</span><span class="sxs-lookup"><span data-stu-id="b1828-135">target</span></span>|[<span data-ttu-id="b1828-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b1828-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b1828-137">O destino de atribuição para o perfil de implantação do piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="b1828-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="b1828-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1828-138">Response</span></span>
<span data-ttu-id="b1828-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1828-139">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1828-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1828-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1828-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1828-141">Request</span></span>
<span data-ttu-id="b1828-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1828-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b1828-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1828-143">Response</span></span>
<span data-ttu-id="b1828-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1828-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




