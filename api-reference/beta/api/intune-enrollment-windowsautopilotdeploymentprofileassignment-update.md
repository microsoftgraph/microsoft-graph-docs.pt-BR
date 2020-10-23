---
title: Atualizar windowsAutopilotDeploymentProfileAssignment
description: Atualiza as propriedades de um objeto windowsAutopilotDeploymentProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e2032fafebe1bbb56cacc6eeeba060b737b8316e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735439"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="63348-103">Atualizar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="63348-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

<span data-ttu-id="63348-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63348-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63348-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63348-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63348-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63348-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63348-107">Atualiza as propriedades de um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="63348-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63348-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63348-108">Prerequisites</span></span>
<span data-ttu-id="63348-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63348-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63348-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63348-111">Permission type</span></span>|<span data-ttu-id="63348-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63348-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63348-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63348-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63348-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63348-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="63348-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63348-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63348-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63348-116">Not supported.</span></span>|
|<span data-ttu-id="63348-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63348-117">Application</span></span>|<span data-ttu-id="63348-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63348-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63348-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63348-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="63348-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63348-120">Request headers</span></span>
|<span data-ttu-id="63348-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63348-121">Header</span></span>|<span data-ttu-id="63348-122">Valor</span><span class="sxs-lookup"><span data-stu-id="63348-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63348-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="63348-123">Authorization</span></span>|<span data-ttu-id="63348-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63348-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63348-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63348-125">Accept</span></span>|<span data-ttu-id="63348-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63348-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63348-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63348-127">Request body</span></span>
<span data-ttu-id="63348-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="63348-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="63348-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="63348-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="63348-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63348-130">Property</span></span>|<span data-ttu-id="63348-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="63348-131">Type</span></span>|<span data-ttu-id="63348-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="63348-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63348-133">id</span><span class="sxs-lookup"><span data-stu-id="63348-133">id</span></span>|<span data-ttu-id="63348-134">String</span><span class="sxs-lookup"><span data-stu-id="63348-134">String</span></span>|<span data-ttu-id="63348-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="63348-135">The key of the assignment.</span></span>|
|<span data-ttu-id="63348-136">destino</span><span class="sxs-lookup"><span data-stu-id="63348-136">target</span></span>|[<span data-ttu-id="63348-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="63348-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="63348-138">O destino de atribuição para o perfil de implantação do piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="63348-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="63348-139">source</span><span class="sxs-lookup"><span data-stu-id="63348-139">source</span></span>|[<span data-ttu-id="63348-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="63348-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="63348-141">Tipo de recurso usado para implantação em um grupo, direto ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="63348-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="63348-142">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="63348-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="63348-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="63348-143">sourceId</span></span>|<span data-ttu-id="63348-144">String</span><span class="sxs-lookup"><span data-stu-id="63348-144">String</span></span>|<span data-ttu-id="63348-145">Identificador para o recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="63348-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="63348-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="63348-146">Response</span></span>
<span data-ttu-id="63348-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63348-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63348-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63348-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="63348-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63348-149">Request</span></span>
<span data-ttu-id="63348-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63348-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 411

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="63348-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="63348-151">Response</span></span>
<span data-ttu-id="63348-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63348-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 460

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```





