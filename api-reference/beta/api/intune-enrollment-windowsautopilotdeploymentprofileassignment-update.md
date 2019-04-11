---
title: Atualizar windowsAutopilotDeploymentProfileAssignment
description: Atualiza as propriedades de um objeto windowsAutopilotDeploymentProfileAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 562ae8b137754acc3475ba98fb335a4f7e7310dd
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783399"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="6e120-103">Atualizar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="6e120-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="6e120-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e120-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e120-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e120-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e120-106">Atualiza as propriedades de um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6e120-106">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e120-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e120-107">Prerequisites</span></span>
<span data-ttu-id="6e120-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e120-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e120-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e120-110">Permission type</span></span>|<span data-ttu-id="6e120-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e120-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e120-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e120-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e120-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e120-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6e120-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e120-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e120-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e120-115">Not supported.</span></span>|
|<span data-ttu-id="6e120-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e120-116">Application</span></span>|<span data-ttu-id="6e120-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e120-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e120-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e120-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6e120-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e120-119">Request headers</span></span>
|<span data-ttu-id="6e120-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e120-120">Header</span></span>|<span data-ttu-id="6e120-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6e120-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e120-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e120-122">Authorization</span></span>|<span data-ttu-id="6e120-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e120-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e120-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e120-124">Accept</span></span>|<span data-ttu-id="6e120-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6e120-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e120-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e120-126">Request body</span></span>
<span data-ttu-id="6e120-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6e120-127">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="6e120-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6e120-128">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="6e120-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e120-129">Property</span></span>|<span data-ttu-id="6e120-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e120-130">Type</span></span>|<span data-ttu-id="6e120-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e120-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e120-132">id</span><span class="sxs-lookup"><span data-stu-id="6e120-132">id</span></span>|<span data-ttu-id="6e120-133">String</span><span class="sxs-lookup"><span data-stu-id="6e120-133">String</span></span>|<span data-ttu-id="6e120-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="6e120-134">The key of the assignment.</span></span>|
|<span data-ttu-id="6e120-135">destino</span><span class="sxs-lookup"><span data-stu-id="6e120-135">target</span></span>|[<span data-ttu-id="6e120-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6e120-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6e120-137">O destino de atribuição para o perfil de implantação do piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="6e120-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="6e120-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e120-138">Response</span></span>
<span data-ttu-id="6e120-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e120-139">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e120-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e120-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e120-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e120-141">Request</span></span>
<span data-ttu-id="6e120-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e120-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6e120-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e120-143">Response</span></span>
<span data-ttu-id="6e120-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e120-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





