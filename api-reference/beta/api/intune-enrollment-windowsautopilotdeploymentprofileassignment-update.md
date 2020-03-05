---
title: Atualizar windowsAutopilotDeploymentProfileAssignment
description: Atualiza as propriedades de um objeto windowsAutopilotDeploymentProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b7d4d7e39d78fd76207a70c4792d282a9cf8f3c2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466350"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="d5368-103">Atualizar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="d5368-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

<span data-ttu-id="d5368-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d5368-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5368-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5368-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5368-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5368-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5368-107">Atualiza as propriedades de um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d5368-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5368-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5368-108">Prerequisites</span></span>
<span data-ttu-id="d5368-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5368-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5368-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5368-111">Permission type</span></span>|<span data-ttu-id="d5368-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5368-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5368-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5368-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5368-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5368-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d5368-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5368-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5368-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5368-116">Not supported.</span></span>|
|<span data-ttu-id="d5368-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5368-117">Application</span></span>|<span data-ttu-id="d5368-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5368-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5368-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5368-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d5368-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5368-120">Request headers</span></span>
|<span data-ttu-id="d5368-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5368-121">Header</span></span>|<span data-ttu-id="d5368-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d5368-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5368-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5368-123">Authorization</span></span>|<span data-ttu-id="d5368-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5368-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5368-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d5368-125">Accept</span></span>|<span data-ttu-id="d5368-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5368-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5368-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5368-127">Request body</span></span>
<span data-ttu-id="d5368-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d5368-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="d5368-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d5368-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="d5368-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5368-130">Property</span></span>|<span data-ttu-id="d5368-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5368-131">Type</span></span>|<span data-ttu-id="d5368-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5368-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5368-133">id</span><span class="sxs-lookup"><span data-stu-id="d5368-133">id</span></span>|<span data-ttu-id="d5368-134">String</span><span class="sxs-lookup"><span data-stu-id="d5368-134">String</span></span>|<span data-ttu-id="d5368-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="d5368-135">The key of the assignment.</span></span>|
|<span data-ttu-id="d5368-136">destino</span><span class="sxs-lookup"><span data-stu-id="d5368-136">target</span></span>|[<span data-ttu-id="d5368-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d5368-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d5368-138">O destino de atribuição para o perfil de implantação do piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="d5368-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="d5368-139">source</span><span class="sxs-lookup"><span data-stu-id="d5368-139">source</span></span>|[<span data-ttu-id="d5368-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="d5368-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="d5368-141">Tipo de recurso usado para implantação em um grupo, direto ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="d5368-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="d5368-142">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="d5368-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="d5368-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="d5368-143">sourceId</span></span>|<span data-ttu-id="d5368-144">String</span><span class="sxs-lookup"><span data-stu-id="d5368-144">String</span></span>|<span data-ttu-id="d5368-145">Identificador para o recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="d5368-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="d5368-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5368-146">Response</span></span>
<span data-ttu-id="d5368-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5368-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5368-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5368-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5368-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5368-149">Request</span></span>
<span data-ttu-id="d5368-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5368-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d5368-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5368-151">Response</span></span>
<span data-ttu-id="d5368-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5368-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





