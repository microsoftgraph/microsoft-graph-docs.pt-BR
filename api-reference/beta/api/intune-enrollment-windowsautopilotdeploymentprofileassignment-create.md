---
title: Criar windowsAutopilotDeploymentProfileAssignment
description: Crie um novo objeto windowsAutopilotDeploymentProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00aff52af62241bc0782ed7e3d6c87eee57f9cfd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159015"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="2a2bd-103">Criar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="2a2bd-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

<span data-ttu-id="2a2bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a2bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a2bd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a2bd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a2bd-107">Crie um novo [objeto windowsAutopilotDeploymentProfileAssignment.](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2a2bd-107">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a2bd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a2bd-108">Prerequisites</span></span>
<span data-ttu-id="2a2bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a2bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a2bd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a2bd-111">Permission type</span></span>|<span data-ttu-id="2a2bd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a2bd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a2bd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a2bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a2bd-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a2bd-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a2bd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a2bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a2bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-116">Not supported.</span></span>|
|<span data-ttu-id="2a2bd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a2bd-117">Application</span></span>|<span data-ttu-id="2a2bd-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a2bd-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a2bd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a2bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2a2bd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a2bd-120">Request headers</span></span>
|<span data-ttu-id="2a2bd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a2bd-121">Header</span></span>|<span data-ttu-id="2a2bd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2a2bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a2bd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a2bd-123">Authorization</span></span>|<span data-ttu-id="2a2bd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a2bd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a2bd-125">Accept</span></span>|<span data-ttu-id="2a2bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a2bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a2bd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a2bd-127">Request body</span></span>
<span data-ttu-id="2a2bd-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-128">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="2a2bd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-129">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="2a2bd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a2bd-130">Property</span></span>|<span data-ttu-id="2a2bd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a2bd-131">Type</span></span>|<span data-ttu-id="2a2bd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a2bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a2bd-133">id</span><span class="sxs-lookup"><span data-stu-id="2a2bd-133">id</span></span>|<span data-ttu-id="2a2bd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a2bd-134">String</span></span>|<span data-ttu-id="2a2bd-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-135">The key of the assignment.</span></span>|
|<span data-ttu-id="2a2bd-136">destino</span><span class="sxs-lookup"><span data-stu-id="2a2bd-136">target</span></span>|[<span data-ttu-id="2a2bd-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2a2bd-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2a2bd-138">O destino de atribuição para o perfil de implantação do Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="2a2bd-139">source</span><span class="sxs-lookup"><span data-stu-id="2a2bd-139">source</span></span>|[<span data-ttu-id="2a2bd-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="2a2bd-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="2a2bd-141">Tipo de recurso usado para implantação para um grupo, direto ou pacote/policySet.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="2a2bd-142">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="2a2bd-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="2a2bd-143">sourceId</span></span>|<span data-ttu-id="2a2bd-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a2bd-144">String</span></span>|<span data-ttu-id="2a2bd-145">Identificador de recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="2a2bd-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="2a2bd-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a2bd-146">Response</span></span>
<span data-ttu-id="2a2bd-147">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-147">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a2bd-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a2bd-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a2bd-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a2bd-149">Request</span></span>
<span data-ttu-id="2a2bd-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
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

### <a name="response"></a><span data-ttu-id="2a2bd-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a2bd-151">Response</span></span>
<span data-ttu-id="2a2bd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a2bd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




