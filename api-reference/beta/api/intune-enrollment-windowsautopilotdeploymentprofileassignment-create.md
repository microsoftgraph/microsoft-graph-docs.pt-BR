---
title: Criar windowsAutopilotDeploymentProfileAssignment
description: Crie um novo objeto de windowsAutopilotDeploymentProfileAssignment.
author: tfitzmac
ms.openlocfilehash: c73cd0c8f32ea5b5e84afb5873700a6523186059
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338847"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="4f172-103">Criar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="4f172-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="4f172-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4f172-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f172-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4f172-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f172-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4f172-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f172-107">Crie um novo objeto de [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4f172-107">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f172-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f172-108">Prerequisites</span></span>
<span data-ttu-id="4f172-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f172-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f172-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f172-111">Permission type</span></span>|<span data-ttu-id="4f172-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f172-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f172-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f172-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f172-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f172-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4f172-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f172-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f172-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f172-116">Not supported.</span></span>|
|<span data-ttu-id="4f172-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f172-117">Application</span></span>|<span data-ttu-id="4f172-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f172-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f172-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f172-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4f172-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f172-120">Request headers</span></span>
|<span data-ttu-id="4f172-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f172-121">Header</span></span>|<span data-ttu-id="4f172-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4f172-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f172-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f172-123">Authorization</span></span>|<span data-ttu-id="4f172-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f172-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f172-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4f172-125">Accept</span></span>|<span data-ttu-id="4f172-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f172-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f172-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f172-127">Request body</span></span>
<span data-ttu-id="4f172-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="4f172-128">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="4f172-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="4f172-129">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="4f172-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f172-130">Property</span></span>|<span data-ttu-id="4f172-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f172-131">Type</span></span>|<span data-ttu-id="4f172-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f172-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f172-133">id</span><span class="sxs-lookup"><span data-stu-id="4f172-133">id</span></span>|<span data-ttu-id="4f172-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f172-134">String</span></span>|<span data-ttu-id="4f172-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="4f172-135">The key of the assignment.</span></span>|
|<span data-ttu-id="4f172-136">destino</span><span class="sxs-lookup"><span data-stu-id="4f172-136">target</span></span>|[<span data-ttu-id="4f172-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4f172-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4f172-138">O destino da atribuição para o perfil da implantação piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="4f172-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="4f172-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f172-139">Response</span></span>
<span data-ttu-id="4f172-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f172-140">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f172-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f172-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f172-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f172-142">Request</span></span>
<span data-ttu-id="4f172-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f172-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f172-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f172-144">Response</span></span>
<span data-ttu-id="4f172-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f172-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





