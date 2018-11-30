---
title: Atualizar windowsAutopilotDeploymentProfileAssignment
description: Atualize as propriedades de um objeto windowsAutopilotDeploymentProfileAssignment.
ms.openlocfilehash: 769c1f6e51a1a4702c5a73bb949f56879dbbf57d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038560"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="35387-103">Atualizar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="35387-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="35387-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="35387-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35387-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="35387-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35387-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="35387-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35387-107">Atualize as propriedades de um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="35387-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35387-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="35387-108">Prerequisites</span></span>
<span data-ttu-id="35387-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35387-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35387-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35387-111">Permission type</span></span>|<span data-ttu-id="35387-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="35387-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35387-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35387-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35387-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35387-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="35387-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35387-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35387-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35387-116">Not supported.</span></span>|
|<span data-ttu-id="35387-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35387-117">Application</span></span>|<span data-ttu-id="35387-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35387-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35387-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35387-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="35387-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35387-120">Request headers</span></span>
|<span data-ttu-id="35387-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35387-121">Header</span></span>|<span data-ttu-id="35387-122">Valor</span><span class="sxs-lookup"><span data-stu-id="35387-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35387-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="35387-123">Authorization</span></span>|<span data-ttu-id="35387-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35387-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35387-125">Accept</span><span class="sxs-lookup"><span data-stu-id="35387-125">Accept</span></span>|<span data-ttu-id="35387-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35387-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35387-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35387-127">Request body</span></span>
<span data-ttu-id="35387-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="35387-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="35387-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="35387-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="35387-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35387-130">Property</span></span>|<span data-ttu-id="35387-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="35387-131">Type</span></span>|<span data-ttu-id="35387-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="35387-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35387-133">id</span><span class="sxs-lookup"><span data-stu-id="35387-133">id</span></span>|<span data-ttu-id="35387-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35387-134">String</span></span>|<span data-ttu-id="35387-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="35387-135">The key of the assignment.</span></span>|
|<span data-ttu-id="35387-136">destino</span><span class="sxs-lookup"><span data-stu-id="35387-136">target</span></span>|[<span data-ttu-id="35387-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="35387-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="35387-138">O destino da atribuição para o perfil da implantação piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="35387-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="35387-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="35387-139">Response</span></span>
<span data-ttu-id="35387-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35387-140">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35387-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35387-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="35387-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35387-142">Request</span></span>
<span data-ttu-id="35387-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35387-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="35387-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="35387-144">Response</span></span>
<span data-ttu-id="35387-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35387-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





