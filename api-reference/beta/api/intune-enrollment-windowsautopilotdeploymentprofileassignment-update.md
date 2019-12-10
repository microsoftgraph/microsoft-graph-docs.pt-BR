---
title: Atualizar windowsAutopilotDeploymentProfileAssignment
description: Atualiza as propriedades de um objeto windowsAutopilotDeploymentProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f52c4e5f9bdc20ca37920b33d818f46ff711f9d8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943723"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="d25e2-103">Atualizar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="d25e2-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="d25e2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d25e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d25e2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d25e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d25e2-106">Atualiza as propriedades de um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d25e2-106">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d25e2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d25e2-107">Prerequisites</span></span>
<span data-ttu-id="d25e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d25e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d25e2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d25e2-110">Permission type</span></span>|<span data-ttu-id="d25e2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d25e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d25e2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d25e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d25e2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25e2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d25e2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d25e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d25e2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d25e2-115">Not supported.</span></span>|
|<span data-ttu-id="d25e2-116">Application</span><span class="sxs-lookup"><span data-stu-id="d25e2-116">Application</span></span>|<span data-ttu-id="d25e2-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25e2-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d25e2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d25e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d25e2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d25e2-119">Request headers</span></span>
|<span data-ttu-id="d25e2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d25e2-120">Header</span></span>|<span data-ttu-id="d25e2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d25e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d25e2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d25e2-122">Authorization</span></span>|<span data-ttu-id="d25e2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d25e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d25e2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d25e2-124">Accept</span></span>|<span data-ttu-id="d25e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d25e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d25e2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d25e2-126">Request body</span></span>
<span data-ttu-id="d25e2-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d25e2-127">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="d25e2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d25e2-128">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="d25e2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d25e2-129">Property</span></span>|<span data-ttu-id="d25e2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d25e2-130">Type</span></span>|<span data-ttu-id="d25e2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d25e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d25e2-132">id</span><span class="sxs-lookup"><span data-stu-id="d25e2-132">id</span></span>|<span data-ttu-id="d25e2-133">String</span><span class="sxs-lookup"><span data-stu-id="d25e2-133">String</span></span>|<span data-ttu-id="d25e2-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="d25e2-134">The key of the assignment.</span></span>|
|<span data-ttu-id="d25e2-135">destino</span><span class="sxs-lookup"><span data-stu-id="d25e2-135">target</span></span>|[<span data-ttu-id="d25e2-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d25e2-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d25e2-137">O destino de atribuição para o perfil de implantação do piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="d25e2-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="d25e2-138">source</span><span class="sxs-lookup"><span data-stu-id="d25e2-138">source</span></span>|[<span data-ttu-id="d25e2-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="d25e2-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="d25e2-140">Tipo de recurso usado para implantação em um grupo, direto ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="d25e2-140">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="d25e2-141">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="d25e2-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="d25e2-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="d25e2-142">sourceId</span></span>|<span data-ttu-id="d25e2-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d25e2-143">String</span></span>|<span data-ttu-id="d25e2-144">Identificador para o recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="d25e2-144">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="d25e2-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d25e2-145">Response</span></span>
<span data-ttu-id="d25e2-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d25e2-146">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d25e2-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d25e2-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d25e2-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d25e2-148">Request</span></span>
<span data-ttu-id="d25e2-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d25e2-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d25e2-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d25e2-150">Response</span></span>
<span data-ttu-id="d25e2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d25e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





