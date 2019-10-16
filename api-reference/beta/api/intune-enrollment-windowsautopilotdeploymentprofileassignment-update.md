---
title: Atualizar windowsAutopilotDeploymentProfileAssignment
description: Atualiza as propriedades de um objeto windowsAutopilotDeploymentProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8e2311f8a8828c81ad471280f40d4bb22e78d480
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535832"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="b0a15-103">Atualizar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="b0a15-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="b0a15-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0a15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0a15-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0a15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0a15-106">Atualiza as propriedades de um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b0a15-106">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0a15-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0a15-107">Prerequisites</span></span>
<span data-ttu-id="b0a15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0a15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0a15-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0a15-110">Permission type</span></span>|<span data-ttu-id="b0a15-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0a15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0a15-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0a15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0a15-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0a15-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b0a15-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0a15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0a15-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0a15-115">Not supported.</span></span>|
|<span data-ttu-id="b0a15-116">Application</span><span class="sxs-lookup"><span data-stu-id="b0a15-116">Application</span></span>|<span data-ttu-id="b0a15-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0a15-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0a15-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0a15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b0a15-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0a15-119">Request headers</span></span>
|<span data-ttu-id="b0a15-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0a15-120">Header</span></span>|<span data-ttu-id="b0a15-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b0a15-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0a15-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0a15-122">Authorization</span></span>|<span data-ttu-id="b0a15-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0a15-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0a15-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0a15-124">Accept</span></span>|<span data-ttu-id="b0a15-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0a15-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0a15-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0a15-126">Request body</span></span>
<span data-ttu-id="b0a15-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b0a15-127">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="b0a15-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b0a15-128">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="b0a15-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0a15-129">Property</span></span>|<span data-ttu-id="b0a15-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0a15-130">Type</span></span>|<span data-ttu-id="b0a15-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0a15-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0a15-132">id</span><span class="sxs-lookup"><span data-stu-id="b0a15-132">id</span></span>|<span data-ttu-id="b0a15-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0a15-133">String</span></span>|<span data-ttu-id="b0a15-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="b0a15-134">The key of the assignment.</span></span>|
|<span data-ttu-id="b0a15-135">destino</span><span class="sxs-lookup"><span data-stu-id="b0a15-135">target</span></span>|[<span data-ttu-id="b0a15-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b0a15-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b0a15-137">O destino de atribuição para o perfil de implantação do piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="b0a15-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="b0a15-138">source</span><span class="sxs-lookup"><span data-stu-id="b0a15-138">source</span></span>|[<span data-ttu-id="b0a15-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="b0a15-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="b0a15-140">Tipo de recurso usado para implantação em um grupo, direto ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="b0a15-140">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="b0a15-141">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="b0a15-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="b0a15-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="b0a15-142">sourceId</span></span>|<span data-ttu-id="b0a15-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0a15-143">String</span></span>|<span data-ttu-id="b0a15-144">Identificador para o recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="b0a15-144">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="b0a15-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0a15-145">Response</span></span>
<span data-ttu-id="b0a15-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0a15-146">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0a15-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0a15-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0a15-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0a15-148">Request</span></span>
<span data-ttu-id="b0a15-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0a15-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="b0a15-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0a15-150">Response</span></span>
<span data-ttu-id="b0a15-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0a15-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```






