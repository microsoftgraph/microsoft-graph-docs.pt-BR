---
title: Criar windowsAutopilotDeploymentProfileAssignment
description: Crie um novo objeto de windowsAutopilotDeploymentProfileAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5edb72c852be52340eae366c0f2031385fb7ad4d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851741"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="e2872-103">Criar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="e2872-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="e2872-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e2872-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2872-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e2872-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2872-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e2872-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2872-107">Crie um novo objeto de [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e2872-107">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2872-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2872-108">Prerequisites</span></span>
<span data-ttu-id="e2872-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2872-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2872-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2872-111">Permission type</span></span>|<span data-ttu-id="e2872-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2872-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2872-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2872-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2872-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2872-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e2872-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2872-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2872-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2872-116">Not supported.</span></span>|
|<span data-ttu-id="e2872-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2872-117">Application</span></span>|<span data-ttu-id="e2872-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2872-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2872-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2872-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e2872-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2872-120">Request headers</span></span>
|<span data-ttu-id="e2872-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2872-121">Header</span></span>|<span data-ttu-id="e2872-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e2872-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2872-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2872-123">Authorization</span></span>|<span data-ttu-id="e2872-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2872-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2872-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2872-125">Accept</span></span>|<span data-ttu-id="e2872-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2872-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2872-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2872-127">Request body</span></span>
<span data-ttu-id="e2872-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="e2872-128">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="e2872-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsAutopilotDeploymentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="e2872-129">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="e2872-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2872-130">Property</span></span>|<span data-ttu-id="e2872-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2872-131">Type</span></span>|<span data-ttu-id="e2872-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2872-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2872-133">id</span><span class="sxs-lookup"><span data-stu-id="e2872-133">id</span></span>|<span data-ttu-id="e2872-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2872-134">String</span></span>|<span data-ttu-id="e2872-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="e2872-135">The key of the assignment.</span></span>|
|<span data-ttu-id="e2872-136">destino</span><span class="sxs-lookup"><span data-stu-id="e2872-136">target</span></span>|[<span data-ttu-id="e2872-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e2872-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e2872-138">O destino da atribuição para o perfil da implantação piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="e2872-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="e2872-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2872-139">Response</span></span>
<span data-ttu-id="e2872-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2872-140">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2872-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2872-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2872-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2872-142">Request</span></span>
<span data-ttu-id="e2872-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2872-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e2872-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2872-144">Response</span></span>
<span data-ttu-id="e2872-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2872-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





