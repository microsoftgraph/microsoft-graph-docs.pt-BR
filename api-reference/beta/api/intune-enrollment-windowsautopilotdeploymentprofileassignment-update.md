---
title: Atualizar windowsAutopilotDeploymentProfileAssignment
description: Atualize as propriedades de um objeto windowsAutopilotDeploymentProfileAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8267019105d42260ec346595680ea8d4805c35dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408086"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="37793-103">Atualizar windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="37793-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="37793-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="37793-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37793-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="37793-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37793-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="37793-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37793-107">Atualize as propriedades de um objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="37793-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37793-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37793-108">Prerequisites</span></span>
<span data-ttu-id="37793-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="37793-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="37793-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37793-111">Permission type</span></span>|<span data-ttu-id="37793-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37793-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37793-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37793-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37793-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37793-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="37793-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37793-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37793-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37793-116">Not supported.</span></span>|
|<span data-ttu-id="37793-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37793-117">Application</span></span>|<span data-ttu-id="37793-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37793-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37793-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37793-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="37793-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37793-120">Request headers</span></span>
|<span data-ttu-id="37793-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37793-121">Header</span></span>|<span data-ttu-id="37793-122">Valor</span><span class="sxs-lookup"><span data-stu-id="37793-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37793-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="37793-123">Authorization</span></span>|<span data-ttu-id="37793-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37793-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37793-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37793-125">Accept</span></span>|<span data-ttu-id="37793-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37793-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37793-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37793-127">Request body</span></span>
<span data-ttu-id="37793-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="37793-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="37793-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="37793-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="37793-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37793-130">Property</span></span>|<span data-ttu-id="37793-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="37793-131">Type</span></span>|<span data-ttu-id="37793-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="37793-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37793-133">id</span><span class="sxs-lookup"><span data-stu-id="37793-133">id</span></span>|<span data-ttu-id="37793-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37793-134">String</span></span>|<span data-ttu-id="37793-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="37793-135">The key of the assignment.</span></span>|
|<span data-ttu-id="37793-136">destino</span><span class="sxs-lookup"><span data-stu-id="37793-136">target</span></span>|[<span data-ttu-id="37793-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="37793-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="37793-138">O destino da atribuição para o perfil da implantação piloto automático do Windows.</span><span class="sxs-lookup"><span data-stu-id="37793-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="37793-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="37793-139">Response</span></span>
<span data-ttu-id="37793-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37793-140">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37793-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37793-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="37793-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37793-142">Request</span></span>
<span data-ttu-id="37793-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37793-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="37793-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="37793-144">Response</span></span>
<span data-ttu-id="37793-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37793-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




