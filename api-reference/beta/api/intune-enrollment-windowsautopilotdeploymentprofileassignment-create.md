---
title: Criar windowsAutopilotDeploymentProfileAssignment
description: Crie um novo objeto de windowsAutopilotDeploymentProfileAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a336ac9540c90cdebf452a08037bd46d5fa33d01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983622"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="a0bfc-103">Criar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="a0bfc-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="a0bfc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0bfc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0bfc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0bfc-107">Crie um novo objeto de [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a0bfc-107">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0bfc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0bfc-108">Prerequisites</span></span>
<span data-ttu-id="a0bfc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0bfc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0bfc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0bfc-111">Permission type</span></span>|<span data-ttu-id="a0bfc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0bfc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0bfc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0bfc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0bfc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0bfc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a0bfc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0bfc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0bfc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-116">Not supported.</span></span>|
|<span data-ttu-id="a0bfc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0bfc-117">Application</span></span>|<span data-ttu-id="a0bfc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0bfc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0bfc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a0bfc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bfc-120">Request headers</span></span>
|<span data-ttu-id="a0bfc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0bfc-121">Header</span></span>|<span data-ttu-id="a0bfc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0bfc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0bfc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0bfc-123">Authorization</span></span>|<span data-ttu-id="a0bfc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0bfc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0bfc-125">Accept</span></span>|<span data-ttu-id="a0bfc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0bfc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0bfc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bfc-127">Request body</span></span>
<span data-ttu-id="a0bfc-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-128">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="a0bfc-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-129">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="a0bfc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0bfc-130">Property</span></span>|<span data-ttu-id="a0bfc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0bfc-131">Type</span></span>|<span data-ttu-id="a0bfc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0bfc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0bfc-133">id</span><span class="sxs-lookup"><span data-stu-id="a0bfc-133">id</span></span>|<span data-ttu-id="a0bfc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0bfc-134">String</span></span>|<span data-ttu-id="a0bfc-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-135">The key of the assignment.</span></span>|
|<span data-ttu-id="a0bfc-136">destino</span><span class="sxs-lookup"><span data-stu-id="a0bfc-136">target</span></span>|[<span data-ttu-id="a0bfc-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a0bfc-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a0bfc-138">O destino da atribuição para o perfil da implantação piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="a0bfc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0bfc-139">Response</span></span>
<span data-ttu-id="a0bfc-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-140">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0bfc-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0bfc-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a0bfc-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bfc-142">Request</span></span>
<span data-ttu-id="a0bfc-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0bfc-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0bfc-144">Response</span></span>
<span data-ttu-id="a0bfc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0bfc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





