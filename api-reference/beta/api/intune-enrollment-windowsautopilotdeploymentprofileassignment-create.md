---
title: Criar windowsAutopilotDeploymentProfileAssignment
description: Criar um novo objeto windowsAutopilotDeploymentProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: abdfb70f36ed8da1166ccb3f3c045271cbddc237
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466420"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="a9c84-103">Criar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="a9c84-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

<span data-ttu-id="a9c84-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a9c84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9c84-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9c84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9c84-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9c84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9c84-107">Criar um novo objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a9c84-107">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9c84-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9c84-108">Prerequisites</span></span>
<span data-ttu-id="a9c84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9c84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9c84-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9c84-111">Permission type</span></span>|<span data-ttu-id="a9c84-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9c84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9c84-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9c84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9c84-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9c84-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a9c84-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9c84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9c84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9c84-116">Not supported.</span></span>|
|<span data-ttu-id="a9c84-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9c84-117">Application</span></span>|<span data-ttu-id="a9c84-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9c84-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9c84-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9c84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a9c84-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9c84-120">Request headers</span></span>
|<span data-ttu-id="a9c84-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9c84-121">Header</span></span>|<span data-ttu-id="a9c84-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a9c84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9c84-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9c84-123">Authorization</span></span>|<span data-ttu-id="a9c84-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9c84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9c84-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9c84-125">Accept</span></span>|<span data-ttu-id="a9c84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9c84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9c84-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9c84-127">Request body</span></span>
<span data-ttu-id="a9c84-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="a9c84-128">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="a9c84-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="a9c84-129">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="a9c84-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9c84-130">Property</span></span>|<span data-ttu-id="a9c84-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9c84-131">Type</span></span>|<span data-ttu-id="a9c84-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9c84-133">id</span><span class="sxs-lookup"><span data-stu-id="a9c84-133">id</span></span>|<span data-ttu-id="a9c84-134">String</span><span class="sxs-lookup"><span data-stu-id="a9c84-134">String</span></span>|<span data-ttu-id="a9c84-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a9c84-135">The key of the assignment.</span></span>|
|<span data-ttu-id="a9c84-136">destino</span><span class="sxs-lookup"><span data-stu-id="a9c84-136">target</span></span>|[<span data-ttu-id="a9c84-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a9c84-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a9c84-138">O destino de atribuição para o perfil de implantação do piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="a9c84-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="a9c84-139">source</span><span class="sxs-lookup"><span data-stu-id="a9c84-139">source</span></span>|[<span data-ttu-id="a9c84-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="a9c84-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="a9c84-141">Tipo de recurso usado para implantação em um grupo, direto ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="a9c84-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="a9c84-142">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="a9c84-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="a9c84-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="a9c84-143">sourceId</span></span>|<span data-ttu-id="a9c84-144">String</span><span class="sxs-lookup"><span data-stu-id="a9c84-144">String</span></span>|<span data-ttu-id="a9c84-145">Identificador para o recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="a9c84-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="a9c84-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9c84-146">Response</span></span>
<span data-ttu-id="a9c84-147">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9c84-147">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9c84-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9c84-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9c84-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9c84-149">Request</span></span>
<span data-ttu-id="a9c84-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9c84-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
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

### <a name="response"></a><span data-ttu-id="a9c84-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9c84-151">Response</span></span>
<span data-ttu-id="a9c84-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9c84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





