---
title: Listar windowsAutopilotDeploymentProfileAssignments
description: Listar Propriedades e relações dos objetos windowsAutopilotDeploymentProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 85e487302608e21df01986d253a5e01f8d5eb4dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35980881"
---
# <a name="list-windowsautopilotdeploymentprofileassignments"></a><span data-ttu-id="f194c-103">Listar windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="f194c-103">List windowsAutopilotDeploymentProfileAssignments</span></span>

> <span data-ttu-id="f194c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f194c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f194c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f194c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f194c-106">Listar Propriedades e relações dos objetos [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f194c-106">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f194c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f194c-107">Prerequisites</span></span>
<span data-ttu-id="f194c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f194c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f194c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f194c-110">Permission type</span></span>|<span data-ttu-id="f194c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f194c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f194c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f194c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f194c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f194c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f194c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f194c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f194c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f194c-115">Not supported.</span></span>|
|<span data-ttu-id="f194c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f194c-116">Application</span></span>|<span data-ttu-id="f194c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f194c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f194c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f194c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f194c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f194c-119">Request headers</span></span>
|<span data-ttu-id="f194c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f194c-120">Header</span></span>|<span data-ttu-id="f194c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f194c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f194c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f194c-122">Authorization</span></span>|<span data-ttu-id="f194c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f194c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f194c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f194c-124">Accept</span></span>|<span data-ttu-id="f194c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f194c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f194c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f194c-126">Request body</span></span>
<span data-ttu-id="f194c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f194c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f194c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f194c-128">Response</span></span>
<span data-ttu-id="f194c-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f194c-129">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f194c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f194c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f194c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f194c-131">Request</span></span>
<span data-ttu-id="f194c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f194c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

### <a name="response"></a><span data-ttu-id="f194c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f194c-133">Response</span></span>
<span data-ttu-id="f194c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f194c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
      "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





