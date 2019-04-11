---
title: Listar windowsAutopilotDeploymentProfileAssignments
description: Listar Propriedades e relações dos objetos windowsAutopilotDeploymentProfileAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2779da775b8a1ee57f43bf9ce622cb3d3ba69767
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792080"
---
# <a name="list-windowsautopilotdeploymentprofileassignments"></a><span data-ttu-id="62387-103">Listar windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="62387-103">List windowsAutopilotDeploymentProfileAssignments</span></span>

> <span data-ttu-id="62387-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62387-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62387-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62387-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62387-106">Listar Propriedades e relações dos objetos [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="62387-106">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62387-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62387-107">Prerequisites</span></span>
<span data-ttu-id="62387-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62387-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62387-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62387-110">Permission type</span></span>|<span data-ttu-id="62387-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62387-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62387-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62387-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62387-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="62387-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="62387-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62387-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62387-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62387-115">Not supported.</span></span>|
|<span data-ttu-id="62387-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62387-116">Application</span></span>|<span data-ttu-id="62387-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62387-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62387-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62387-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="62387-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62387-119">Request headers</span></span>
|<span data-ttu-id="62387-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62387-120">Header</span></span>|<span data-ttu-id="62387-121">Valor</span><span class="sxs-lookup"><span data-stu-id="62387-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62387-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="62387-122">Authorization</span></span>|<span data-ttu-id="62387-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62387-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62387-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62387-124">Accept</span></span>|<span data-ttu-id="62387-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62387-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62387-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62387-126">Request body</span></span>
<span data-ttu-id="62387-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62387-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62387-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="62387-128">Response</span></span>
<span data-ttu-id="62387-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62387-129">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62387-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62387-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="62387-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62387-131">Request</span></span>
<span data-ttu-id="62387-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62387-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

### <a name="response"></a><span data-ttu-id="62387-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="62387-133">Response</span></span>
<span data-ttu-id="62387-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62387-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





